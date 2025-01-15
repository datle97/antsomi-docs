# How to send Telegram message in CDP 365?

## STEP 1 - Create Telegram destination

### 1. Log in to **CDP 365**. Hover your mouse over **Settings**. Choose **Channel Integration**.

<figure><img src="../../.gitbook/assets/image (3388).png" alt=""><figcaption></figcaption></figure>

### 2. Click + button and select Telegram

<figure><img src="../../.gitbook/assets/image (3389).png" alt=""><figcaption></figcaption></figure>

### 3. Destination Catalog: Choose Telegram

<figure><img src="../../.gitbook/assets/image (3390).png" alt=""><figcaption></figcaption></figure>

### 4. Fill in the necessary information for the destination

#### General Information

* Destination Name
* Description

_NOTE:_ You can add another language if you want by clicking ![](<../../.gitbook/assets/image (3393).png>)

<figure><img src="../../.gitbook/assets/image (3391).png" alt=""><figcaption></figcaption></figure>

#### Configure fields

<figure><img src="../../.gitbook/assets/image (3394).png" alt=""><figcaption></figcaption></figure>

The configuration of the Telegram destination has required these fields:

* [Access Token](how-to-send-telegram-message-in-cdp-365.md#how-to-get-your-access-token)
* [Customer ID](how-to-send-telegram-message-in-cdp-365.md#customer-id)

#### How to get your 'Access Token'?

* **Step 1**: Navigate to your Telegram account and search the '**BotFather**' account. The Bot **provides your Access Token**.
* **Step 2**: Chat the '**/start**' keyword to start your conversation **getting the Access Token** with the Bot.
* **Step 3**: Chat the '**/newbot**' keyword to create your new bot that has a unique Access Token.
* **Step 4**: **Name** your bot with a **not existing name**.
* **Step 5**: Get your **Access Token**.

<figure><img src="../../.gitbook/assets/image (2639).png" alt=""><figcaption><p>Chat with the BotFather</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (2643).png" alt=""><figcaption><p>Chat with the BotFather</p></figcaption></figure>

#### Customer ID

Customer ID is **the Telegram ID of a user who has chatted with your newly created bot**.

<mark style="background-color:red;">Note: This Customer ID is</mark> <mark style="background-color:red;"></mark><mark style="background-color:red;">**different**</mark> <mark style="background-color:red;"></mark><mark style="background-color:red;">from the Customer ID existing in CDP 365.</mark>&#x20;

#### General Setting

<figure><img src="../../.gitbook/assets/image (3395).png" alt=""><figcaption></figcaption></figure>

_Frequency Capping_

Frequency Capping settings allows users to limit the times an audiences receiving an email

<table><thead><tr><th width="262">Option</th><th>Description</th></tr></thead><tbody><tr><td>Ignore duplicate messages for the scheduled journey</td><td>One audience just receive one email in an iteration of journey schedule </td></tr><tr><td>Limit frequency for the journey (3 months duration)</td><td><p>Limit allocation frequency to 1 audience in a journey for 3 months </p><p>(Ex: 2 times/person)</p></td></tr><tr><td>Limit frequency for destination</td><td><p>Limit allocation frequency to 1 audience per unit of time (hour, day, etc.) </p><p>(Ex: 3 times/month, 1 times/day)</p></td></tr></tbody></table>

_Delivered rate_

Delivered rate setting allows users to limit the number of email sent per second&#x20;

<table><thead><tr><th width="333">Option</th><th>Description</th></tr></thead><tbody><tr><td>As fast as possible</td><td>The maximum number of email sent per second will depend on the system possibility.</td></tr><tr><td>Limit send rate {x} time(s) per second</td><td><p>The number of email sent per second will be set by user. </p><p>(Ex: The value you set is 100. That means only 100 emails will be sent in 1 second)</p></td></tr></tbody></table>

### 4.  Click Save

<figure><img src="../../.gitbook/assets/image (3396).png" alt=""><figcaption></figcaption></figure>

## STEP 2 - Create a Customer Journey

### 1. Log into **CDP 365** system. Hover your mouse over **Marketing** and go to **All Channels** menu.

<figure><img src="../../.gitbook/assets/image (3397).png" alt=""><figcaption></figcaption></figure>

### 2. Choose a Channel

We have 2 channels that supporting to send Telegram messages:

* Telegram
* Orchestration

<figure><img src="../../.gitbook/assets/image (3398).png" alt=""><figcaption></figcaption></figure>

### 3. Click + to create a Journey

<figure><img src="../../.gitbook/assets/image (3399).png" alt=""><figcaption></figcaption></figure>

### 4. Add and configure _Destination_ node&#x20;

* Click ![](<../../.gitbook/assets/image (3401).png>) to add **Destination** node -> Choose **Telegram**

<figure><img src="../../.gitbook/assets/image (3408).png" alt=""><figcaption></figcaption></figure>

* Choose the method to design the message

<figure><img src="../../.gitbook/assets/image (3402).png" alt=""><figcaption></figcaption></figure>

* Select the **Telegram** destination that you have created in [Step 1](how-to-send-telegram-message-in-cdp-365.md#step-1-create-mailjet-destination)

<figure><img src="../../.gitbook/assets/image (3404).png" alt=""><figcaption></figcaption></figure>

* Fill out the necessary information.

<figure><img src="../../.gitbook/assets/image (3405).png" alt=""><figcaption></figcaption></figure>

### 5. Save and activate the Journey

* Click **Save** to save the Journey

<figure><img src="../../.gitbook/assets/image (3406).png" alt=""><figcaption></figcaption></figure>

* Click **Activate** to start running the Journey and sending Telegram messages to customers

<figure><img src="../../.gitbook/assets/image (3407).png" alt=""><figcaption></figcaption></figure>
