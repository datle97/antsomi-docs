# How to send "SMS Yondu" using CDP 365

### 1. Access "MARKETING HUB" app and go to "Destinations" menu

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FiQgKWXUuBHPKNXVLTJL8%2Fimage.png?alt=media&#x26;token=abbd150b-beb9-4e40-a72f-ac0fcadd91b8" alt=""><figcaption></figcaption></figure>

### 2. Click "+" button and select "SMS"

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FrDh4v6F3ldLqAVwcKfXl%2Fimage.png?alt=media&#x26;token=382eb25b-3820-43ac-a8f4-3418e55fba4b" alt=""><figcaption></figcaption></figure>

### 3. Select "Destination catalog": "SMS Yondu"

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FFXbTnP6L8Og0bcQgGvOq%2Fimage.png?alt=media&#x26;token=499193a8-11b4-4c1f-866c-3a2301950598" alt=""><figcaption></figcaption></figure>

### 4. Fill out "Destination name" and required Info

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FTveWMqXVNzNe5BgaPQ0i%2Fimage.png?alt=media&#x26;token=3b1f803f-d26a-4e4b-96a2-99f79c782f37" alt=""><figcaption></figcaption></figure>

| Field                 | Description                                                             |
| --------------------- | ----------------------------------------------------------------------- |
| User name             | Client’s username on Mobile 360 Platform. (Supplied by Yondu)           |
| Password              | Client’s password on Mobile 360 Platform. (Supplied by Yondu)           |
| Receiver phone number | Phone number of sms recipient.                                          |
| Shortcode Mask        | Client’s provisioned source at Mobile360 Platform. (Approved by Yondu). |

#### Note: You can select the customer's phone number by:

Click "Add Personalization"

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FifvjIePJIZKP54sFa4qE%2Fimage.png?alt=media&#x26;token=2151ce49-08ad-42c8-91c1-828d53ff0d02" alt=""><figcaption></figcaption></figure>

"Personalization type": Select "Visitor"/"Customer" Attribute

"Personalization Attribute": List of attributes of Visitor/customer that you selected at Personalization type -> Select the attribute containing the customer's phone number that you want to send SMS

Click "Insert" button to finish adding personalization

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FUQtwWMyMnU8cBvXYWhk3%2Fimage.png?alt=media&#x26;token=e06ba1bc-1f13-4271-b4d3-d9ceb5c087a3" alt=""><figcaption></figcaption></figure>

### 5. Save to finish creating the "Yondu SMS" destination

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FqjPzg7UTE3BATrCKF4lr%2Fimage.png?alt=media&#x26;token=346d2f3c-df99-4a63-915b-09e2857c9ce6" alt=""><figcaption></figcaption></figure>

### 6. Sending "Yondu SMS" via Customer Journey

Log into CDP system,  access **"MARKETING HUB"** app and go to **"Customer Journeys"** menu

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FVP19xnZV2JvVmId0MRIC%2Fimage.png?alt=media&#x26;token=d9cceea5-710d-45f1-92fc-d01f2e584b3a" alt=""><figcaption></figcaption></figure>

We have 2 channels that supporting to send "Yondu SMS"

* "SMS"
* "Journey Orchestration"

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FFJ3g9WOQGMb4NqoDJZJu%2Fimage.png?alt=media&#x26;token=0f522515-c1bc-49b3-a998-7caff880347a" alt=""><figcaption></figcaption></figure>

Click "+" button to Create Journey, add "Destination" node and select "SMS Yondu" destination

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FO6oWIFNCivpSAa2zEu95%2Fimage.png?alt=media&#x26;token=9a9228dd-29f2-4e98-bcd1-2346a32e0ac0" alt=""><figcaption></figcaption></figure>

Fill out necessary information

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FmN1xczUKwgv8kKXPfi2G%2Fimage.png?alt=media&#x26;token=ef665fca-a929-47e6-9d48-e47caf94de8a" alt=""><figcaption></figcaption></figure>

Message: message content which the user wishes to send (limit 450 char)

Click "Save change" button to finish setting journey

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2F1dPIurc43XX5e7R8EM6B%2Fimage.png?alt=media&#x26;token=f162e90a-aa76-4c07-8b92-559a24327844" alt=""><figcaption></figcaption></figure>



