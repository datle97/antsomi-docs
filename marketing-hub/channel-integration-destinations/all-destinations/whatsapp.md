---
description: >-
  Seamlessly Connect CDP 365 with many vendors to use WhatsApp: A Practical
  Guide to Supercharge Your Marketing Campaigns
---

# Whatsapp

This feature manages the connection of CDP 365 with vendors which providing services of sending messages through Whatsapp

## Infobip Whatsapp

### Prerequisites

In order to successfully implement the whole process, you need to ensure these factors are met:

* **Prerequisites Access Requirements:** CDP 365 and Infobip accounts with the relevant permissions.&#x20;
* W**hatsApp Business Approval:** Confirm the WhatsApp Business API setup with Infobip.
* **User Interaction**: To send a free form message, the user needs to interact with OA or vice versa within 24 hours
* **Receiver phone number**: The sending phone number must include the country code & not contain a plus sign

### Instruction

#### Step 1 - Choose Infobip Whatsapp&#x20;

<figure><img src="../../../.gitbook/assets/image (4137).png" alt=""><figcaption></figcaption></figure>

#### Step 2 - Add the configuration info

<figure><img src="../../../.gitbook/assets/image (4138).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="161">Field Name</th><th>Description</th><th>NOTE</th></tr></thead><tbody><tr><td>API Key</td><td>Unique key provided by Infobip for API authentication</td><td></td></tr><tr><td>Base URL</td><td>The Base URL is the foundational endpoint provided by Infobip to authenticate and connect with their API services. It determines the region and server your account is hosted on. You can find this URL in your Infobip account settings or API documentation</td><td>Ensure you use the correct Base URL for smooth integration with CDP 365.</td></tr><tr><td>Phone Number (Recipient Number)</td><td>The number you intend to send messages to </td><td>Must include the country code</td></tr><tr><td>From Number (Sender Number)</td><td>Your WhatsApp Business phone number configured on Infobip</td><td></td></tr></tbody></table>

#### How to find authentication info in your Infobip account?

**Base URL**

* Infobip supports a personalized base URL for API requests. By default, each Infobip client has a different base URL which helps our platform identify the originator of each API request.
* To see your base URL, log in to the hub with your Infobip credentials and choose DEVELOPER TOOLS >> API Key

<figure><img src="../../../.gitbook/assets/image (4139).png" alt=""><figcaption></figcaption></figure>

* On this page you should see your base URL in this format: xxxxx.api.infobip.com

<figure><img src="../../../.gitbook/assets/image (4141).png" alt=""><figcaption></figcaption></figure>

**API Keys**

* Only users with certain roles can fetch api key; for example, Account Manager and Integrations Manager roles.
* If you have created any API Key, click on the button CREATE KEY

<figure><img src="../../../.gitbook/assets/image (4143).png" alt=""><figcaption></figcaption></figure>

* Then, choose the necessary scope of your endpoint by following the documentation. To understand these scope, you could read this document: https://www.infobip.com/docs/api/channels/whatsapp/whatsapp-outbound-messages/send-whatsapp-template-message
* If your purpose is sending a whatsapp template messages, scope would be: "message:send", "whatsapp:manage" and "whatsapp:message:send".&#x20;
* Each endopint has it's own set of scopes, so make sure you follow the documentation.&#x20;
* Eventually, click CREATE and copy the Key & paste to CDP 365

<figure><img src="../../../.gitbook/assets/image (4144).png" alt=""><figcaption></figcaption></figure>

After created integration successfully, you can now create a Customer Journey to send your messages

<figure><img src="../../../.gitbook/assets/image (4145).png" alt=""><figcaption></figcaption></figure>

For details, see the example [here](https://docs.antsomi.com/cdp-365-user-guide-en/use-cases/marketing-hub/how-to-send-messages-using-oneway-sms-destination#step-2-create-a-customer-journey)

### Results

#### 1. Quick Test

The testing process is considered successful when you see the following response:&#x20;

{"to":"{receiver phone number}","messageCount":1,"messageId":"antsomi-{receiver phone number}-{random number}","status":{"groupId":1,"groupName":"PENDING","id":7,"name":"PENDING\_ENROUTE","description":"Message sent to next instance"\}}



<figure><img src="../../../.gitbook/assets/image (4146).png" alt=""><figcaption></figcaption></figure>

#### 2. Run Campaign

#### Whatsapp Chat Screen

In reality, the message will be sent to Whatsapp users, see example below:

<figure><img src="../../../.gitbook/assets/image (4148).png" alt="" width="375"><figcaption></figcaption></figure>
