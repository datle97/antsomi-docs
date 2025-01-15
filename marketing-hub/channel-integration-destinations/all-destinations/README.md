---
description: This page include instruction on how to create and remove a destination
---

# All Destinations

## Create a Destination

To create a destination, follow these steps:

### Step 1 - Start off

* Click on the Create button&#x20;

<figure><img src="../../../.gitbook/assets/image (2932).png" alt=""><figcaption></figcaption></figure>

* Choose the Channels & Catalog (Vendor) you want to use

<figure><img src="../../../.gitbook/assets/image (2933).png" alt=""><figcaption></figcaption></figure>

### Step 2: Declare information

<figure><img src="../../../.gitbook/assets/image (2934).png" alt=""><figcaption></figcaption></figure>

Depending on the combination of the chosen channel & catalog, the step will vary. In general, there will be fundamental fields in each destination, such as:

#### General Information

* **Destination Name\*** : This is a required field
* **Description**: Enter what you want to describe the destination
* **Method:** The sending/receiving method depends on the Destination Catalog you choose provided

#### Configure fields&#x20;

The configure fields will be varied depending on the type of Destination Catalog you chose above. Here you need to declare the information fields required by the third party.&#x20;

{% hint style="info" %}
Locate the description of configure fields for a specific catalog in a channel

* [Email](email.md)
* [Web Personalization](web-personalization.md)
* [Web Notification](web-push-notification.md)
* [App Notification](app-push-notification.md)
* [Conversation](conversation.md)
* [Webhook](webhook.md)
* [SMS](sms.md)
* [Viber](viber.md)
* [Line](line.md)
* [Zalo](zalo.md)
* [File Transfer](line.md)
{% endhint %}

#### General Setting

_Frequency Capping_

Frequency Capping settings allows users to limit the times an audiences receiving a marketing message.

<table><thead><tr><th width="262">Option</th><th>Description</th></tr></thead><tbody><tr><td>Ignore duplicate messages for the scheduled journey</td><td>One audience just receive one message in an iteration of journey schedule </td></tr><tr><td>Limit frequency for the journey (3 months duration)</td><td><p>Limit allocation frequency to 1 audience in a journey for 3 months </p><p>(Ex: 2 times/person)</p></td></tr><tr><td>Limit frequency for destination</td><td><p>Limit allocation frequency to 1 audience per unit of time (hour, day, etc.) </p><p>(Ex: 3 times/month, 1 times/day)</p></td></tr></tbody></table>

_Delivered rate_

Delivered rate setting allows users to limit the number of messages sent per second for a specific Destination.&#x20;

<table><thead><tr><th width="333">Option</th><th>Description</th></tr></thead><tbody><tr><td>As fast as possible</td><td>The maximum number of marketing messages sent per second will depend on the system possibility.</td></tr><tr><td>Limit send rate {x} time(s) per second</td><td><p>The number of marketing messages sent per second will be set by user. </p><p>(Ex: You are creating a destination for G Suite Email, the value you set is 100. That means only 100 emails will be sent in 1 second)</p></td></tr></tbody></table>

### Step 3 - Determine permission

Choose who have the permission to view & edit the created destination

<figure><img src="../../../.gitbook/assets/image (150).png" alt=""><figcaption></figcaption></figure>

## Remove Destination

If you want to remove a Destination, follow these steps:

1. Select the destination aimed to remove
2. Click ![](<../../../.gitbook/assets/image (1071).png>) and select '**Remove**'

<figure><img src="../../../.gitbook/assets/create new des (1).png" alt=""><figcaption></figcaption></figure>

3. Confirm your action

<figure><img src="../../../.gitbook/assets/image (292).png" alt=""><figcaption></figcaption></figure>

* Remove: Confirm to remove the destination (This button only enable if the chosen destinations are not being used as input of other features)
* Cancel: Close the pop-up and cancel the action

