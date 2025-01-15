# How to Send email  using "SendGrid" in CDP 365

### 1. Log in to **CDP 365**. Hover your mouse over **Settings**. Choose **Channel Integration**.

<figure><img src="../../.gitbook/assets/image (3351).png" alt=""><figcaption></figcaption></figure>

### 2. Click + button and select Email

<figure><img src="../../.gitbook/assets/image (3352).png" alt=""><figcaption></figcaption></figure>

### 3. Select Destination catalog: SendGrid

<figure><img src="../../.gitbook/assets/image (3348).png" alt=""><figcaption></figcaption></figure>

### 4. Fill in the necessary information for the destination

<figure><img src="../../.gitbook/assets/image (3349).png" alt=""><figcaption></figcaption></figure>

| Field                | Description                                                                                                                                                                                                              |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| To Email             | <p>Email recipients. </p><p>You can click <img src="../../.gitbook/assets/image (1858).png" alt=""> icon to add Personalization</p><p><img src="../../.gitbook/assets/image (3356).png" alt="" data-size="original"></p> |
| CC Email             | Use to send an email to many people same time                                                                                                                                                                            |
| API Key              | [API key that you created on SendGrid](how-to-send-email-using-sendgrid-in-cdp-365.md#how-to-create-api-key-on-sendgrid)                                                                                                 |
| From Email Name      | Sender name                                                                                                                                                                                                              |
| From Email Address   | Email that you use to send to customers                                                                                                                                                                                  |
| Unsubscribe Group Id | [ID of Unsubcribe Group that you create on SendGrid (optional)](how-to-send-email-using-sendgrid-in-cdp-365.md#how-to-create-an-unsubscribe-group)                                                                       |

### How to create "API Key" on "SendGrid"

&#x20;  1\. Login **SendGrid** system

&#x20;  2\. Navigate to **Settings** on the left navigation bar, and then select **API Keys**.

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2Fg3L36dgcmXRduiU93bBO%2Fimage.png?alt=media&#x26;token=edbcf413-9687-47ef-b61c-0bc3b1933334" alt=""><figcaption></figcaption></figure>

&#x20; 3\. Click **Create API Key**.

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2Fand6ecJNWsglbKO9Bylo%2Fimage.png?alt=media&#x26;token=aea0e2da-2e4e-4932-aa94-f93c5802933b" alt=""><figcaption></figcaption></figure>

&#x20;  4\. Give your API key a name and select **Full Access**, **Restricted Access**, or **Billing Access**.

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2F1FxNqm2lJ3GaYucN5Mnq%2Fimage.png?alt=media&#x26;token=87f0210a-f4fe-48b0-9761-7d47b775d192" alt=""><figcaption></figcaption></figure>

&#x20;  5\. Click **Create & View** button.

&#x20;  6\. After successfully creating, copy your API key somewhere safe. For security reasons, do not put it directly in your code, or commit it somewhere public like GitHub.

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FzbbfB3D7iVTB583oI22u%2Fimage.png?alt=media&#x26;token=19109b73-a20e-49f5-8f3c-f28759aa992d" alt=""><figcaption></figcaption></figure>

### How to create an Unsubscribe Group

Allow customers to opt-out of specific types of emails you send.

&#x20;  1\. Login **SendGrid** system

&#x20;  2\. Navigate to **Marketing** on the left navigation bar, and then select **Unsubscribe Group**

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FRsoQOzRN8gtiYfcGLA4P%2Fimage.png?alt=media&#x26;token=cdb1037f-fb11-4872-bb49-7ced793165ee" alt=""><figcaption></figcaption></figure>

&#x20;  3\. Click **Create new Group** button

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FmZpiWRuApy9UYiXPW6RG%2Fimage.png?alt=media&#x26;token=d3049afe-6ba2-4b1b-b65d-03bb8b3944c2" alt=""><figcaption></figcaption></figure>

&#x20;  4\. Fill in the **Group name** and description

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FmkoNvIA7aF78EeOv8Dzi%2Fimage.png?alt=media&#x26;token=c7bbf9e9-8f3f-4e47-9ace-ce90e077a365" alt=""><figcaption></figcaption></figure>

&#x20;  5\. After successfully creating, you must upload or manual add data for **Unsubscribe Group**

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2F3VwrIxApyEzeKnyBxjj7%2Fimage.png?alt=media&#x26;token=969142a8-4269-46eb-93ff-e9d36e92ca23" alt=""><figcaption></figcaption></figure>

&#x20;  6\. Get **Unsubscribe Group Id**

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FRNeDeEyDrzseRWjE1OTr%2Fimage.png?alt=media&#x26;token=a3c1d98c-8b3d-4e66-b98b-0f65403f79d7" alt=""><figcaption></figcaption></figure>

### 5. Save to finish creating the SendGrid destination

### &#x20;

<figure><img src="../../.gitbook/assets/image (3350).png" alt=""><figcaption></figcaption></figure>

### 6. Sending email using SendGrid via Customer Journey

Log into **CDP 365** system. Hover your mouse over **Marketing** and go to **All Channels** menu.

<figure><img src="../../.gitbook/assets/image (3358).png" alt=""><figcaption></figcaption></figure>

We have 2 channels that supporting to send:

* Email
* Orchestration

<figure><img src="../../.gitbook/assets/image (3359).png" alt=""><figcaption></figcaption></figure>

Click **+** button to Create Journey, add **Destination** node and select **SendGrid** destination

<figure><img src="../../.gitbook/assets/image (3360).png" alt=""><figcaption></figcaption></figure>

Select the **SendGrid** destination that you have created before

<figure><img src="../../.gitbook/assets/image (3361).png" alt=""><figcaption></figcaption></figure>

Fill out necessary information

<figure><img src="../../.gitbook/assets/image (3363).png" alt=""><figcaption></figcaption></figure>

* Variant Name: The name of Variant. This field is required.
* Subject: title of Email. This field is required.
* Preheader: overview of email. This field is optional. If there is no value, the default will show the content of the email in the preheader position.&#x20;
* Select email template: Can select from gallery or you template. Hover on template and click Use template to select.

Click the **Save** button to finish setting up journey

<figure><img src="../../.gitbook/assets/image (3364).png" alt=""><figcaption></figcaption></figure>

After finishing the setting of the Journey, we can **activate** and send email to customer.
