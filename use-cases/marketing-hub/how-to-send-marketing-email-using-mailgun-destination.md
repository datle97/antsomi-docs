# How to send marketing email using Mailgun Destination?

## STEP 1: Create a Mailgun Destination

### 1. Open Destination app

* Hover your mouse over **Settings**. Open **Email** in **Channel Integration**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXePG4m-j3RbuK8XU6Ktx9dbHK-URy8VUflYNBVidR9VrUuXi6Ouh5fTF4ix9nmtIqr96Ty4fVb0sMlolWduxKjOQOXWPeC7c43QbfeLrSkR8h2G_7KrzG9t-1teX55Smw5g7WzxrGrw-rBFoSjpoVaM1Efi?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### 2. Click  ![](<../../.gitbook/assets/image (1435).png>) to create a new Destination

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfgavWyvN5wVmwCAVLn1Mh6swMDehUiBpN4cvAVfP2tOKgam1egj0Hjjk8YIOEfA31qWGwSodFbvAg_n5ImOmZi1j5F0ORIMRKImd7LO9oi0z8w512lkcZIb_33f9UoL-aWEhOihgy2fMpLQKE08oHo8AMT?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### 3. Choose Catalog: Mailgun

<figure><img src="../../.gitbook/assets/2024-09-09_16-34-46.png" alt=""><figcaption></figcaption></figure>

### 4. Fill the necessary information

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfgsJ7nAsFMJkveHAcjfQk4l6resBi-WzQOBjOTJ4N6AJMso9ngeahxP3ScKqfBcc97xwKYrCeLaqly3GuCSpFre4JHGhWS3jlvlaMNTogyoVAFIAEwENAlrzKY-622gXe0KJjjSs9PjlS_yB2JQt4BoWUo?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

_**General information**_

* Destination Name: Input the name for the destination.
* Description: Input description for this destination (optional).
* Destination Catalog: Select **Mailgun Email** option.
* Method: Select **Send** (default).

#### _**Configure fields**_

* **API key:** To get this API key, follow these steps:

1. Log in to your **Mailgun** account, then select **Sending >> Overview >> Select**
2. Copy the API key as highlighted in below image

<figure><img src="../../.gitbook/assets/image (2541).png" alt=""><figcaption><p>Get API key</p></figcaption></figure>

* **Domain**: To get this item, follow these steps:

1. Log in to your Mailgun account, then select **Sending >> Domains**
2. Copy domain URL as highlighted in below image:

<figure><img src="../../.gitbook/assets/image (1121).png" alt=""><figcaption><p>Get Domain</p></figcaption></figure>

* **From email address**: Input the email used to send marketing message
* **Email:** Input the email you need to send marketing email to.

At this step, users can input email by email, or click on <img src="../../.gitbook/assets/image (1600).png" alt="" data-size="line">icon to use Personalization function. By clicking on that icon, a popup will be show up as below:

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfL3XFWJUQSWRukRCUSCCU5wO3rPJnpCQUVyL9GE8U_VCYnyW_lWIIiAnSOBuMiP4J_kQneQydO5fnMGa9tNnLhSoVMFnFqBgpPmb15qT0n5-uk4xHQX1vlm74ooioOJcbEnFTxBRDsF06-7_vl2l2hbH7a?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

* **Personalization type**: Select **Customer Attribute** or **Visitor Attribute** depending on the target audience you are desire to send marketing messages.
* **Personalization Attribute**: Select **Email**
* Click **Insert** to save the setting. The result can be found as below:

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdvPvitRLhAExqoTFuH-EWJwCZjdCcVNGk4EXTzQF7VjE2rMW4bEd4wLaw4jB4Y8JQNderHekm3NiB591bOpwVc_mB2GIUgCktsByYK_lU1R0vqNRD5nJ7WhKoStO3Pzh5ZogL3oA3eraVt_6qfi2vkonFl?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

#### General Setting

_**Frequency Capping**_

Frequency Capping settings allows users to limit the times an audiences receiving a marketing message.

<table><thead><tr><th width="262">Option</th><th>Description</th></tr></thead><tbody><tr><td>Ignore duplicate messages for the scheduled journey</td><td>One audience just receive one message in an iteration of journey schedule </td></tr><tr><td>Limit frequency for the journey (3 months duration)</td><td><p>Limit allocation frequency to 1 audience in a journey for 3 months </p><p>(Ex: 2 times/person)</p></td></tr><tr><td>Limit frequency for destination</td><td><p>Limit allocation frequency to 1 audience per unit of time (hour, day, etc.) </p><p>(Ex: 3 times/month, 1 times/day)</p></td></tr></tbody></table>

_**Delivered rate**_

Delivered rate setting allows users to limit the number of messages sent per second for a specific Destination.&#x20;

<table><thead><tr><th width="333">Option</th><th>Description</th></tr></thead><tbody><tr><td>As fast as possible</td><td>The maximum number of marketing messages sent per second will depend on the system possibility.</td></tr><tr><td>Limit send rate {x} time(s) per second</td><td><p>The number of marketing messages sent per second will be set by user. </p><p>(Ex: You are creating a destination for G Suite Email, the value you set is 100. That means only 100 emails will be sent per second.)</p></td></tr></tbody></table>

### 5. Click ![](<../../.gitbook/assets/image (1172).png>) to save the Destination



## STEP 2: Create a Customer Journey

### 1. Open Customer Journeys app

* Hover your mouse over **Marketing** -> Choose Channel **Email** or **Orchestration**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXebBPN5fnXUwHPhyKsxPDxcCxnbaPREpRbx3XKKfkEgVoUI7Ipk7EzEgCnkwJdeXKtXLmI8E20dPahl3AzHL_UP1v6Ua471YzuTonWFcC39ePYucaIaROweP7K7Z7zmP7UKzlvcvA6rl0xtqmYP_O06OTc?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### 2. Select Email or Journey Orchestration channel, then click <img src="../../.gitbook/assets/image (685).png" alt="" data-size="line">to create a new Customer Journey

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcD0nlsN7OUWR92RJJej3tWyZxr50pjDz4jIuns5MNKykpDrMpO6fl9c3844KriWcapjl0iRFXq5EXqQkY2rY6kACkYrIq9POVqg-MwAjW2_s93bSvS925fmSVBTAvmYhRyYILiSt6UF8b4H7PvBLomsvcW?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### 3. Complete the setting of the Trigger node and Action node

* Drag  & drop the desire trigger node and action nodes in the Journey and finish the setting&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd5MxNq-QGBDXbpq2QFi3EWIn_s69myZvOzam6T8TYy0IyECA_m6K3MeBUzM7LOffPEePZeRAp21eRzyBx30Z9d_rruidkgNlL2Ea4dXHhRbHU9vy-SUOdztBfvI0Ei2y0mEIy1H_AeR74rSwnkzVCyg_du?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### 4. Add and configure Destination node

* Drag & drop the **Mailgun** Destination into the Journey, then select **Design from Email template** to create a new Destination

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXef5reCqurZzxpKmai9QLPmUznsEGZZr2v7TRDZNSXCE4lbxvfq5mUhjFzU4Ckh_vo-H2bLy6rfogBbacEX2rPvu26NWMLQXQMvH4MYmSJDbS8U-_0MQhEfec7PG03ioepC0VQtF6HKjMYaV40rTctYNalt?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

Then finish the settings of **Mailgun** Email as following:

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXet5d5yjyMkdFp03F0K6eDm1g57A2q2XQF6VlOgfOeyP14wIgFzWLc1VWxvJZeKTKyljBN_onev0gu765JoMBZxLDpePCsIjfenIus1LVtB3_EvK8jzHH9vbJirXW1ZbEMXuMqSxk_5EaDgLWmcMnIgAuBQ?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

#### Setting tab:

* Campaign Name: Input the name of this campaign
* Delivery Destination: Select the destination you created in **STEP 1**
* Delivery Algorithm: Randomization (default)
* Delivery Hours of the Day: Select the time of day you want to send this Email.

**Compose tab:**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdfS3mF2_12g2g1Z5RL-sdt7euntBpR2orXj8O7kExZJioJXsVMAyVlQyfkagvgzIor_vMx3Nj5PovuEWxg0v9iOVj3yrE7cw4ztaImw03ubFnsVS3PpxsRwgWrSh4LcG8KqTb9bhBojW6-w9KKw1AecPXq?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

Finish the setting of **Compose tab** as any other Email Destination.

### 5. Save and Activate the Journey

* Click **Save** and then click **Activate** to save and start running the Journey

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc6QZPyf3YWK7GySdvY2U5ue58vRKHEJ3wK7ttF5qgQzbrMwNpYQHkrmfm3iVNYb22mShTwPr6_0CabI8cbRvPgNsqrgdwOfZGwQc9pjJ_HWVTS9v-hit6a6gfv9x27gKvJlUjLbQ4WGJjrX0xWmpOW7KdG?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>
