# How to send "eSMS Viber" using CDP 365

## STEP 1: Create the eSMS Viber destination

### 1. Log in to **CDP 365**. Hover your mouse over **Settings**. Choose **Channel Integration**.

<figure><img src="../../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

### 2. Click the ![](<../../.gitbook/assets/image (896).png>) button and select Viber

<figure><img src="../../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

Choose destination catalog: **eSMS Viber**

<figure><img src="../../.gitbook/assets/image (3647).png" alt=""><figcaption></figcaption></figure>

### 3. Fill in the necessary information for the destination

#### General Information

* Destination Name
* Description

_NOTE:_ You can add another language if you want by clicking ![](<../../.gitbook/assets/image (911).png>)

#### Configure fields

<figure><img src="../../.gitbook/assets/image (3634).png" alt=""><figcaption></figcaption></figure>

The configuration of the **eSMS Viber** destination is required these fields:

**API Key**, **Secret Key**, and **Brand Name** are the information that you registered with Vihat. So please go to your Vihat account to get the information.

**Country Code**

Its the country code of the receiver's phone number which can be formatted 84 for the Vietnam country code.&#x20;

_**Note:**_&#x20;

* No "+" before the code, for example, +84. If there is +84, the destination is wrong, and can not send the message.
* Only one country code for a destination.
* Limit by 255 characters.

**Phone Number**

The phone number of receivers that you can use data available in CDP 365 to set the configuration of the receiver.

_**Note:**_

* Limit by 150 characters.

You click the ![](<../../.gitbook/assets/image (1881).png>) icon to add Personalization.

<figure><img src="../../.gitbook/assets/image (3632).png" alt=""><figcaption></figcaption></figure>

* **Personalization type**: Visitor/Customer Attribute
* **Personalization attribute**: List of attributes in Visitor/customer that you selected before
* **Default value**: The default phone number that will be used if a customer does not have a phone number.

_Example_: The receiver phone number is the phone number in the Visitor Business Object.\
&#xNAN;_<mark style="background-color:red;">**Note**</mark>_<mark style="background-color:red;">: You should add personalization so your receiver's phone number could be dynamic in the journey. If not, the journey could only send Viber messages to the phone number you put in here.</mark>

#### General Setting

For the general setting, please check [here](https://docs.antsomi.com/cdp-365-user-guide-en/use-cases/marketing-hub/how-to-send-email-using-mailjet-in-cdp-365#general-setting)!

<figure><img src="../../.gitbook/assets/image (3635).png" alt=""><figcaption></figcaption></figure>

## STEP 2: Create a Customer Journey

### 1.  Hover your mouse over MARKETING to see all the available channels

<figure><img src="../../.gitbook/assets/image (3636).png" alt=""><figcaption></figcaption></figure>

### 2. Choose a Channel

We have 2 channels that supporting to send Viber:

* Viber
* Journey Orchestration

<figure><img src="../../.gitbook/assets/image (3637).png" alt=""><figcaption></figcaption></figure>

### 3. Click ![](<../../.gitbook/assets/image (2265).png>) to create a Journey

<figure><img src="../../.gitbook/assets/image (3638).png" alt=""><figcaption></figcaption></figure>

In this example, let's choose Orchestration journey.

<figure><img src="../../.gitbook/assets/image (3639).png" alt=""><figcaption></figcaption></figure>

### 4. Add and configure the _Destination_ node

* Click ![](<../../.gitbook/assets/image (3641).png>) to add Destination node, choose **eSMS Viber**

<figure><img src="../../.gitbook/assets/image (3640).png" alt=""><figcaption></figcaption></figure>

* Choose the method to design the Viber message

<figure><img src="../../.gitbook/assets/image (3643).png" alt=""><figcaption></figcaption></figure>

* Select the **eSMS Viber** destination that you have created in [Step 1](how-to-send-esms-viber-using-cdp-365.md#step-1-create-the-esms-viber-destination) and fill out the necessary information

<figure><img src="../../.gitbook/assets/image (3644).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (3645).png" alt=""><figcaption></figcaption></figure>

### 5. Save and activate the Journey

* Click **Save** to save the Journey.
* Then click **Activate** to start running the Journey and sending Viber messages to journey targeted audience.

<figure><img src="../../.gitbook/assets/image (3646).png" alt=""><figcaption></figcaption></figure>
