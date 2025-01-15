# Data Format

## Data type

CDP 365 provides a number of data types:&#x20;

| Data type                            | Description                                                                                                                                              |
| ------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Number](data-format.md#number)      | Numeric data                                                                                                                                             |
| [String](data-format.md#string)      | String data - limited to 255 characters                                                                                                                  |
| Text                                 | Text-type data - limited to 30,000 characters                                                                                                            |
| [Datetime ](data-format.md#datatime) | Datetime type data                                                                                                                                       |
| Boolean                              |                                                                                                                                                          |
| Array                                | <p>Array data, including: </p><ul><li>Array of Numbers: mảng số</li><li>Array of Strings: mảng chuỗi</li><li>Array of Datetimes: mảng ngày giờ</li></ul> |
| [Object](data-format.md#object)      | Object type data                                                                                                                                         |

## Display format

After selecting the [Data type](data-format.md#data-type), click Edit to change the display format:

{% hint style="warning" %}
Note: the maximum number of characters that can be displayed is 15 characters
{% endhint %}

### Number

For numeric data, there are 3 display formats:

* **Number**
* **Percentage**
* **Currency**

{% tabs %}
{% tab title="Number" %}
![](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-MfSgjdWJGVBoBw27MYp%2Fuploads%2FeYL8vM3ucK3GWqHw73tV%2Fimage.png?alt=media\&token=01d70858-a19d-476e-a23a-8a5d33bf332b)

* **Display format:** sample data display area after adjustment
* **Use portal default:** use Portal's default settings
* **Custom:** customize
* **Decimal places:** decimal point position
* **Grouping:** mark to group thousands
* **Decimal:** integer and decimal division mark
{% endtab %}

{% tab title="Percentage " %}
![](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-MfSgjdWJGVBoBw27MYp%2Fuploads%2FtKNXJwEEI5mQvV4FV5el%2Fimage.png?alt=media\&token=3dd10504-12b9-41df-b86f-c66d3225161a)

* **Display format:** vùng hiển thị dữ liệu mẫu sau khi điều chỉnh
* **Use portal default:** sử dụng cài đặt mặc định của Portal
* **Custom:** tùy biến
* **Decimal places:** vị trí dấu thập phân
* **Grouping:** dấu phân nhóm hàng ngàn
* **Decimal:** dấu phân nhóm phần nguyên và phần thập phân​
{% endtab %}

{% tab title="Currency" %}
![](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-MfSgjdWJGVBoBw27MYp%2Fuploads%2F7UFcB1rS1AYtTu8duXuQ%2Fimage.png?alt=media\&token=775c5d9f-e808-4102-a70a-fd23c04e69de)

* **Display format:** vùng hiển thị dữ liệu mẫu sau khi điều chỉnh
* **Use portal default:** sử dụng cài đặt mặc định của Portal
* **Custom:** tùy biến
* **Edit Currency:** điều chỉnh loại tiền tệ
* **Decimal places:** vị trí dấu thập phân
* **Grouping:** dấu phân nhóm hàng ngàn
* **Decimal:** dấu phân nhóm phần nguyên và phần thập phân
{% endtab %}
{% endtabs %}

### String

For string data, there are 3 display formats:&#x20;

* **Raw String:** strings
* **Image:** Pictures can be hovered to view
* **Link:** clickable link to open

{% tabs %}
{% tab title="Raw String" %}
![](<../.gitbook/assets/image (1849).png>)
{% endtab %}

{% tab title="Image" %}
![](<../.gitbook/assets/image (1139).png>)
{% endtab %}

{% tab title="Link" %}
![](<../.gitbook/assets/image (1985).png>)
{% endtab %}
{% endtabs %}

### Datatime

![](<../.gitbook/assets/image (2473).png>)

* **Display format:** sample data display area after adjustment
* **Use portal default:** use Portal's default settings
* **Custom:** customization



* **Data display format:** hiển thị định dạng ngày
  * Short: `tháng/ ngày/ năm`
  * Medium: `tháng (chữ tắt)/ ngày năm`
  * Long: `tháng (chữ đầy đủ)/ ngày năm`

{% hint style="info" %}
Format: <mark style="color:green;">MM/DD/YYYY HH:MM:SS</mark> \
hoặc <mark style="color:green;">DD/MM/YYYY HH:MM:SS</mark>
{% endhint %}



* **Time display format:** hiển thị định dạng giờ
  * Short: `giờ: phút`
  * Medium: `giờ: phút: giây`
  * Long: `giờ: phút: giây GT`

{% hint style="info" %}
Định dạng: <mark style="color:green;">12 giờ (AM/ PM)</mark>

hoặc <mark style="color:green;">24 giờ</mark>
{% endhint %}

### Object

![](<../.gitbook/assets/image (1527).png>)

* **Key name:** tên khóa
* **Key code:** mã khóa
* **Data-type:** [kiểu dữ liệu](data-format.md#data-type)
* **Default value:** giá trị mặc định
* **Is Required:** có bắt buộc?
* **Clear all:** xóa tất cả

## Data rule format

* **Is Required:** Is field selection mandatory?
* **Auto suggestion:** Check if you want the attribute value to show in the Filter
* **Enable Data Encryption:** tích chọn để mã hóa dữ liệu
