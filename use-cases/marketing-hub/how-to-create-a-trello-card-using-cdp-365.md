# How to create a "Trello Card" using CDP 365

## ![](<../../.gitbook/assets/image (1087).png>) Create destination Trello

For creating **Trello** card purpose, destination Trello has been designed and implemented.

Destination Trello is in the **Webhook** channel.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfeUGc5g5VjYDFSA4Rpi9MGAl2HegeP9watvvULNUjN2IoMapdYkoA_CxChcaxahemD_kWV5o2z0LiJQ9sdSvJFJK4Wv9KgMVM0M_0KNlmAmKt1p6t2gtrsS_fM1IPpFxHCX8s3pLSHV9-bALTYp6Fz9f5m?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

For using this destination, some information are required as follow:

* App-key and token
* List ID
* Member ID

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfUbRwakElbMSVbqjKLdmi4wH5q49fO-sfaUykZpwr7MQHseQfUlcCELoQmQL24B-AgoAmOg8HWUzSAC8JcilEd2TGqZIoC7yB93i0zZza7AhkSOwhgwVraTdMoyXvynmDIQg_XuQaKdTOTLDdeqwkFA47D?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

#### App-key and token

App-key and token can be obtained from the website : [https://trello.com/app-key](https://trello.com/app-key)

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FaIzvMJMsDA2AVRXqHWGx%2FUntitled.png?alt=media&#x26;token=e286285a-269a-4cde-a953-e0da782783e9" alt=""><figcaption></figcaption></figure>

#### List ID and Member ID

* List ID: where the Trello Card will be created&#x20;
* Member ID: which member will be assigned to the card. You can add more than 1 member ID and separate them with commas

In order to get **List ID** and **Member ID**, you can follow the instructions below:

1. Go to your Trello board&#x20;
2. Add "**.json**" to end of the URL
3. Format the JSON so it's readable (you can find a JSON viewer online)
4. Search for **List ID** and **Member ID**

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2Ft20kwPRbWNGmJRJiCSLB%2Fimage.png?alt=media&#x26;token=7c86928e-70f2-4b8e-82c2-a01279740a5d" alt=""><figcaption></figcaption></figure>

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FnC5BkZo0VMoSlTzIrI4C%2FUntitled1.png?alt=media&#x26;token=05ff8d18-84e9-487f-b4a1-4e349666b760" alt=""><figcaption></figcaption></figure>

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FlIXK1w7Cx3PbdOHxmqkH%2Fimage.png?alt=media&#x26;token=1059e26c-2e88-4266-a54a-e5ba6dba73c1" alt=""><figcaption></figcaption></figure>

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FdNsrQs69K9l8jNoR2f8z%2Fimage.png?alt=media&#x26;token=48511b0c-de10-4579-9a19-5d5ae61cfccf" alt=""><figcaption></figcaption></figure>

## ![](<../../.gitbook/assets/image (2161).png>) Set up journey to create a Trello Card

1\. Hover your mouse over **Marketing >>** Choose **Orchestration**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfBw52ZsG4WN5-puGs_fAPAKPtitQZocFd5uuuBsX1rpab_tjRRNn_yg8VyNx184rcAF7ia4j1LOhTrU2aHc3s2KA4KcHiruC-b2qMhOgj7kIjQUqDa8BHOM6-T0DQUlL8L5kG516sL8wXh00_lSUDqY-Xh?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

2\.  Click icon ![](<../../.gitbook/assets/image (1493).png>) to create journey

<figure><img src="../../.gitbook/assets/image (3552).png" alt=""><figcaption></figcaption></figure>

3\.  Select the account you want to create Journeys on.

4\. Set up the necessary information for Journey

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcT9Bh83XsYNoVjgOcF_c-OCwlhVHYFgJlXH9Oxjn61B0Crf1-pELdrmXjoa7a3jFKEc3V0b6gGszBOO9_MI19wxXYFV8hz_fCk5_3npjOO4edIV5wjSAaOBdc9FryUvSDXIorfbRehLFLc9mDGM-Z6LtwB?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

5\.  Add destination Trello

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdRc6YiDY8okH5EhqYO6_WJH0vg1ZlBuVVQtqN4S2IKXKlrijQ845diRVPiuIq-1vbOzUwGBeJCjlsx2x5H8sRuyoVKMm90p31H5TAUGaMUUJIVuaR8Hwk8j8AjnulS7Ql5e2t0oKkqXY0i45h0y3IjYZs?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

6\. Choose the correct destination that users want to create the Trello Card

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd4tSR_OpLdofMPmxhkBNUrqzD-4Q11wlCfiiUANVIbH8saq_bjcbpMzBRklZdeYs6Lvty0rMiJBS8h2iqdUege7xmQVnoN7Ucar2GEIbDqk3OGVdA7onb4WxQT9ySlp5THu2pv_EGxhGumSv2uVh16K08?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

7\. Enter the title and content of the Trello Card

* Name: title of the card
* Description: content of the card

<figure><img src="../../.gitbook/assets/2024-09-09_16-44-38.png" alt=""><figcaption></figcaption></figure>
