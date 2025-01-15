# Set up Dataflows to push data to a Business Object in CDP 365

## **Push data from Dataflows to Business Object in DATA HUB**

&#x20;   1\. Log into the **CDP 365** system.

&#x20;   2\. Hover your mouse over **Data** -> Choose **Batch Stream**

<figure><img src="../../.gitbook/assets/image (3507).png" alt=""><figcaption></figcaption></figure>

&#x20; 3\. Click **+** button to create a Dataflow

<figure><img src="../../.gitbook/assets/image (3508).png" alt=""><figcaption></figcaption></figure>

&#x20;  4\. Select a Data source (containing data) that you want to push into the **Data object** in CDP 365

<figure><img src="../../.gitbook/assets/image (3512).png" alt=""><figcaption></figcaption></figure>

Click **Create stream** after you have selected Data source

&#x20;  5\.  Select the necessary fields for your data push

<figure><img src="../../.gitbook/assets/image (3514).png" alt=""><figcaption></figcaption></figure>

You can click the **Preview** button to check the accuracy of data at each node

<figure><img src="../../.gitbook/assets/image (3515).png" alt=""><figcaption></figcaption></figure>

&#x20;  6\. Add **Destination channel** node -> Select the Business Object destination channel that you created before

<figure><img src="../../.gitbook/assets/image (3518).png" alt=""><figcaption></figcaption></figure>

&#x20;  7\. Set up the necessary information to push data into the Data Object

<figure><img src="../../.gitbook/assets/image (3519).png" alt=""><figcaption></figcaption></figure>

&#x20;  8\. Set up a **schedule** that you want the **Dataflow** to execute

<figure><img src="../../.gitbook/assets/image (3520).png" alt=""><figcaption></figcaption></figure>

&#x20;  9\. Some features you need to pay attention to when setting up Dataflows

<figure><img src="../../.gitbook/assets/image (3521).png" alt=""><figcaption></figcaption></figure>

&#x20;      (1) **Version history:** Version history lets you view or restore previous revisions

&#x20;      (2) **Force Run:** You can run dataflow immediately without waiting for the scheduled time

&#x20;      (3) **Save:** Save your dataflow after editing

&#x20;      (4) **Activate:** Active your dataflow (you must active the Dataflows if you want to run on schedule)



&#x20;  10\. You can check the progress and running results of Dataflows at the **Action log** Tab

<figure><img src="../../.gitbook/assets/image (3522).png" alt=""><figcaption></figcaption></figure>

## **Push promotion code from Dataflows to promotion pool in CDP**

&#x20;   1\. Log into the CDP 365 system.&#x20;

&#x20;    2\. Hover your mouse over **Data** -> Choose **Batch Stream**

<figure><img src="../../.gitbook/assets/image (3523).png" alt=""><figcaption></figcaption></figure>

&#x20;   3\. Click **+** button to create a Dataflow

<figure><img src="../../.gitbook/assets/image (3524).png" alt=""><figcaption></figcaption></figure>

&#x20;   4\. Select a Datasource (containing data) that you want to push into the **promotion pool** in CDP

<figure><img src="../../.gitbook/assets/image (3525).png" alt=""><figcaption></figcaption></figure>

Click **Create stream** after you have selected the Data source.

&#x20;   5\. Select the field containing the data of the **promotion code** that you want to push into the **promotion pool** of CDP

<figure><img src="../../.gitbook/assets/image (3526).png" alt=""><figcaption></figcaption></figure>

&#x20;    6\. Add a **Destination Channel** that you have connected before

<figure><img src="../../.gitbook/assets/image (3527).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (3528).png" alt=""><figcaption></figcaption></figure>

&#x20;    7\. **Save** Dataflow

&#x20;    8\. Set up the schedule to run for Dataflows, then **Activate** the Dataflow.

&#x20;           **Note: You can use the Force Run feature to run immediately**

&#x20;     9\. After the Dataflow runs complete, you can go to the promotion code tab in the pool that you selected to check the results

<figure><img src="../../.gitbook/assets/image (3529).png" alt=""><figcaption></figcaption></figure>
