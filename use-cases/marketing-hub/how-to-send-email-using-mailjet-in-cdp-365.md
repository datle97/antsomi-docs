# How to send email using "Mailjet" in CDP 365?

## STEP 1 - Create "Mailjet" destination

### 1. Access the "MARKETING HUB" app and go to the "Destinations" menu

<figure><img src="../../.gitbook/assets/image (1657).png" alt=""><figcaption><p>CDP 365 menu</p></figcaption></figure>

### 2. Click ![](<../../.gitbook/assets/image (896).png>) button and select "Email"

<figure><img src="../../.gitbook/assets/image (656).png" alt=""><figcaption><p>Destination list</p></figcaption></figure>

### 3. Fill in the necessary information for the destination

#### General Information

* Destination Name
* Description
* Destination Catalog: Choose _Mailjet Email_

_NOTE:_ You can add another language if you want by clicking ![](<../../.gitbook/assets/image (911).png>)

<figure><img src="../../.gitbook/assets/Mailjet.png" alt=""><figcaption><p>Destination Catalog</p></figcaption></figure>

#### Configure fields

<figure><img src="../../.gitbook/assets/Configure fields.png" alt=""><figcaption><p>Configure fields</p></figcaption></figure>

<table><thead><tr><th width="140.33333333333331">Fields</th><th width="259">Description</th><th>NOTE</th></tr></thead><tbody><tr><td>API Key</td><td>The key provided by Mailjet for your Mailjet account. </td><td>To know your API Key, follow the instructions <a href="how-to-send-email-using-mailjet-in-cdp-365.md#how-to-know-your-api-key-and-secret-key">here</a>.</td></tr><tr><td>Secret Key</td><td>The key generated by Mailjet. </td><td>To know your Secret Key, follow the instructions <a href="how-to-send-email-using-mailjet-in-cdp-365.md#how-to-know-your-api-key-and-secret-key">here</a>.</td></tr><tr><td>From Email Name</td><td>Sender Name</td><td>Required field</td></tr><tr><td>From Email Address</td><td>A regional email address that you verified with Mailjet.</td><td>Required field</td></tr><tr><td>Email</td><td>Receiver's email</td><td><p>You can click <img src="../../.gitbook/assets/image (1881).png" alt=""> icon to add Personalization.</p><p></p><p><img src="../../.gitbook/assets/image (929).png" alt=""><br>It uses data available in CDP 365 to set the receivers configuration.</p><ul><li>Personalization type: Visitor/Customer Attribute</li><li>Personalization attribute: List of attributes in Visitor/customer that you selected before</li><li>Default value: The default email address that will be used if a customer does not have an email</li></ul><p>→ Example: Receiver email addresses are the email addresses in the BO Customer.<br><br><mark style="background-color:red;">NOTE: You should add personalization so your receiver's email could be dynamic in the journey. If not, the journey could only send email to the address you put in here.</mark><br>--> Example: <br>Destination --> Email: abc@gmail.com<br>Journey's audience: Customer segment<br>When the journey run, email will be sent to abc@gmail.com only </p></td></tr></tbody></table>

#### How to know your API Key and Secret Key?

1. In Mailjet, open Account Settings at: [https://app.mailjet.com/account](https://app.mailjet.com/account)
2. Choose REST API section
3. Choose _Show icon_ - ![](<../../.gitbook/assets/image (2520).png>)to see the information.&#x20;
4. Copy the keys and paste to the fields in CDP 365

_NOTE_:

* Secret Key: If you have not had it yet, click _Generate_ to create one. This key is only displayed once, so you should take it at that time. (If not, you must choose _Reset_ to have another key)

#### General Setting

<figure><img src="../../.gitbook/assets/info (1).png" alt=""><figcaption><p>General Setting</p></figcaption></figure>

_Frequency Capping_

Frequency Capping settings allows users to limit the times an audiences receiving an email

<table><thead><tr><th width="262">Option</th><th>Description</th></tr></thead><tbody><tr><td>Ignore duplicate messages for the scheduled journey</td><td>One audience just receive one email in an iteration of journey schedule </td></tr><tr><td>Limit frequency for the journey (3 months duration)</td><td><p>Limit allocation frequency to 1 audience in a journey for 3 months </p><p>(Ex: 2 times/person)</p></td></tr><tr><td>Limit frequency for destination</td><td><p>Limit allocation frequency to 1 audience per unit of time (hour, day, etc.) </p><p>(Ex: 3 times/month, 1 times/day)</p></td></tr></tbody></table>

_Delivered rate_

Delivered rate setting allows users to limit the number of email sent per second&#x20;

<table><thead><tr><th width="333">Option</th><th>Description</th></tr></thead><tbody><tr><td>As fast as possible</td><td>The maximum number of email sent per second will depend on the system possibility.</td></tr><tr><td>Limit send rate {x} time(s) per second</td><td><p>The number of email sent per second will be set by user. </p><p>(Ex: The value you set is 100. That means only 100 emails will be sent in 1 second)</p></td></tr></tbody></table>

### 4.  Click "Save"

<figure><img src="../../.gitbook/assets/image (2280).png" alt=""><figcaption></figcaption></figure>



## STEP 2 - Create a Customer Journey

### 1.  Access the "MARKETING HUB" app and go to the "Customer Journeys" menu

<figure><img src="../../.gitbook/assets/image (1156).png" alt=""><figcaption><p>CDP 365 menu</p></figcaption></figure>

### 2. Choose a Channel

We have 2 channels that supporting to send email:

* Email
* Journey Orchestration

<figure><img src="../../.gitbook/assets/image (1956).png" alt=""><figcaption></figcaption></figure>

### 3. Click ![](<../../.gitbook/assets/image (2265).png>) to create a Journey

<figure><img src="../../.gitbook/assets/image (1879).png" alt=""><figcaption></figcaption></figure>

### 4. Add and configure _Destination_ node&#x20;

* Click ![](<../../.gitbook/assets/image (2113).png>) to add Destination node --> Choose Mailjet Email

<figure><img src="../../.gitbook/assets/Destination node.png" alt=""><figcaption><p>Destination node</p></figcaption></figure>

* Choose the method to design the email

<figure><img src="../../.gitbook/assets/Email Template.png" alt=""><figcaption></figcaption></figure>

* Select a "Mailjet" destination that you have created in [Step 1](how-to-send-email-using-mailjet-in-cdp-365.md#step-1-create-mailjet-destination)

<figure><img src="../../.gitbook/assets/Delivery destination.png" alt=""><figcaption><p>Delivery Destination</p></figcaption></figure>

* Fill out necessary information

<figure><img src="../../.gitbook/assets/info.png" alt=""><figcaption></figcaption></figure>

### 5. Save and activate the Journey

* Click "Save change" to save the Journey

<figure><img src="../../.gitbook/assets/image (2432).png" alt=""><figcaption></figcaption></figure>

* Click "Activate" to start running the Journey and sending email to customers

<figure><img src="../../.gitbook/assets/image (809).png" alt=""><figcaption></figcaption></figure>
