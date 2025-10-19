---
description: >-
  Hệ thống Search được thiết kế như một lớp ứng dụng của CDP, nơi mọi truy vấn
  tìm kiếm đều được xử lý và xếp hạng dựa trên dữ liệu hành vi thực tế của người
  dùng.
---

# System Search

Đối với các hệ thống **Search** , hầu hết các mô hình triển khai thực tế đều tuân theo một cấu trúc tương tự.\
Cụ thể, toàn bộ quy trình thường được chia thành hai trục chính:

* **Môi trường xử lý:** tách biệt giữa **offline** (huấn luyện, xây dựng dữ liệu) và **online** (xử lý truy vấn thời gian thực).
* **Giai đoạn xử lý:** bao gồm hai bước chính là **retrieval (truy xuất ứng viên)** và **ranking (xếp hạng kết quả)**.

Hình minh họa dưới đây mô tả mô hình “2 x 2” giúp đơn giản hóa và làm rõ cấu trúc này:

<figure><img src="../../.gitbook/assets/System Search-Overall_1.png" alt="Hệ thống Search, dựa trên mô hình “2 x 2”"><figcaption></figcaption></figure>

#### Môi trường Offline và Online trong hệ thống Search

**Môi trường&#x20;**_**offline**_ chủ yếu phục vụ các tiến trình xử lý theo lô (_batch processes_) như:

* **Xây dựng** model ranking (ví dụ: , mô hình xếp hạng – _ranking_).
* **Sinh vector embedding** cho toàn bộ sản phẩm trong _Product feed_.
* **Xây dựng chỉ mục lân cận gần ( Index)**  để tìm các item tương tự.
* **Tải dữ liệu Product và Behavior Customer vào Feature Store**, nơi sẽ được dùng để bổ sung đặc trưng cho dữ liệu đầu vào trong giai đoạn xếp hạng.
* **Tracking hành vi** click product sau khi nhận kết quả

**Môi trường&#x20;**_**online**_ sử dụng các “data” đã được tạo ra từ offline (như  Index, mô hình, feature store) để phục vụ **các yêu cầu truy vấn thời gian thực** của người dùng.\
Quy trình điển hình gồm các bước:

1. Xử lý điều kiện đầu vào.
2. Thực hiện truy xuất ứng viên (candidate retrieval).
3. Xử lý Score (boosting score)
4. Tiến hành xếp hạng (ranking).

Để hình dung rõ hơn toàn bộ luồng hoạt động từ khi dữ liệu được xử lý đến khi kết quả tìm kiếm được trả về cho người dùng, sơ đồ dưới đây trình bày chi tiết cách hệ thống _Search_ vận hành giữa hai môi trường **Offline** (huấn luyện, xây dựng dữ liệu) và **Online** (xử lý truy vấn thời gian thực).

<figure><img src="../../.gitbook/assets/System Search-Detail_1.png" alt=""><figcaption></figcaption></figure>

#### **Ví dụ luồng hoạt động của hệ thống Search**

Giả sử người dùng tìm kiếm từ khóa _**“thịt heo”**_ trên trang web:

1. **Client → Query**\
   Người dùng nhập từ khóa _**“thịt heo”**_. Request được gửi đến hệ thống _Search Service_.
2. **Search Service – Filter & Keyword Handling**
   * Hệ thống xử lý cú pháp, tách từ khóa và kiểm tra điều kiện lọc (ví dụ: danh mục sản phẩm, promotion, price).
   * Tiếp theo, Search Service xác định xem từ khóa có **khớp chính xác (exact match)** với tên sản phẩm nào trong hệ thống hay không.
3.  **Filter “exact match”**

    *   **Nếu YES:**\
        Hệ thống chỉ truy vấn theo trường `"title"` (tên sản phẩm).

        ```
        query_by = "title"
        pinned = product_ads
        ```

        → Ví dụ: “thịt heo rừng” sẽ được hiển thị.
    *   **Nếu NO:**\
        Hệ thống mở rộng phạm vi tìm kiếm theo nhiều trường: `"title"` và `"category"`, đồng thời gán trọng số khác nhau.

        ```
        query_by = "title,category"
        query_by_weights = "1,5"
        pinned = product_ads
        ```

        → Giúp lấy thêm các sản phẩm có liên quan trong cùng danh mục  “thịt heo”

    **Note:** `pinned = product_ads` → **ghim các sản phẩm quảng cáo lên đầu danh sách ứng viên** trước khi thực hiện boosting/ranking.
4.  **Boosting Score – Ưu tiên kết quả**\
    Sau khi lấy được danh sách sản phẩm từ _Antsomi search engine_, hệ thống **tăng điểm ưu tiên (boost)** cho các sản phẩm:

    * Đã từng được người dùng **click nhiều nhất** cho từ khóa này.
    * Hoặc **đã từng được chính khách hàng này mua** trước đó.

    → Ví dụ:\
    Nếu người dùng từng mua “Ba rọi heo” thì sản phẩm đó sẽ được đẩy lên cao hơn trong danh sách kết quả cho từ khóa “thịt heo”.\
    Hoặc: với từ khóa "thịt heo" sản phẩm "Giò heo" được click nhiều nhất trong vòng 30 ngày qua, hệ thống sẽ ưu tiên đẩy sản phẩm "Giò heo" lên top đầu
5. **Ranking Model – Xếp hạng kết quả**\
   Dữ liệu đã được boost score sẽ được gửi vào mô hình xếp hạng (Ranking Model).\
   Mô hình này tính toán điểm tổng hợp dựa trên nhiều yếu tố (độ phù hợp, hành vi người dùng, quảng cáo được ghim, v.v.) để sắp xếp thứ tự hiển thị cuối cùng.
6. **Return Data – Trả kết quả cho người dùng**\
   Hệ thống trả về danh sách sản phẩm đã được xếp hạng tối ưu lên giao diện người dùng.
7. **History Click after Search – Ghi nhận hành vi**\
   Khi người dùng click vào sản phẩm sau khi Search, hành vi này được ghi nhận lại vào **History Click** để:
   * Cập nhật dữ liệu học cho mô hình _Ranking_ (offline retraining).
   * Nâng độ chính xác cho các lần tìm kiếm sau.

Tổng kết lại, Search hoạt động như một lớp ứng dụng tận dụng dữ liệu CDP để hiểu rõ người dùng hơn. Mỗi kết quả được trả về không chỉ dựa trên độ khớp của từ khóa, mà còn dựa trên **hành vi, lịch sử tương tác và khả năng chuyển đổi của người dùng**, giúp kết quả tìm kiếm trở nên chính xác và mang tính cá nhân hóa cao hơn.
