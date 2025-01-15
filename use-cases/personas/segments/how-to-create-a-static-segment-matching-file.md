# How to create a Static Segment (Matching file)

## Use case:

I have a group of customers who have a number of purchases in the fair, the information about them was stored in my local file. I want to create a **VIP Customer segment** that the data from the system matches my file

<figure><img src="../../../.gitbook/assets/Create Static Segment - Matching file – My file.png" alt=""><figcaption></figcaption></figure>

## Prerequisites:

A file of Customers (file formats include: .csv, .xls, .xlsx)

## Steps:

1. On the left hand side menu, hover your mouse over **Profiles**, select **Segments**, click ![](<../../../.gitbook/assets/image (1779).png>)and choose **Customer Segment** in the Segment data table interface&#x20;

<figure><img src="../../../.gitbook/assets/image (3039).png" alt=""><figcaption></figcaption></figure>

2\. **Configure Segment:**

**2.1.** Audience Name: VIP Customers

**2.2.** Update Segment: Static Segment - no update

**2.3.** Member input method: Matching file

**2.4**. After choosing the Member input method, the system will display Upload your audiences file.

Click **Browse** and select file name **VIP** **Customer** from the Local

<figure><img src="../../../.gitbook/assets/image (3041).png" alt=""><figcaption></figcaption></figure>

**2.5**. Click **Add Criteria** and input **criteria**

* Choose logic between 2 criteria: OR
* Criteria 1:&#x20;
  * The field in the system: Name (name)
  * Condition: is exactly&#x20;
  * Matching column: Name
* Criteria 2:
  * The field in the system: Email (email)
  * Condition: is exactly&#x20;
  * Matching column: Email

<figure><img src="../../../.gitbook/assets/image (3042).png" alt=""><figcaption></figcaption></figure>

**2.6.** Segment Member: No limit

<figure><img src="../../../.gitbook/assets/Create Static Segment - Matching file – Segment member.png" alt=""><figcaption></figcaption></figure>

**2.7.** Notification Setup: Notify when the computation fails by **sending an Email and pushing a notification**

<figure><img src="../../../.gitbook/assets/image (3043).png" alt=""><figcaption></figcaption></figure>

3\. Click **Save**

## The result of Segment Computation

### Computation Status

You can check the **Computation Status** of the **VIP Customer** in the data table of the **Computation History** tab

<figure><img src="../../../.gitbook/assets/image (3045).png" alt=""><figcaption></figcaption></figure>

### Segment information

You can find **detailed information about the Segment** by clicking Segment name - **VIP Customer**

<figure><img src="../../../.gitbook/assets/image (3046).png" alt=""><figcaption></figcaption></figure>

## Guidance video

{% embed url="https://drive.google.com/file/d/1s9VMsxunhFPC817POmA06O9d1FTP7W2t/view?usp=sharing" %}
