# Smart Inbox

## I - Introduction

Smart Inbox is a channel that allows you to send messages to customers. However, it's a special channel. Specifically, when it's used on your website, it serves as a message center that receives all messages you send to your customers. If it's used on your app, you can use it to deliver messages to the app's notification module.&#x20;

<figure><img src="../../../.gitbook/assets/image (2807).png" alt=""><figcaption></figcaption></figure>

## II - Detail

### First of all, you have to create a smart inbox destination

Click![](<../../../.gitbook/assets/image (2829).png>) to generate a new destination that belongs to smart inbox channe&#x6C;**.**

<figure><img src="../../../.gitbook/assets/image (2842).png" alt=""><figcaption></figcaption></figure>

There are four steps to set up a Smart Inbox destination.

#### Step 1 - General Information

You need to complete certain information fields for the destination.

* General information: Fill in the name and description for the destination.
* Configure fields: 'Recipient' refers to the objects to which you want to send messages. This includes two options: Customer ID and App Visitor.
* Advanced push settings (optional): You can limit the number of times the audience is engaged in this journey.

<figure><img src="../../../.gitbook/assets/image (2841).png" alt=""><figcaption></figcaption></figure>

#### Step 2 - Notification - Verify Configure

This channel supports an additional feature that sends web and app notifications to inform users about new messages through two channels: Antsomi WebPush and Antsomi AppPush. Therefore, you need to verify these two channels before using them.

Note: You may not need to successfully verify both channels to proceed to the next step.

<figure><img src="../../../.gitbook/assets/image (2840).png" alt=""><figcaption></figcaption></figure>

#### Step 3 - Inbox - Display Setting

You can design the interface of smart inbox when it displays on your website.

In the **Toggle** tab, you have the freedom to craft the perfect toggle style. Choose from a variety of icons or images, adjust its size and color, and even fine-tune the badge style. Elevate your design by adding animations to your toggle, making it more engaging and attractive.

<figure><img src="../../../.gitbook/assets/image (2839).png" alt=""><figcaption></figcaption></figure>

In the **Notification Box** tab, we provide the following settings:

* Notification Box: Adjust the width, height, corner radius, and background color of the notification box.
* Header: Refine the title of the notification box.
* New Message Indicator: When users receive a new message, the indicator will automatically count. You can also change the style of the indicator.
* Category: We support you in categorizing messages. Design the style for categories according to the campaign's objective.
* Unread Indicator: We highlight unread messages with an unread indicator, and you can change its color.
* Notification Bubble: This is the most crucial part of the notification box. Currently, we offer three templates for you. Choose the suitable template for your marketing campaign.

<figure><img src="../../../.gitbook/assets/image (2838).png" alt=""><figcaption></figcaption></figure>

Note: To send messages to the app's notification module, you need to install the SDK according to the device's operating system (Android/iOS).

Installation Instructions for <mark style="color:blue;">Anrdroid</mark>, <mark style="color:blue;">IOS</mark> (in progress).

#### Step 4 - Authentication

If you send messages to the app's notification module, proceed to Step 4.

[<mark style="color:blue;">Authentication Instructions</mark>](https://docs.antsomi.com/developers-guide/hybrid-apps/flutter).

<figure><img src="../../../.gitbook/assets/image (2837).png" alt=""><figcaption></figcaption></figure>

### After creating a destination, you need to add a script to your website&#x20;

First, add the script below to the `<head>` tag on your website.

{% code fullWidth="false" %}
```html
<script src="https://st-platform.ants.tech/js/libs/app-inbox/app-inbox.min.js?v=1"></script>
```
{% endcode %}

Second, add the following script to the `<body>` tag.

```html
<antsomi-webinbox portalid="your portalId" destinationid="your smart inbox destinationId" lookupType="customer" lookupId="{customerId}" selector="body"></antsomi-webinbox>
```

Note: You need to change the `portalId` and `destinationId` (the ID of the Smart Inbox destination you want to use on your website).

#### How to get `PortalId` and `DestinationId`

<figure><img src="../../../.gitbook/assets/image (2834).png" alt=""><figcaption></figcaption></figure>

### How to set up a smart inbox campaign in Customer Journey?

In **Settings** tab of Smart Inbox Node, select a destination you want to display on your website.

<figure><img src="../../../.gitbook/assets/image (2833).png" alt=""><figcaption></figcaption></figure>

In **Compose** tab, you have the flexibility to set the message category and craft your message by including a heading, image, and content. Furthermore, you can enhance your message by incorporating buttons, which can be utilized to guide your customers to a designated landing page.

<figure><img src="../../../.gitbook/assets/image (2832).png" alt=""><figcaption></figcaption></figure>
