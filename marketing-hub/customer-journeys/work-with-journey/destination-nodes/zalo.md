# Zalo

## I - Zalo OA (Zalo Official Account)

### Step 1 - Add the Destination Node & choose Zalo OA catalog

<figure><img src="../../../../.gitbook/assets/Add destination node.gif" alt=""><figcaption></figcaption></figure>

### Step 2 - Choose a template you want to use

{% hint style="info" %}
Only the templates which has been chosen in any of the created destination were displayed here, so if you don't see the template you want, please check the destination.
{% endhint %}

<figure><img src="../../../../.gitbook/assets/image (2917).png" alt=""><figcaption></figcaption></figure>

### Step 3 - Configure the destination node

#### &#x20;1. Choose a destination to send messages.&#x20;

<figure><img src="../../../../.gitbook/assets/image (2918).png" alt=""><figcaption></figcaption></figure>

#### 2. Compose the message content

Depend on the template type you choose, the fields will be displayed accordingly

#### **1️⃣   Text Message**

* Using this template, you could send out text message to your audience. It is useful in some scenarios such as sending welcome/ thank you message for following or purchasing a product/ service, etc.
* Type the content of your message in the Content <mark style="color:red;">\*</mark> field

<figure><img src="../../../../.gitbook/assets/image (2919).png" alt=""><figcaption></figcaption></figure>

#### **2️⃣   Image Message**

This template brings a great way to rapidly catch the attion of your audience by using vivid image. You could insert the image URL or click the button to choose the desired one.

* Image URL <mark style="color:red;">\*</mark> : Enter the link of image or click button ![](../../../../.gitbook/assets/outline_perm_media_black_24dp.png)  to add image
* Content <mark style="color:red;">\*</mark> : The description of the image or any content you want

<figure><img src="../../../../.gitbook/assets/image (2920).png" alt=""><figcaption></figcaption></figure>

#### **3️⃣ Sticker Message**

The targeted Line users will receive a sticker from your Line Official Account . You could only send one sticker at a time.

* Sticket Set <mark style="color:red;">\*</mark>: The name of the sticker package provided by ZALO
* Sticker <mark style="color:red;">\*</mark>: The sticker in the chosen Sticker Set above

<figure><img src="../../../../.gitbook/assets/image (2927).png" alt=""><figcaption></figcaption></figure>

**4️⃣** **Request information**

This type of template allows you to send an image and a text to Zalo users. When the user touches on the template, a built-in form will be opened to collect user information (<img src="https://lh7-us.googleusercontent.com/Q3Wv6pVdYHJTgUiYCUcZFkCtuXFcMlbb_OSv27DU8zA5769mwKz7RnQFjiIRckaeiCra7t4afBYqw7ehBZNjnvnrxUtoh_MFBVjyB2ClSMb9LsCQrUj-N1VDr0DJvqsDLdKQwbd1VUWc6ME3hh4-X1iD3g=s2048" alt="" data-size="line">)

Using this method will assist you in enrich customer data and increase the feasibility of future marketing scenarios.

To create a Request Information message, you need to fill in these fields below:

* Image URL <mark style="color:red;">\*:</mark> Enter the link of image or click button ![](../../../../.gitbook/assets/outline_perm_media_black_24dp.png)  to add image
* Description <mark style="color:red;">\* :</mark> The text element of the template.

<figure><img src="../../../../.gitbook/assets/image (2921).png" alt=""><figcaption></figcaption></figure>

#### **5️⃣ Transaction message**

* For those use cases specified for transaction such as Order/ Service Confirmation, Order/ Service Summary, etc, this type of template is the most suitable choice.&#x20;
* Since it relates to transaction, there are some required information you need to prepare beforehand which are&#x20;
  * The Customer Name
  * The Code to identify the customer in the transaction (eg: Order Code, Booking code, Invoice code, etc)
* Also, you can decide which action will happen when a Zalo user clicks on the buttons in the template
* To configure this template, you need to complete these fields

<table><thead><tr><th width="188">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Message Type <mark style="color:red;">*</mark></td><td>It's the text which will appear in the device's notifications, chat list, and quote messages as an alternative to the template message.</td></tr><tr><td>Banner <mark style="color:red;">*</mark></td><td>The Image which will appear in the slide</td></tr><tr><td>Title <mark style="color:red;">*</mark></td><td>The title of the message template</td></tr><tr><td>Subtitle <mark style="color:red;">*</mark></td><td>The subtitle of the template</td></tr><tr><td>Content Table <mark style="color:red;">*</mark></td><td>The detailed information about the transaction organized by a table. Imagining it like an excel table, the label is the header and the content is its information. Both fields are obligatory.<br><br><strong>NOTE:</strong> <br><strong>-</strong> There will be a Message type row which stands in the second position  by default <br>- The first row of the table must be Customer Name or “…Code…” <br>- There’s maximum of 5 fields to be added in the table (not including Message Type fields) <br>- The label could not be duplicated <br>- Be aware of the character limit on each field if you don’t want to send the messages unsuccessfully.</td></tr><tr><td>Message</td><td>The second text of the template</td></tr><tr><td>Action <mark style="color:red;">*</mark></td><td>Setup the action which will happen when Line users click on a button. See <a href="zalo.md#action-type">here</a></td></tr></tbody></table>

<figure><img src="../../../../.gitbook/assets/2023-12-25_15-00-03.gif" alt=""><figcaption></figcaption></figure>

#### 6️⃣ **Rich Media Message**

This type of message includes many fields that are the same as Transaction Message

<table><thead><tr><th width="188">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Banner <mark style="color:red;">*</mark></td><td>The Image which will appear in the slide</td></tr><tr><td>Title <mark style="color:red;">*</mark></td><td>The title of the message template</td></tr><tr><td>Subtitle <mark style="color:red;">*</mark></td><td>The subtitle of the template</td></tr><tr><td>Content Table <mark style="color:red;">*</mark></td><td>The information organized by a table. Imagining it like an excel table, the label is the header and the content is its information. Both fields are obligatory.<br><br><strong>NOTE:</strong> <br>- There’s maximum of 7 fields to be added in the table<br>- The label could not be duplicated <br>- Be aware of the character limit on each field if you don’t want to send the messages unsuccessfully.</td></tr><tr><td>Message</td><td>The second text of the template</td></tr><tr><td>Action <mark style="color:red;">*</mark></td><td>Setup the action which will happen when Line users click on a button. See <a href="zalo.md#action-type">here</a></td></tr></tbody></table>

After finishing, your message would look like this:

<figure><img src="../../../../.gitbook/assets/2023-12-25_15-02-28.gif" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
This template could only be sent from 06:00 AM to 10:00 PM everyday. To prevent sending message unsuccessfully, make sure you choose the appropriate time range in [Step 1 - Settings.](zalo.md#id-1.-choose-a-destination-to-send-messages)
{% endhint %}

### ACTIONS

When Zalo users interact with the buttons in a template sent from CDP 365, the chosen action will happened.&#x20;

Each block of button includes these fields:

* Icon URL <mark style="color:red;">\*</mark>: The URL of the icon for the button
* Button Label <mark style="color:red;">\*</mark>: The description of the button
* Action Type <mark style="color:red;">\*</mark>: Based on the action you choose, the fields below will vary. See detail [here](zalo.md#action-type)

<figure><img src="../../../../.gitbook/assets/image (2923).png" alt=""><figcaption></figcaption></figure>

#### Action Type

**1️⃣ Message Action**

When an element associated with this action is tapped, a message would be sent from Zalo user to Zalo OA.&#x20;

* Display Mode <mark style="color:red;">\*</mark>: To decide if the message will be shown or hidden in the chat box or not.&#x20;
* Content <mark style="color:red;">\*</mark>: The content of the message to be sent.

<figure><img src="../../../../.gitbook/assets/image (2922).png" alt=""><figcaption></figcaption></figure>

**2️⃣ Open an URL**

When Zalo user clicks on the button, a link which was setup in URL <mark style="color:red;">\*</mark> an CDP 365 will be opened in Zalo's in-app browser.

<figure><img src="../../../../.gitbook/assets/image (2925).png" alt=""><figcaption></figcaption></figure>

**3️⃣** **Open SMS**

When the button associated with this action is tapped, the texting screen of user device will be open with the phone number & message content setup in CDP 365 was filled beforehand.&#x20;

* Phone Number <mark style="color:red;">\*</mark>: The receiver's number
* Content <mark style="color:red;">\*</mark>: The content of the message to be sent

<figure><img src="../../../../.gitbook/assets/image (2926).png" alt=""><figcaption></figcaption></figure>



**4️⃣ Open Phone**

When the button associated with this action is tapped, the calling screen of user device will be open with the Phone Number <mark style="color:red;">\*</mark> setup in CDP 365 was filled beforehand

<figure><img src="../../../../.gitbook/assets/image (2924).png" alt=""><figcaption></figcaption></figure>

❗<mark style="color:red;">**NOTE**</mark> ❗

* With every Landing Page URL you add to the template, if you want to record the number of clicks, you must shorten the link. To do so, please follow these step:
* Click on the ![](../../../../.gitbook/assets/outline_person_black_24dp.png)  icon -> Choose Add Shortlink option (optional, it only displays when it also allows Add Personalization) -> Choose the type of short link you want -> insert the link and click OK

<figure><img src="../../../../.gitbook/assets/2023-12-25_15-34-49.gif" alt=""><figcaption></figcaption></figure>

* To manage the link you have shortened, go to app [Link Management](../../../link-management.md) in Marketing Hub
