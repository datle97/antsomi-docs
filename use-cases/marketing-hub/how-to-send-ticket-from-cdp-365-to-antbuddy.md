# How to send Ticket from CDP 365 to Antbuddy?

## STEP 1: Create Antbuddy destination

### 1. Open Channel Integration

* Log in to **CDP 365**. Hover your mouse over **Settings**. Choose **Channel Integration**.

<figure><img src="../../.gitbook/assets/image (3412).png" alt=""><figcaption></figcaption></figure>

### 2. Click  ![](<../../.gitbook/assets/image (1435).png>) to create a new Destination. Choose Webhook.

<figure><img src="../../.gitbook/assets/image (3413).png" alt=""><figcaption></figcaption></figure>

### 3. Choose Antbuddy

<figure><img src="../../.gitbook/assets/image (3414).png" alt=""><figcaption></figcaption></figure>

### 4. Fill the necessary information

<figure><img src="../../.gitbook/assets/image (3415).png" alt=""><figcaption></figcaption></figure>

_**General information**_

* Destination Name
* Description
* Method: Choose Send Ticket

_**Configure fields**_

* Webhook Url: The Webhook Listener link in your account on Antbuddy. To get the URL, do as follow:

1. Open Webhook setting on Antbuddy&#x20;

<figure><img src="../../.gitbook/assets/image (1356).png" alt=""><figcaption></figcaption></figure>

2. Copy the URL -> Paste to Webhook URL field in CDP 365

If you haven't had the URL, click ![](<../../.gitbook/assets/image (1504).png>)

<figure><img src="../../.gitbook/assets/image (2305).png" alt=""><figcaption></figcaption></figure>

* Sender User: Email address of sender&#x20;

_**General Setting**_

_Frequency Capping_

Frequency Capping settings allows users to limit the times an audiences receiving a marketing message.

<table><thead><tr><th width="262">Option</th><th>Description</th></tr></thead><tbody><tr><td>Ignore duplicate messages for the scheduled journey</td><td>One audience just receive one message in an iteration of journey schedule </td></tr><tr><td>Limit frequency for the journey (3 months duration)</td><td><p>Limit allocation frequency to 1 audience in a journey for 3 months </p><p>(Ex: 2 times/person)</p></td></tr><tr><td>Limit frequency for destination</td><td><p>Limit allocation frequency to 1 audience per unit of time (hour, day, etc.) </p><p>(Ex: 3 times/month, 1 times/day)</p></td></tr></tbody></table>

_Delivered rate_

Delivered rate setting allows users to limit the number of messages sent per second for a specific Destination.&#x20;

<table><thead><tr><th width="333">Option</th><th>Description</th></tr></thead><tbody><tr><td>As fast as possible</td><td>The maximum number of marketing messages sent per second will depend on the system possibility.</td></tr><tr><td>Limit send rate {x} time(s) per second</td><td><p>The number of marketing messages sent per second will be set by user. </p><p>(Ex: You are creating a destination for G Suite Email, the value you set is 100. That means only 100 emails will be sent in 1 second)</p></td></tr></tbody></table>

### 5. Click Save to save the Destination

<figure><img src="../../.gitbook/assets/image (3416).png" alt=""><figcaption></figcaption></figure>

## STEP 2: Create a Customer Journey

### 1. Log into **CDP 365** system. Hover your mouse over **Marketing** and go to **All Channels** menu.

<figure><img src="../../.gitbook/assets/image (3417).png" alt=""><figcaption></figcaption></figure>

### 2. Choose Orchestration

<figure><img src="../../.gitbook/assets/image (3418).png" alt=""><figcaption></figcaption></figure>

### 3. Click  ![](<../../.gitbook/assets/image (1435).png>) to create a new Customer Journey

<figure><img src="../../.gitbook/assets/image (3419).png" alt=""><figcaption></figcaption></figure>

### 4. Configure the Trigger node

* The type of trigger node for **Webhook** is always **Scheduled trigger**

<figure><img src="../../.gitbook/assets/image (3420).png" alt=""><figcaption></figcaption></figure>

**Journey schedule**

_Trigger Journey_

* Once: The journey will run only 1 time
* By hour/day/week/month: The Journey will run hourly/ daily/ weekly/ monthly

<figure><img src="../../.gitbook/assets/image (3421).png" alt=""><figcaption></figcaption></figure>

_Trigger time -_ The time Journey will start running

<figure><img src="../../.gitbook/assets/image (3422).png" alt=""><figcaption></figcaption></figure>

* At a specific date & time: Choose the date and time the journey will start
* Right after the journey activated: The journey will run after you click Activate

**Include/ Exclude Audiences**

* Choose the audiences who are able/not able to go to the Journey
* Click ![](<../../.gitbook/assets/image (3425).png>)or <img src="../../.gitbook/assets/image (3426).png" alt="" data-size="original"> to add audiences.

<figure><img src="../../.gitbook/assets/image (3428).png" alt=""><figcaption></figcaption></figure>

**General Settings**

Limit the time an audience would receive a ticket

* Unlimited frequency: The audience will receive as many ticket as the journey run
* Limited frequency: The audience will receive {x} ticket per day/week/month/lifetime

### 5. Add and configure Destination node

* Click ![](<../../.gitbook/assets/image (3430).png>) to add Destination node -> Choose **Antbuddy**

<figure><img src="../../.gitbook/assets/image (3411).png" alt=""><figcaption></figcaption></figure>

* Choose **Design from scratch**

<figure><img src="../../.gitbook/assets/image (3432).png" alt=""><figcaption></figcaption></figure>

* Design the campaign:

1. Settings

<figure><img src="../../.gitbook/assets/image (3433).png" alt=""><figcaption></figcaption></figure>

* Campaign Name
* Delivery Destination: Choose the destination you created in STEP 1
* Delivery Algorithm
* Delivery Hours of the Day: Choose the time you want to send the Ticket to Antbudy

2. Compose

<figure><img src="../../.gitbook/assets/image (3434).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (3435).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="223">Field</th><th>Description</th></tr></thead><tbody><tr><td>Variant Name</td><td>The name of the Ticket you will send</td></tr><tr><td>Contact Type</td><td>BO Customer or BO Lead</td></tr><tr><td>Title</td><td>The title of the ticket</td></tr><tr><td>Content</td><td>The content of the Ticket</td></tr><tr><td>Email</td><td>The email of customers</td></tr><tr><td>Phone Number</td><td>The phone number of customers</td></tr><tr><td>Group Name</td><td>Choose the group of ticket</td></tr><tr><td>SLA Name</td><td>SLA (Service-level Agreement) of the ticket</td></tr><tr><td>Channel</td><td>The channel that you will reply ticket from client</td></tr><tr><td>Tag Name</td><td>Choose the tag of Ticket</td></tr></tbody></table>

### 6. Save and Activate the Journey

* Click **Save** to save the Journey

<figure><img src="../../.gitbook/assets/image (3436).png" alt=""><figcaption></figcaption></figure>

* Click **Activate** to start running the Journey

<figure><img src="../../.gitbook/assets/image (3437).png" alt=""><figcaption></figcaption></figure>
