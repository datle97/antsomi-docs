# Email

## Antsomi Email

Antsomi email destination includes the following settings:

<figure><img src="../../../.gitbook/assets/image (384).png" alt=""><figcaption></figcaption></figure>

### Configure fields

* _Identity type:_ You are identified by a domain
* _Domain:_ Input your domain or subdomain
* _From Email Address:_ The send's email address
* _From Email Name:_ The sender's name
* _To Addresses:_ The receiver's email address

### **Verifying your domain**

The instruction to verify your domain

### **Advanced DKIM Settings**

There are two ways to verify your domain:&#x20;

* **Easy DKIM**

<figure><img src="../../../.gitbook/assets/image (385).png" alt="" width="375"><figcaption><p><em>Easy DKIM</em></p></figcaption></figure>

When you set up Easy DKIM for a domain identity, Amazon SES automatically adds a 2048-bit DKIM key to every email that you send from that identity.

In the DKIM signing key length field, choose either [RSA\_2048\_BIT or RSA\_1024\_BIT](https://docs.aws.amazon.com/ses/latest/dg/send-email-authentication-dkim.html#send-email-authentication-dkim-1024-2048).

* **Provide DKIM authentication token (BYODKIM)**

<figure><img src="../../../.gitbook/assets/image (387).png" alt="" width="375"><figcaption><p>BYODKIM - Bring your own DKIM</p></figcaption></figure>

_Private key:_ Input the private key of your domain

_Selector name:_ Unique selector that you specified when you created the TXT record in the DNS configuration for your domain.

## Onesignal Email

<figure><img src="../../../.gitbook/assets/Destination - Email - Onesignal.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="253">Field</th><th>Description</th></tr></thead><tbody><tr><td>App ID</td><td>The ID of the app</td></tr><tr><td>App Secret</td><td>Is a code used to unlock the application</td></tr><tr><td>User ID</td><td>ID of user</td></tr><tr><td>Email From Name</td><td>Sender name</td></tr><tr><td>Email From Address</td><td>Sender email</td></tr></tbody></table>

## Sendgrid

<figure><img src="../../../.gitbook/assets/Destination - Email - Sendgrid.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="263">Field</th><th>Description</th></tr></thead><tbody><tr><td>To Email</td><td><ul><li>Email recipients</li></ul><ul><li>Click the <img src="../../../.gitbook/assets/image (1300).png" alt=""> icon to add Personalization</li></ul><p><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FyRBaTMkLooiimsV3VUIA%2Fimage.png?alt=media&#x26;token=85d0ae63-9c53-437b-9bef-982a74151e34" alt="" data-size="original"></p><p><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FcGa7ClhQ3TwLyJSH5Ibu%2Fimage.png?alt=media&#x26;token=2c22b4ec-582e-4b6a-946a-e7124cc75837" alt="" data-size="original"></p><p></p></td></tr><tr><td>CC Email</td><td>Use to send an email to many people at the same time</td></tr><tr><td>API Key</td><td>​<a href="https://app.gitbook.com/o/-LzunofLVjpTa_-p1PQt/s/mECwNqMNUmu6OXHSYgDv/quick-start-guide/how-to-send-email-using-sendgrid-in-cdp-365#how-to-create-api-key-on-sendgrid">API key that you created on SendGrid</a></td></tr><tr><td>From Email Name</td><td>Sender name</td></tr><tr><td>From Email Address</td><td>Email sends to customers</td></tr><tr><td>Unsubscribe Group Id</td><td><a href="https://app.gitbook.com/o/-LzunofLVjpTa_-p1PQt/s/mECwNqMNUmu6OXHSYgDv/quick-start-guide/how-to-send-email-using-sendgrid-in-cdp-365#how-to-create-an-unsubscribe-group">ID of Unsubcribe Group that you create on SendGrid (optional)</a></td></tr></tbody></table>

## G Suite Email

<figure><img src="../../../.gitbook/assets/Destination - Email - G-suit email (1).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="247">Field</th><th>Description</th></tr></thead><tbody><tr><td>Email</td><td>Receiver email</td></tr><tr><td>From Email Name</td><td>Sender name</td></tr><tr><td>Username</td><td>Sender email</td></tr><tr><td>Password</td><td>Sender email pass</td></tr></tbody></table>



## Amazon SES

<figure><img src="../../../.gitbook/assets/Destination - Email - Amazon SES.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="216">Field</th><th>Description</th></tr></thead><tbody><tr><td>Email</td><td><ul><li>Receiver email</li><li>Click the <img src="../../../.gitbook/assets/image (2526).png" alt=""> icon to add Personalization</li></ul><p><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FyRBaTMkLooiimsV3VUIA%2Fimage.png?alt=media&#x26;token=85d0ae63-9c53-437b-9bef-982a74151e34" alt="" data-size="original"></p><p></p><p><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FrN8x5pFXD06amSNkuvwb%2Fimage.png?alt=media&#x26;token=811dabe2-ac8b-4837-8891-88e49600c54f" alt="" data-size="original"></p></td></tr><tr><td>Access Key</td><td>​<a href="https://app.gitbook.com/o/-LzunofLVjpTa_-p1PQt/s/mECwNqMNUmu6OXHSYgDv/quick-start-guide/how-to-send-email-using-amazon-ses-in-cdp-365#get-your-access-key-id-and-secret-access-key">Get your access key ID and secret access key</a></td></tr><tr><td>Secret Key</td><td>​<a href="https://app.gitbook.com/o/-LzunofLVjpTa_-p1PQt/s/mECwNqMNUmu6OXHSYgDv/quick-start-guide/how-to-send-email-using-amazon-ses-in-cdp-365#get-your-access-key-id-and-secret-access-key">Get your access key ID and secret access key</a></td></tr><tr><td>Region</td><td><p>The region where email is verified </p><p><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FfTupBie2WQUOB4pWevvh%2Fimage.png?alt=media&#x26;token=3e58b660-a452-4c81-bb4c-52fc47f1b782" alt="" data-size="original"></p></td></tr><tr><td>From Email Name</td><td>Sender name</td></tr><tr><td>From Email Address</td><td>A regional email address verified with Amazon SES</td></tr></tbody></table>

## Sendinblue

<figure><img src="../../../.gitbook/assets/Destination - Email - Sendinblue.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="260">Field</th><th>Description</th></tr></thead><tbody><tr><td>Email</td><td>Receiver email</td></tr><tr><td>API Key</td><td>API key created on Sendinblue</td></tr><tr><td>From Email Name</td><td>Sender name</td></tr><tr><td>From Email Address</td><td>Email sends to customers</td></tr></tbody></table>

## Infobid

<figure><img src="../../../.gitbook/assets/Destination - Email - Infobid.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="271">Field</th><th>Description</th></tr></thead><tbody><tr><td>Email</td><td>Receiver email</td></tr><tr><td>Base URL</td><td>As a basis for the platform to determine the originator of each API request</td></tr><tr><td>API Key</td><td>API key created on Infobid</td></tr><tr><td>From Email Name</td><td>Sender name email</td></tr><tr><td>From Email Address</td><td>Email sends to customers</td></tr></tbody></table>

## Salesforce Email

<figure><img src="../../../.gitbook/assets/Destination - Email - Salesforce Email.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="264">Field</th><th>Description</th></tr></thead><tbody><tr><td>Email</td><td>Receiver email</td></tr><tr><td>Client ID</td><td>ID of the customer who has registered for the service</td></tr><tr><td>Client Secret</td><td>Is a code used to unlock the application</td></tr><tr><td>Account ID</td><td>ID of the account registered for the service</td></tr><tr><td>Endpoint URL</td><td>A web address (URL) at which customers of a particular service can access it</td></tr><tr><td>Definition Key</td><td>Identifier code</td></tr></tbody></table>

## Amazon SES with Password

<figure><img src="../../../.gitbook/assets/Destination - Email - Amazon SES with Password.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="254">Field</th><th>Description</th></tr></thead><tbody><tr><td>Email</td><td>Receiver email</td></tr><tr><td>From Email Name</td><td>Sender name email</td></tr><tr><td>From Email Address</td><td>Email sends to customers</td></tr><tr><td>Username</td><td><strong>The username of the user</strong></td></tr><tr><td>Password</td><td><strong>The password if LOGIN or PLAIN was used</strong></td></tr></tbody></table>

## Mailchimp

<figure><img src="../../../.gitbook/assets/image (301).png" alt=""><figcaption><p>Mailchimp Email</p></figcaption></figure>



<table><thead><tr><th width="219">Fields</th><th>Description</th></tr></thead><tbody><tr><td>API Key</td><td>The API Key in your Mailchimp account. To know how to take this key, see the instruction below.</td></tr><tr><td>From Email Name</td><td>Sender's name</td></tr><tr><td>From Email Address</td><td>Sender's Email Address</td></tr><tr><td>To Email</td><td>Receiver's Email Address</td></tr></tbody></table>

To connect CDP 365 with Mailchimp, first you have to navigate Mandrillapp and then [verify your sending domains](email.md#verifying-your-domain) and [take an API Key](email.md#get-api-key).

* After logging in your Mailchimp account,open the Account Information --> click Mailchimp Home

<figure><img src="../../../.gitbook/assets/image (2767).png" alt=""><figcaption></figcaption></figure>

* &#x20;Then, open the **Automation menu** and choose **Transactional email** --> Click **Launch App**

<figure><img src="../../../.gitbook/assets/image (311).png" alt=""><figcaption></figcaption></figure>

### Verify your sending domains

* Open Sending Domains menu&#x20;

<figure><img src="../../../.gitbook/assets/image (312).png" alt=""><figcaption></figcaption></figure>

* Add a domain

<figure><img src="../../../.gitbook/assets/image (2728).png" alt=""><figcaption></figcaption></figure>

* Add domain information

The added domain must satisfy the 3 conditions:

1. **Verified Domain**

If your domain is valid, it will already by verified. If not, click View details and follow the instructions.

<figure><img src="../../../.gitbook/assets/image (2730).png" alt=""><figcaption></figcaption></figure>

2. **DKIM Settings**

Click on **View DKIM Settings** and add the provided DKIM in your web hosting DNS Zone.

<figure><img src="../../../.gitbook/assets/image (2732).png" alt=""><figcaption></figcaption></figure>

3. **SPF Settings**: If no problem arise, your DKIM Settings is automatically valid

<figure><img src="../../../.gitbook/assets/image (2734).png" alt=""><figcaption></figcaption></figure>

* **Verify your domain:**

After validating all the information, click Verify a Domain to finally verify your domain

<figure><img src="../../../.gitbook/assets/image (2733).png" alt=""><figcaption></figcaption></figure>

### Get API Key

To authenticate your account, copy and paste the API Key to API Key field in the destination. To do so, follow these steps:

#### Step 1 - Locate API Keys menu

Open SMTP & API Info menu and click <img src="../../../.gitbook/assets/image (314).png" alt="" data-size="line">

<figure><img src="../../../.gitbook/assets/image (313).png" alt=""><figcaption></figcaption></figure>

#### STEP 2 - Create a new API Key

* Enter the description and then click <img src="../../../.gitbook/assets/image (316).png" alt="" data-size="line">

<figure><img src="../../../.gitbook/assets/image (315).png" alt=""><figcaption></figcaption></figure>

* Copy the API Key and paste to CDP 365

<figure><img src="../../../.gitbook/assets/image (317).png" alt=""><figcaption></figcaption></figure>
