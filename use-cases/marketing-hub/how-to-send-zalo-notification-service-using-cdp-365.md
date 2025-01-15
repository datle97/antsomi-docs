---
description: >-
  "Zalo Notification Service (ZNS)" is a service that sends customer care
  notifications via API to phone numbers using Zalo
---

# How to send "Zalo Notification Service" using CDP 365

## 1. Instruction to get information for using "ZNS" in CDP system

* Accessing the link [Zalo Developer](https://developers.zalo.me/) to log in your account

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2F9erAqnbKCVhFZ8EY3mRe%2Fimage.png?alt=media&#x26;token=74cde166-ec50-4ab0-a302-af94a3e0055f" alt=""><figcaption><p>Log in your account</p></figcaption></figure>

* Selecting existing app or creating a new one

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FMoDtG5RLADhVWPNzWDGE%2Fimage.png?alt=media&#x26;token=18d26d66-a9f0-48e0-92b4-d259b25e2583" alt=""><figcaption><p>App</p></figcaption></figure>

* When clicking an app, the screen will be shown as:

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FTG2arLJd0FeWWtou5oSn%2Fimage.png?alt=media&#x26;token=081b7895-5c8e-4b03-8b91-983f96e103cb" alt=""><figcaption><p>App Detail</p></figcaption></figure>

* We can take the information of "App ID", "App Name" and "Secret key" on this screen
* We also need the information of "Refresh token" for using in CDP
* We can get "Refresh token" via getting "access token"
* Accessing the link [API Explorer](https://developers.zalo.me/tools/explorer/) and selecting "**OA Access token"** type then clicking "Get access token"

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FplQeJNLg1PFbSHBAumAu%2Fimage.png?alt=media&#x26;token=5418b8ea-dfd0-483e-9c3e-166667cb8e8e" alt=""><figcaption><p>Get OA access token</p></figcaption></figure>

* We can click to copy "Refresh token"

With all information above, we have enough data to create "destination" in CDP system

## 2. Destination ZNS

To create **ZNS** destination, we need to access **Channel Integration**.

Hover your mouse over **Settings**. Choose **Channel Integration**.

<figure><img src="../../.gitbook/assets/image (60).png" alt=""><figcaption></figcaption></figure>

After that, we click **+** button Create and select **Zalo** channel

<figure><img src="../../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

Select **Destination catalog** as **Zalo Notification Service**

<figure><img src="../../.gitbook/assets/image (50).png" alt=""><figcaption></figcaption></figure>

Fill out **Name**, required **Info** and then click **Save**

<figure><img src="../../.gitbook/assets/image (52).png" alt=""><figcaption></figcaption></figure>

* "App ID", "Secret Key", "Refresh Token" are information we mentioned in **section 1**
* "Country Phone Code": **84**
* "Is Scheduled": **true**

After clicking **Save**, we have finished creating **ZNS** destination.

To send ZNS to customer, we need to use Customer Journey

## 3. Sending ZNS via Customer Journeys

* Log into CDP 365 system, hover your mouse over **Marketing** -> Choose **All Channels**

<figure><img src="../../.gitbook/assets/image (53).png" alt=""><figcaption></figcaption></figure>

We have 2 channels that are supporting to send **ZNS**

* Zalo
* Orchestration

<figure><img src="../../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>

* Click **+** button to create a journey.

<figure><img src="../../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

* If you choose the channel as Journey Orchestration then you need to add 1 trigger node first (Action base or schedule trigger).

For this example, we will use Action-based node to send ZNS after the customer purchase.

<figure><img src="../../.gitbook/assets/image (3339).png" alt=""><figcaption></figcaption></figure>

* Add Destination node and select ZNS destination

<figure><img src="../../.gitbook/assets/image (3340).png" alt=""><figcaption></figcaption></figure>

* Choose a ZNS template, fill out necessary information, and Save

<figure><img src="../../.gitbook/assets/image (3341).png" alt=""><figcaption></figcaption></figure>

* Phone number: Phone number of customer

<figure><img src="../../.gitbook/assets/ZNS - 2.gif" alt=""><figcaption></figcaption></figure>

* Template data: Information we want to send to customer. Go to the ZNS template to get dynamic parameters, and map them to CDP 365 attributes. It means taking attribute values from CDP 365 and show on ZNS messages with the corresponding params. &#x20;

<figure><img src="../../.gitbook/assets/ZNS - 3.gif" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/ZNS - 5.gif" alt=""><figcaption></figcaption></figure>

Notes: Besides the CDP 365 attribute values, the Template data can be a fixed value.&#x20;

After finishing the setting of journey, we can **activate** and send this **ZNS** to customer.
