# How to create a Customer Computed-Last Attribute

## Use case:

You want to create an attribute that **returns the name of the product visited by a customer  - Last viewed product**

## Steps:

You can follow these steps below in order to create a Customer Computed Attribute:

1. Hover your mouse over **Data** (on the left hand side menu), then click **Data Object** and select **Customer**

<figure><img src="../../../.gitbook/assets/image (3013).png" alt=""><figcaption></figcaption></figure>

2\. Select **Attributes** on the left hand side, click **+** button, and then select **Create new Attribute**

<figure><img src="../../../.gitbook/assets/image (3014).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (3016).png" alt=""><figcaption></figcaption></figure>

3\. At the Create a new attribute interface, choose **Last - Computed Attribute Types**

<figure><img src="../../../.gitbook/assets/image (3017).png" alt=""><figcaption></figcaption></figure>

4\. **Configure computed attribute - Last viewed product**:&#x20;

* **General information**:&#x20;
  * Group attribute: Web Analytics History
  * Attribute name: Last viewed Product&#x20;
  * Attribute internal code: last\_viewe&#x64;_\__&#x70;roduct
  * Description: The product that the customer viewed the last time

<figure><img src="../../../.gitbook/assets/image (3018).png" alt=""><figcaption></figcaption></figure>

* **Setting:**
  * Time range: All time
  * Events: View product
  * Sources: Websites
  * Event attribute: Product >> Name
  * Display format: Raw string

<figure><img src="../../../.gitbook/assets/image (3019).png" alt=""><figcaption></figcaption></figure>

* **Computation schedule:**
  * Repeat by: Day, at 3:00 AM
  * Repeat every: 1 day
  * Start time: 06/10/2022
  * End time: On 13/10/2022 at 02:00 AM

<figure><img src="../../../.gitbook/assets/image (3020).png" alt=""><figcaption></figcaption></figure>

* **Notification Setup**: Notify when the computation fails by sending an Email and pushing a notification

<figure><img src="../../../.gitbook/assets/image (3021).png" alt=""><figcaption></figcaption></figure>

5\. Click ![](<../../../.gitbook/assets/image (2530).png>)

## The result of the attribute

### Process status

You can find the process status, size, and more information about the **Last viewed Product** in the **Attribute Data table**&#x20;

<figure><img src="../../../.gitbook/assets/image (3022).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (3024).png" alt=""><figcaption></figcaption></figure>

### The returned value corresponding result of the computed attribute

You can find the value **Last viewed Product of each customer** in the **Customer Data table**

<figure><img src="../../../.gitbook/assets/image (3025).png" alt=""><figcaption></figcaption></figure>

{% embed url="https://drive.google.com/file/d/1oAsA86DkPMySRXGsuZtqIPmVSllE48GX/view?usp=sharing" %}

