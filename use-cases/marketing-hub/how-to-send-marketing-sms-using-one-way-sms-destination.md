# How to send marketing SMS using One Way SMS Destination?

## STEP 1: Create an One Way SMS Destination

### 1. Hover your mouse over Settings, and choose Channel Integration

* Hover your mouse over **Settings** >> Choose **SMS**

<figure><img src="../../.gitbook/assets/image (3579).png" alt=""><figcaption></figcaption></figure>

### 2. Click  ![](<../../.gitbook/assets/image (1435).png>) to create a new Destination

<figure><img src="../../.gitbook/assets/image (3580).png" alt=""><figcaption></figcaption></figure>

### 3. Choose _One Way SMS_ category

<figure><img src="../../.gitbook/assets/image (3598).png" alt=""><figcaption></figcaption></figure>

### 4. Fill the necessary information

<figure><img src="../../.gitbook/assets/image (3582).png" alt=""><figcaption></figcaption></figure>

_**General information**_

* Destination Name: Input the name for the destination.
* Description: Input description for this destination (optional).
* Destination Catalog: Select **My One Way SMS** option.
* Method: Select **Send** (default).

#### _**Configure fields**_

* **User name:** Input the user name of your One Way SMS account.
* **Password**: Input the password to login to your One Way SMS account.
* **Phone number:** Input the phone number you need to send SMS message to.

At this step, users can input phone by phone, or click on <img src="../../.gitbook/assets/image (1600).png" alt="" data-size="line">icon, then select **Add personalization** to use Personalization function. A popup will show up as below:

<figure><img src="../../.gitbook/assets/image (3583).png" alt=""><figcaption></figcaption></figure>

1. **Personalization type**: Select **Customer Attribute** or **Visitor Attribute** depending on the target audience you are desire to send marketing messages.
2. **Personalization Attribute**: Select **Phone**
3. Click **Insert** to save the setting.&#x20;

* **Base URL:** Input the Base URL of your account.

#### General Setting

_**Frequency Capping**_

Frequency Capping settings allows users to limit the times an audiences receiving a marketing message.

<table><thead><tr><th width="262">Option</th><th>Description</th></tr></thead><tbody><tr><td>Ignore duplicate messages for the scheduled journey</td><td>One audience just receive one message in an iteration of journey schedule </td></tr><tr><td>Limit frequency for the journey (3 months duration)</td><td><p>Limit allocation frequency to 1 audience in a journey for 3 months </p><p>(Ex: 2 times/person)</p></td></tr><tr><td>Limit frequency for destination</td><td><p>Limit allocation frequency to 1 audience per unit of time (hour, day, etc.) </p><p>(Ex: 3 times/month, 1 times/day)</p></td></tr></tbody></table>

_**Delivered rate**_

Delivered rate setting allows users to limit the number of messages sent per second for a specific Destination.&#x20;

<table><thead><tr><th width="333">Option</th><th>Description</th></tr></thead><tbody><tr><td>As fast as possible</td><td>The maximum number of marketing messages sent per second will depend on the system possibility.</td></tr><tr><td>Limit send rate {x} time(s) per second</td><td><p>The number of marketing messages sent per second will be set by user. </p><p>(Ex: You are creating a destination for G Suite Email, the value you set is 100. That means only 100 emails will be sent per second.)</p></td></tr></tbody></table>

### 5. Click Save to save the Destination



## STEP 2: Create a Customer Journey

### 1. Hover your mouse over Marketing

* Choose **Orchestration**

<figure><img src="../../.gitbook/assets/image (3584).png" alt=""><figcaption></figcaption></figure>



* Or choose **SMS**

<figure><img src="../../.gitbook/assets/image (3585).png" alt=""><figcaption></figcaption></figure>

### 2. Click + button to create a new Customer Journey.&#x20;

### Then configure the Trigger Node

<figure><img src="../../.gitbook/assets/image (3586).png" alt=""><figcaption></figcaption></figure>

**Journey schedule**

_Trigger Journey_

* Once: The journey will run only 1 time
* By hour/day/week/month: The Journey will run hourly/ daily/ weekly/ monthly

<figure><img src="../../.gitbook/assets/image (3587).png" alt=""><figcaption></figcaption></figure>

_Trigger time -_ The time Journey will start running

<figure><img src="../../.gitbook/assets/image (3588).png" alt=""><figcaption></figcaption></figure>

* At a specific date & time: Choose the date and time the journey will start
* Right after the journey activated: The journey will run after you click **Activate**

**Include/ Exclude Audiences**

* Choose the audiences who are able/not able to go to the Journey
* Click ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe7qtnJ_skUvCFC1zGezn3rThbIYXp7cLtkWJVzou-iO5QnwqkxWRDmKlE8w8HkcJfa7Pwx-JjBeYIwPYo0z2DldLSrkOb5RFd-dlM_qjh-9Kp5YbFAsun9N9kj0Q9o_F3o336cH43AH2evGhb3XpXcBNs?key=jqlrLHcQRq84j2mU-bHqrw)or ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdSeJuse1J544mjbLWR3dnGc1_niyb4hj3Mh4o-Z1HtMn99h3RoEW-8lsakkPFNsxYd5yf23fnOXFssfpNhp1w9RONHQzbOGnssmuNClwcoEMEwXGVJmMUhUC6ibGHhGjuHVa0EpCnTUtdW8M6p5Padxhov?key=jqlrLHcQRq84j2mU-bHqrw) to add audiences

<figure><img src="../../.gitbook/assets/image (3589).png" alt=""><figcaption></figcaption></figure>

**General Settings**

Limit the time an audience would receive a ticket

* Unlimited frequency: The audience will receive as many ticket as the journey run
* Limited frequency: The audience will receive {x} ticket per day/week/month/lifetime

### 3. Add Action node (optional)

<figure><img src="../../.gitbook/assets/image (3590).png" alt=""><figcaption></figcaption></figure>

### 4. Add and configure Destination node

* Click + to add Destination node -> Choose **My One Way SMS**

<figure><img src="../../.gitbook/assets/image (3591).png" alt=""><figcaption></figcaption></figure>

Choose **Design from scratch**

<figure><img src="../../.gitbook/assets/image (3592).png" alt=""><figcaption></figcaption></figure>

Design the campaign:

1. _**Settings**_

<figure><img src="../../.gitbook/assets/image (3593).png" alt=""><figcaption></figcaption></figure>

#### Setting tab:

* Campaign Name: Input the name of this campaign
* Delivery Destination: Select the destination you created in **STEP 1**
* Delivery Algorithm: Randomization (default)
* Delivery Hours of the Day: Select the time of day you want to send this Email.

2. _**Compose**_

<figure><img src="../../.gitbook/assets/image (3599).png" alt=""><figcaption></figcaption></figure>

* **Variant Name:** The name of the message template
* **Content:** The content of the message. You could make your content dynamic by clicking ![](<../../.gitbook/assets/image (933).png>) icon

<figure><img src="../../.gitbook/assets/image (3600).png" alt=""><figcaption></figcaption></figure>

### 5. Save and Activate the Journey

* Click **Save** to save the Journey

<figure><img src="../../.gitbook/assets/image (3601).png" alt=""><figcaption></figcaption></figure>

* Click **Activate** to start running the Journey

<figure><img src="../../.gitbook/assets/image (3602).png" alt=""><figcaption></figcaption></figure>
