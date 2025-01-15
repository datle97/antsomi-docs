# How to send WhatsApp message in CDP 365?

## STEP 1 - Create WhatsApp destination

### 1. Log in to **CDP 365**. Hover your mouse over **Settings**. Choose **Channel Integration**.

<figure><img src="../../.gitbook/assets/image (3365).png" alt=""><figcaption></figcaption></figure>

### 2. Click + button and select WhatsApp

<figure><img src="../../.gitbook/assets/image (3366).png" alt=""><figcaption></figcaption></figure>

### 3. Choose the Destination Catalog: Antsomi WhatsApp.&#x20;

<figure><img src="../../.gitbook/assets/image (3367).png" alt=""><figcaption></figcaption></figure>

### 4. Then fill in the necessary information for the destination

#### General Information

* Destination Name
* Description

<figure><img src="../../.gitbook/assets/image (3368).png" alt=""><figcaption></figcaption></figure>

_NOTE:_ You can add another language if you want by clicking ![](<../../.gitbook/assets/image (3369).png>)

* Method:&#x20;

The **WhatsApp** destination offers two available methods for you to choose from, each governed by specific settings that determine the content you can send via this destination.

1. **Send Text Message**: In CDP 365, you can configure the content of your WhatsApp message, limited to text-only format.
2. **Send Templates Message**: Alternatively, you can input your customized WhatsApp template into CDP 365, allowing for more structured and predefined message formats.

<figure><img src="../../.gitbook/assets/image (3370).png" alt=""><figcaption></figcaption></figure>

#### Configure fields

<figure><img src="../../.gitbook/assets/image (3372).png" alt=""><figcaption></figcaption></figure>

The configuration of the WhatsApp destination has required these fields:

* [Access Token](how-to-send-whatsapp-message-in-cdp-365.md#how-to-get-your-access-token)
* [Phone Number ID](how-to-send-whatsapp-message-in-cdp-365.md#phone-number-id)
* [Country Code](how-to-send-whatsapp-message-in-cdp-365.md#country-code)
* [Phone Number](how-to-send-whatsapp-message-in-cdp-365.md#phone-number)

#### How to get your Access Token?

To obtain the access token, please navigate to the **Meta for Developers** and API section and follow the appropriate steps outlined in the provided documentation.

<figure><img src="../../.gitbook/assets/image (1642).png" alt=""><figcaption><p>Access Token</p></figcaption></figure>

_Note: The 'Access token' has a validity period of 24 hours. If you wish to make it permanent, please refer to_ [_the provided document_](https://developers.facebook.com/blog/post/2022/12/05/auth-tokens/) _for instructions and guidelines on how to achieve this._

#### Phone Number ID

Phone Number ID is the **phone number of the sender**.

To obtain the access token, please navigate to the Meta for Developers and API section and follow the appropriate steps outlined in the provided documentation.

<figure><img src="../../.gitbook/assets/image (1500).png" alt=""><figcaption><p>Phone Number ID</p></figcaption></figure>

#### Country Code

Its the country code of the receiver's phone number which can be formatted 84 for the Vietnam country code.&#x20;

NOTE:&#x20;

* No "+" before the code, for example, +84. If there is +84, the destination is wrong and can not send the message.
* Only one country code for a destination.
* Limit by 255 characters.

#### Phone Number

The **phone number of receivers** that you can use data available in CDP 365 to set the configuration of the receiver.

NOTE:

* Limit by 150 characters.

You click the ![](<../../.gitbook/assets/image (1881).png>) icon to add Personalization.

<figure><img src="../../.gitbook/assets/image (3373).png" alt=""><figcaption></figcaption></figure>

* Personalization type: Visitor/Customer Attribute
* Personalization attribute: List of attributes in Visitor/customer that you selected before
* Default value: The default phone number that will be used if a customer does not have a phone number.

Example: The receiver phone number is the phone number in the Visitor Business Object.\
<mark style="background-color:red;">NOTE: You should add personalization so your receiver's phone number could be dynamic in the journey. If not, the journey could only send Whatsapp</mark>

&#x20;<mark style="background-color:red;">messages to the phone number you put in here.</mark>

#### General Setting

<figure><img src="../../.gitbook/assets/image (3374).png" alt=""><figcaption></figcaption></figure>

_Frequency Capping_

Frequency Capping settings allows users to limit the times an audiences receiving an email

<table><thead><tr><th width="262">Option</th><th>Description</th></tr></thead><tbody><tr><td>Ignore duplicate messages for the scheduled journey</td><td>One audience just receive one email in an iteration of journey schedule </td></tr><tr><td>Limit frequency for the journey (3 months duration)</td><td><p>Limit allocation frequency to 1 audience in a journey for 3 months </p><p>(Ex: 2 times/person)</p></td></tr><tr><td>Limit frequency for destination</td><td><p>Limit allocation frequency to 1 audience per unit of time (hour, day, etc.) </p><p>(Ex: 3 times/month, 1 times/day)</p></td></tr></tbody></table>

_Delivered rate_

Delivered rate setting allows users to limit the number of email sent per second&#x20;

<table><thead><tr><th width="333">Option</th><th>Description</th></tr></thead><tbody><tr><td>As fast as possible</td><td>The maximum number of email sent per second will depend on the system possibility.</td></tr><tr><td>Limit send rate {x} time(s) per second</td><td><p>The number of email sent per second will be set by user. </p><p>(Ex: The value you set is 100. That means only 100 emails will be sent in 1 second)</p></td></tr></tbody></table>

### 5.  Click Save

<figure><img src="../../.gitbook/assets/image (3375).png" alt=""><figcaption></figcaption></figure>

## STEP 2 - Create a Customer Journey

### 1.  Log into **CDP 365** system. Hover your mouse over **Marketing** and go to **All Channels** menu.

<figure><img src="../../.gitbook/assets/image (3376).png" alt=""><figcaption></figcaption></figure>

### 2. Choose a Channel

We have 2 channels that supporting to send WhatsApp messages:

* WhatsApp
* Orchestration

<figure><img src="../../.gitbook/assets/image (3377).png" alt=""><figcaption></figcaption></figure>

### 3. Click + button to create a Journey

<figure><img src="../../.gitbook/assets/image (3378).png" alt=""><figcaption></figcaption></figure>

### 4. Add and configure _Destination_ node&#x20;

Add **Destination** node -> Choose **Antsomi WhatsApp**

<figure><img src="../../.gitbook/assets/image (3387).png" alt=""><figcaption></figcaption></figure>

Choose the method to design the message

<figure><img src="../../.gitbook/assets/image (3380).png" alt=""><figcaption></figcaption></figure>

* Select the WhatsApp destination that you have created in [Step 1](how-to-send-whatsapp-message-in-cdp-365.md#step-1-create-mailjet-destination)

<figure><img src="../../.gitbook/assets/image (3381).png" alt=""><figcaption></figcaption></figure>

* Fill out necessary information

<figure><img src="../../.gitbook/assets/image (1203).png" alt=""><figcaption></figcaption></figure>

_Note: The setting mentioned in Step 2 is dependent on the specific Method you selected during the creation of this destination. The method you choose will determine the configuration and options available for the setting in question._

* If the Method is **Send Text Message**

<figure><img src="../../.gitbook/assets/image (3383).png" alt=""><figcaption></figcaption></figure>

* If the Method is **Send Templates Message**

<figure><img src="../../.gitbook/assets/image (3384).png" alt=""><figcaption></figcaption></figure>

### 5. Save and activate the Journey

* Click **Save** to save the Journey

<figure><img src="../../.gitbook/assets/image (3385).png" alt=""><figcaption></figcaption></figure>

* Click **Activate** to start running the Journey and sending WhatsApp message to customers

<figure><img src="../../.gitbook/assets/image (3386).png" alt=""><figcaption></figcaption></figure>
