# How to Send email using "Amazon SES" in CDP 365

1\. Log in to **CDP 365**. Hover your mouse over **Settings**. Choose **Channel Integration**.

<figure><img src="../../.gitbook/assets/image (3181).png" alt=""><figcaption></figcaption></figure>

2\. Click **+** button and select **Email**

<figure><img src="../../.gitbook/assets/image (3182).png" alt=""><figcaption></figcaption></figure>

3\. Select **Destination catalog**: **Amazon SES**

<figure><img src="../../.gitbook/assets/image (3285).png" alt=""><figcaption></figcaption></figure>

4\. Fill in the necessary information for the destination

<figure><img src="../../.gitbook/assets/image (3287).png" alt=""><figcaption></figcaption></figure>

| Field              | Description                                                                                                                                                                                                                                                                                   |
| ------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Email              | <p>Email recipients. </p><p>You can click <img src="../../.gitbook/assets/image (1881).png" alt=""> icon to add Personalization</p><p><img src="../../.gitbook/assets/image (3185).png" alt="" data-size="original"></p>                                                                      |
| Access Key         | [Get your access key ID and secret access key](https://app.gitbook.com/o/-LzunofLVjpTa_-p1PQt/s/mECwNqMNUmu6OXHSYgDv/quick-start-guide/how-to-send-email-using-amazon-ses-in-cdp-365#get-your-access-key-id-and-secret-access-key)                                                            |
| Secret Key         | [Get your access key ID and secret access key](how-to-send-email-using-amazon-ses-in-cdp-365.md#get-your-access-key-id-and-secret-access-key)                                                                                                                                                 |
| Region             | <p>The region where your email is verified</p><p><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FfTupBie2WQUOB4pWevvh%2Fimage.png?alt=media&#x26;token=3e58b660-a452-4c81-bb4c-52fc47f1b782" alt="" data-size="original"></p> |
| From Email Name    | Sender name                                                                                                                                                                                                                                                                                   |
| From Email Address | A regional email address that you verified with Amazon SES                                                                                                                                                                                                                                    |

#### **Get your access key ID and secret access key**

1. Open the IAM console at [https://console.aws.amazon.com/iam/](https://console.aws.amazon.com/iam/).
2. On the navigation menu, choose **Users**.
3. Choose your IAM user name (not the check box).
4. Open the **Security credentials** tab, and then choose **Create access key**.
5. To see the new access key, choose **Show**. Your credentials resemble the following:
   * Access key ID: `AKIAIOSFODNN7EXAMPLE`
   * Secret access key: `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY`&#x20;

5\. Click **Save** to finish creating the **Amazon SES** destination

<figure><img src="../../.gitbook/assets/image (3288).png" alt=""><figcaption></figcaption></figure>

6\. Sending email using **Amazon SES** via Customer Journey

Log into CDP 365 system. Hover your mouse over **Marketing** and go to **All Channels** menu.

<figure><img src="../../.gitbook/assets/image (3188).png" alt=""><figcaption></figcaption></figure>

We have 2 channels that supporting to send:

* Email
* Orchestration

<figure><img src="../../.gitbook/assets/image (3189).png" alt=""><figcaption></figcaption></figure>

Click **+** button to Create Journey.

<figure><img src="../../.gitbook/assets/image (3190).png" alt=""><figcaption></figcaption></figure>

Add **Destination** node and select **Amazon SES** destination

<figure><img src="../../.gitbook/assets/image (3289).png" alt=""><figcaption></figcaption></figure>

Select a **Amazon SES** destination that you have created before

<figure><img src="../../.gitbook/assets/image (3290).png" alt=""><figcaption></figcaption></figure>

Fill out necessary information, and choose a template or create one yourself.

<figure><img src="../../.gitbook/assets/image (3291).png" alt=""><figcaption></figcaption></figure>

Click **Save** button to finish setting journey

<figure><img src="../../.gitbook/assets/image (3292).png" alt=""><figcaption></figcaption></figure>

After finishing the setting of the Journey, we can click **Activate** and send email to customer.
