# How to create a Dynamic Segment

## Use case:

I want to create a segment in which the customers have viewed products of Men at least 1 time in the last 30 days and compute it 6 times

## Steps:

1. On the left hand side menu, hover your mouse over **Profiles**, select **Segments**, click ![](<../../../.gitbook/assets/image (1779).png>)and choose **Customer Segment** in the Segment data table interface&#x20;

<figure><img src="../../../.gitbook/assets/image (3027).png" alt=""><figcaption></figcaption></figure>

2\. **Configure Segment:**

**2.1.** Audience Name: Customer viewed Men Product in the last 30 days

**2.2.** Update Segment: Dynamic Segment - scheduled update

**2.3.** Member input method: Conditions

**2.4**. Include people that: click **Add condition,** select **Perform event**, and choose **Event Counter**

<figure><img src="../../../.gitbook/assets/image (3028).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (3029).png" alt=""><figcaption></figcaption></figure>

*   Select event: View product

    Condition: greater than 1 (times)
* In any source of: Websites
*   Where: Product>>product.cate\_l1

    Condition: match any of Men
* Time range: Last 30 days

<figure><img src="../../../.gitbook/assets/image (3030).png" alt=""><figcaption></figcaption></figure>

**2.5.** Segment Member: No limit

<figure><img src="../../../.gitbook/assets/Create Static Segment - Matching file – Segment member.png" alt=""><figcaption></figcaption></figure>

2.6. Computation Schedule:&#x20;

* Repeat by: day at 03:00 AM
* Repeat every 1 day
* Start time: 02/08/2024
* End time: after 6 occurrences

<figure><img src="../../../.gitbook/assets/image (3032).png" alt=""><figcaption></figcaption></figure>

**2.7.** Notification Setup: Notify when the computation fails by **sending an Email and pushing a notification**

<figure><img src="../../../.gitbook/assets/image (3033).png" alt=""><figcaption></figcaption></figure>

**2.8. Forecast (optional)**

You can preview a sample of users in this audience by clicking **Forecast** on the right of the screen

<figure><img src="../../../.gitbook/assets/image (3034).png" alt=""><figcaption></figcaption></figure>

The Forecast is:&#x20;

<figure><img src="../../../.gitbook/assets/image (3035).png" alt=""><figcaption></figcaption></figure>

3\. Click **Save**

## The result of Segment Computation

### Computation Status

You can check the **Computation Status of the Customer viewed Men Product in the last 30 days** in the data table of the **Computation History** tab

<figure><img src="../../../.gitbook/assets/image (3037).png" alt=""><figcaption></figcaption></figure>

### Segment information

You can find **detailed information about the Segment** by clicking Segment name - **Customer viewed Men Product in the last 30 days**

<figure><img src="../../../.gitbook/assets/image (3038).png" alt=""><figcaption></figcaption></figure>

{% embed url="https://drive.google.com/file/d/181MYc8R77n0dbeRInTEz8SRw4fYJPC10/view?usp=sharing" %}
