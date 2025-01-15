# How to create Coupon from Magento or ERP system to CDP 365?

### Create a Data Source

&#x20;1\. Log into the **CDP 365** system.

&#x20;2\. Hover your mouse over **Data**, and choose **Source** under **Dataflows**.

<figure><img src="../../.gitbook/assets/image (3535).png" alt=""><figcaption></figcaption></figure>

3\. Click <img src="../../.gitbook/assets/image (596).png" alt="" data-size="line"> to create Data Source. Choose **Batch**.

<figure><img src="../../.gitbook/assets/image (3536).png" alt=""><figcaption></figcaption></figure>

4\. Select **MySQL** Connector

<figure><img src="../../.gitbook/assets/image (3538).png" alt=""><figcaption></figcaption></figure>

4\. Input the necessary information to connect to your database to get the data coupon. Then click the **Authenticate** button

<figure><img src="../../.gitbook/assets/image (3539).png" alt=""><figcaption></figcaption></figure>

5\. Input the **Data Source name** then click the **Connect** button to connect

### Create a Dataflow to push data coupons into CDP

&#x20;1\. Log into the **CDP 365** system. After logging in, click the menu in the left corner of the screen

&#x20;2\. Select the menu as follows: "**DATAFLOWS" -> "Dataflows"**

<figure><img src="../../.gitbook/assets/image (3540).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (679).png" alt=""><figcaption></figcaption></figure>

3\. Click **+** button to create a Dataflow

<figure><img src="../../.gitbook/assets/image (3530).png" alt=""><figcaption></figcaption></figure>

4\. Select the **MySQL** data source that you created earlier, then click the **Create dataflow** button

[Create a "MySQL" Datasource](how-to-create-coupon-from-magento-or-erp-system-to-cdp-365.md#create-a-new-datasource)

<figure><img src="../../.gitbook/assets/image (3533).png" alt=""><figcaption></figcaption></figure>

5\. Select the **fields** contains coupon data that you want to push to **CDP 365**

<figure><img src="../../.gitbook/assets/image (891).png" alt=""><figcaption></figcaption></figure>

6\. Add a **Destination channel** node. Select the **Data Coupon** destination channel you created earlier

**You can see how to create a Data Coupon destination channel** [**here**](../dataflows/how-to-create-a-destination-channel-in-dataflows.md)&#x20;

<figure><img src="../../.gitbook/assets/image (1051).png" alt=""><figcaption></figcaption></figure>

7\. Select the pool you created earlier on the CDP to which you want to push Coupon data

**NOTE: You should create an empty pool first. You can see how to create a pool** [**here**](../../marketing-hub/promotion-center.md)

<figure><img src="../../.gitbook/assets/image (650).png" alt=""><figcaption></figcaption></figure>

8\. Save dataflow

9\. Set up a schedule that you want the **Dataflows** to execute

<figure><img src="../../.gitbook/assets/image (951).png" alt=""><figcaption></figcaption></figure>

**Note: Force Run ->** You can run dataflow immediately without waiting for the scheduled time

<figure><img src="../../.gitbook/assets/image (2070).png" alt=""><figcaption></figcaption></figure>
