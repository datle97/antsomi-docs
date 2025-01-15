# How to send "Infobip Viber" using CDP 365

## STEP 1: Create the 'Infobip Viber' destination&#x20;

### 1. Log in to **CDP 365**. Hover your mouse over **Settings**. Choose **Channel Integration**.

<figure><img src="../../.gitbook/assets/image (3197).png" alt=""><figcaption></figcaption></figure>

### 2. Click the ![](<../../.gitbook/assets/image (896).png>) button and select Viber

<figure><img src="../../.gitbook/assets/image (3198).png" alt=""><figcaption></figcaption></figure>

Select **Infobip Viber** in the **Destination Catalog**

<figure><img src="../../.gitbook/assets/image (3199).png" alt=""><figcaption></figcaption></figure>

### 3. Fill in the necessary information for the destination

#### General Information

* Destination Name
* Description

_NOTE:_ You can add another language if you want by clicking ![](<../../.gitbook/assets/image (3200).png>)

<figure><img src="../../.gitbook/assets/image (3201).png" alt=""><figcaption></figcaption></figure>

#### Configure fields

<figure><img src="../../.gitbook/assets/image (3202).png" alt=""><figcaption></figcaption></figure>

The configuration of the Infobip Viber destination is required these fields:

[API Key](how-to-send-infobip-viber-using-cdp-365.md#api-key)

[Base URL](how-to-send-infobip-viber-using-cdp-365.md#base-url)

[Country Code](how-to-send-infobip-viber-using-cdp-365.md#country-code)

[Phone Number](how-to-send-infobip-viber-using-cdp-365.md#phone-number)

[Sender Name](how-to-send-infobip-viber-using-cdp-365.md#sender-name)

#### API Key

The key is provided by Infobip for your Infobip Viber account.&#x20;

To get the API Key, please follow these steps&#x20;

Step 1: Go to your Infobip account, find the API Keys app at the DEVELOPER TOOLS&#x20;

<figure><img src="../../.gitbook/assets/image (1349).png" alt=""><figcaption><p>API Keys</p></figcaption></figure>

Step 2: Copy the API Key&#x20;

<figure><img src="../../.gitbook/assets/image (2100).png" alt=""><figcaption><p>API Keys</p></figcaption></figure>

Step 3: Paste it to the API Key in the Configure field&#x20;

<figure><img src="../../.gitbook/assets/image (3203).png" alt=""><figcaption></figcaption></figure>

#### Base URL

To get the Base URL, go to your Infobip account

Step 1: Go to the Developers tab, copy the API Base URL

<figure><img src="../../.gitbook/assets/image (468).png" alt=""><figcaption><p>API Base URL</p></figcaption></figure>

Step 2: Paste the Base URL in the Configure fields

_NOTE:_ You have to add "https://" before the API Base URL after pasting it, for example, _https://jdv4xv.api.infobip.com._

<figure><img src="../../.gitbook/assets/image (3204).png" alt=""><figcaption></figcaption></figure>

#### Country Code

Its the country code of the receiver's phone number which can be formatted as 84 for the Vietnam country code.&#x20;

NOTE:&#x20;

* No "+" before the code, for example, +84. If there is +84, the destination is wrong and can not send the message.
* Only one country code for a destination.
* Limit by 255 characters.

#### Phone number

The phone number of receivers that you can use data available in CDP 365 to set the configuration of the receiver.

NOTE:

* Limit by 150 characters.

You click the ![](<../../.gitbook/assets/image (1881).png>) icon to add Personalization.

<figure><img src="../../.gitbook/assets/image (3205).png" alt=""><figcaption></figcaption></figure>

* Personalization type: Visitor/Customer Attribute
* Personalization attribute: List of attributes in Visitor/customer that you selected before
* Default value: The default phone number that will be used if a customer does not have a phone number.

Example: The receiver phone number is the phone number in the Visitor Business Object.\
<mark style="background-color:red;">NOTE: You should add personalization so your receiver's phone number could be dynamic in the journey. If not, the journey could only send Viber messages to the phone number you put in here.</mark>

#### Sender Name

You input the Name that will be shown in the Viber message.

<figure><img src="../../.gitbook/assets/image (3206).png" alt=""><figcaption></figcaption></figure>

#### General Setting

For the general setting, please check [here](https://docs.antsomi.com/cdp-365-user-guide-en/use-cases/marketing-hub/how-to-send-email-using-mailjet-in-cdp-365#general-setting)!

<figure><img src="../../.gitbook/assets/image (3207).png" alt=""><figcaption></figcaption></figure>

## STEP 2: Create a Customer Journey

### 1. Hover your mouse over **Marketing** and go to **All Channels** menu.

<figure><img src="../../.gitbook/assets/image (3208).png" alt=""><figcaption></figcaption></figure>

### 2. Choose a Channel

We have 2 channels that supporting to send Viber:

* Viber
* Orchestration

<figure><img src="../../.gitbook/assets/image (3209).png" alt=""><figcaption></figcaption></figure>

### 3. Click ![](<../../.gitbook/assets/image (2265).png>) to create a Journey

<figure><img src="../../.gitbook/assets/image (3210).png" alt=""><figcaption></figcaption></figure>

### 4. Add and configure _Destination_ node&#x20;

* Click ![](<../../.gitbook/assets/image (3283).png>) to add Destination node, choose **Infobip Viber**

<figure><img src="../../.gitbook/assets/image (3282).png" alt=""><figcaption></figcaption></figure>

* Choose the method to design the Viber message

<figure><img src="../../.gitbook/assets/image (3215).png" alt=""><figcaption></figcaption></figure>

* Select a "Infobip Viber" destination that you have created in [Step 1](how-to-send-infobip-viber-using-cdp-365.md#step-1-create-the-infobip-viber-destination)

<figure><img src="../../.gitbook/assets/image (3216).png" alt=""><figcaption></figcaption></figure>

* Fill out the necessary information

<figure><img src="../../.gitbook/assets/image (3284).png" alt=""><figcaption></figcaption></figure>

_Notes: If you input the Button Title, the Landing Page is required to fill._

### &#x20;5. Save and activate the Journey

* Click **Save** to save the Journey.
* After that, click **Activate** to start running the Journey and sending Viber messages to journey targeted audience.
