---
description: Used to verify the code sent to the audience
---

# OTP Verification

## I - INTRODUCTION

To add a OTP verification block, drag and drop it to the workspace

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd6GQgMET1jkzaeCkl19ceFPXzECAwgaSnfp-fVgyx2CEMkEVZx9qPQ_2n5qVrxpdkOiEfqk4w-LZfF9jVEs2gYTGP2rKTmKWHlI73NVrK41uz7LIJ-v9VCPYBq_R5uW_SMHYAihSshxwkZBbXsNMO7zInx?key=UxIPxAd5bPKNJihWsLwzZQ" alt=""><figcaption></figcaption></figure>

The elements in the block include:

* OTP Form : The field to input the code
* Expiration timer: A countdown to mark the time the code could not be used
* Verify button: The CTA button used to verify OTP action
* Resend button: The CTA button used to send the code again

In the setting panel, there are two tabs:

[Content](otp-verification.md#a-content) - Include the basic information settings&#x20;

* Layout: Choose the layout of the block&#x20;
* OTP Form: Set general information of the input field which allow users to enter the code
* Resend Button: Basic settings of Resend button&#x20;
* Verify button: Basic settings of Verify button&#x20;
* Message: set up notifications on the block: Verify OTP and Resend&#x20;
* Event Trigger: The event to be fired if the OTP has been verified successfully&#x20;

[Advanced](otp-verification.md#b-advanced) - Include the complex design settings&#x20;

* OTP Form Styling
* Input Field Styling
* Resend Button Styling
* Verify Button Styling
* Message Styling
* Container Styling

## II - DETAILS

### A - Content

#### 1. Layout

Popular layout will be chosen by default. You could choose any type of layout you want. The differences between these layouts lies in the arrangement of elements in it.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcxdjT8CFoL4HGSTYueiD3MmbKnglSjqt4BGUlad3ItnpbYyO8B2ExaTa6bV0XPx_qDCv8dmlK8ROzqPFf9tLFDYYscH3bnikeOrlchHDEn2PbedSPaiBzggL1f1CUZH7XSGtsWuJM1Nt7bZdWMhPEFFnY?key=UxIPxAd5bPKNJihWsLwzZQ" alt=""><figcaption></figcaption></figure>

#### 2. OTP Form

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdw1ykWR1p-NbJquU_519hd4G2yWdgnLdGZbk6pVaep6ciSebDU44Tg29KB_G0v9CISDzi43Pafa_dmQ9hJDvl-anHbD1DA2QRGPqYcokStymC4TOBNvSeK5KrfKXZVA-HntcESvLzihdv1mPwqVI7MlYY?key=UxIPxAd5bPKNJihWsLwzZQ" alt=""><figcaption></figcaption></figure>

* Width: The width of OTP block
* Align: The alignment of elements in OTP block
* Timer Label: The label of the countdown. The amount of time to be count downed will vary depending on the Service Provider set in Optin Field (Read [here](../../../../use-cases/marketing-hub/strengthening-user-identity-verification-with-otp-authentication.md))
* Expired Message: The message which will replace the countdown if the timer has counted to 00:00

#### 3. Resend Button

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfUgFt6BxNmNKJOw_elnza8Mmm5TvKYLLZDVzYZB9Skaod6BuJO8rm8fks6N0ckGWfMZsYbCCmelb2HW9FUtDX7QsFhO8oLtniyLhzD8o0bE69yGfWXZYsYCfX2kYtxqzzEqqZqlcPQD24WgFgiwfygpgBY?key=UxIPxAd5bPKNJihWsLwzZQ" alt=""><figcaption></figcaption></figure>

* Description: The description attached to the Resend button. You can see it only if Popular & Neat layout is chosen
* Button Text: The label of the button
* Width: The width of the button
* Align: The align of the button
* Button Size: The size of the button

#### 4. Verify Button

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfUgFt6BxNmNKJOw_elnza8Mmm5TvKYLLZDVzYZB9Skaod6BuJO8rm8fks6N0ckGWfMZsYbCCmelb2HW9FUtDX7QsFhO8oLtniyLhzD8o0bE69yGfWXZYsYCfX2kYtxqzzEqqZqlcPQD24WgFgiwfygpgBY?key=UxIPxAd5bPKNJihWsLwzZQ" alt=""><figcaption></figcaption></figure>

* Button Text: The label of the button
* Button Click Action: The action to be performed after the button is clicked
* Go to View: The screen to be appeared after the button is clicked
* Width: The width of the button
* Align: The alignment of the button&#x20;
* Button Size: The size of the button

#### 5. Message

Here you can enter the content and position of the message to be displayed when:

* The code has been verified unsuccessfully
* The code has been sent again

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdZF3atAwTj56MtjghXNvPvbZdl4aOocuaUx6chq1Hl9IOx8Kv2KDjN7cKv-UgUzTpD76JCSmuFvrtTTUpn8nhZVjWVbKFJIgOYyhoQBFTHWLtB1Zf7jyZntLUmIu7q_hLVyic6SJnkXIYmLtx3haCMS6s5?key=UxIPxAd5bPKNJihWsLwzZQ" alt=""><figcaption></figcaption></figure>

#### 6. Trigger Event

Choose the event to be triggered after the code has been verifed successfully. By default, the Verify OTP Successfully event will be chosen. This event could be used in Segment and Customer Journeys later. (Read [here](https://docs.antsomi.com/cdp-365-user-guide-en/use-cases/marketing-hub/strengthening-user-verification-with-otp-authentication-a-use-case-in-identity-verification#iii-data-usage))

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdvHLDL8axTRo7Zizhq3Kv-Nr8n0huQTHoATCiv3zMmiPVLmYZekvMuXieo2uYOWue8Vr9gKb1uGghIQuJ1bLDJ7EX6u4I2CbmJbDAE-WgR9s8oavUc45CU8n5jI1JKhI7V6bmlMVNIgVD1lyniKk5mVPns?key=UxIPxAd5bPKNJihWsLwzZQ" alt=""><figcaption></figcaption></figure>

### B - Advanced

#### 1. OTP Form Styling&#x20;

Adjust the appearance of the whole OTP block

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXddZ3NzqXPnh6GSZ3lxS3ILS213rNd6UQPU-wFrFW7UFHjG77zOXWekpmmHKrBA-0WGBXTxsOBsRQvGVhzuirCJnmKtHhVwOw3FWMfv8n99y_BWeheiWOazd90IpAZOxY8R8K3ZOTW6QXOcV-JcT67KxMGO?key=UxIPxAd5bPKNJihWsLwzZQ" alt=""><figcaption></figcaption></figure>

#### 2. Input Field Styling&#x20;

Adjust the appearance of the OTP input field

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfm39kWv9--2Irq-738oYcP2ZBuXCsOrmCnjV7H2dPelWEY3lihhL8pXuOUAwbKK7u_9fzieV5ZUgo4mC-4VzI5bLMzCy5GI8soLgx_EjaLUAUxSenyGyWYniA836XTRGEUnSvWcdfan1OKvjTgG1voz_IZ?key=UxIPxAd5bPKNJihWsLwzZQ" alt=""><figcaption></figcaption></figure>

#### 3. Resend Button Styling

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcw1K2VfVbECbtyL1wq0jpyFzd7uT4QAAtZ5ACNSB4jxkl71WXAEY5SCzdyQjPPiTJX6kD3p6TdncwK49-D83pzHBK9BCfu9lCpbKFY_XR2XKeLApbpCNywwS9fli5FLMyQ5VwEWlHAvOu0ajT3ARbOcsI?key=UxIPxAd5bPKNJihWsLwzZQ" alt=""><figcaption></figcaption></figure>

#### 4. Verify Button Styling

Adjust the appearance of the Verify Button

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcT1KS7UoVbB8HUIBZF62pN5jN3OLHVx8jkka9r5-Mbryp504UOHUd1jD1x_xe8pufydpynh-OpORiLIuida8LtmDMhr3DeGVNj8m76un6HzwK2tw_dLEen03iEFOoqQP5F5ihZDzI3ZWm6bktkB-ed6tA?key=UxIPxAd5bPKNJihWsLwzZQ" alt=""><figcaption></figcaption></figure>

#### 5. Message Styling

Adjust the appearance of the message

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfBUplFnttawY1RptdzveikJJBODeR6vEuoLoKwZTtyoqJdU5lUSIOwuLe0X5KpEmXhd78hxrqkt_PCUqvpYIKAxA_UtsTpT3M33cZ2D1WYu2WGlUZhMcLVvyUsi_0l2ZMLjp4mmelcoPU9wyb2roL35B_t?key=UxIPxAd5bPKNJihWsLwzZQ" alt=""><figcaption></figcaption></figure>

#### 6. Container Styling

Adjust the appearance of the whole container which include the block

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdmiEvjsZB_XE8kTHN-MevL7nXbNxIpPS3sRF6TW9hYFmGGPsdTMXnrLd1g5g11vfgsanTWgz-GPiusIfnTfkmnG5RT3qk0RVSLQmBj1uzUjn1TAKsFWV-ftzbgOStGKO0HYx_4NgVdZYVReSQZj0ptfSQI?key=UxIPxAd5bPKNJihWsLwzZQ" alt=""><figcaption></figcaption></figure>

After editing the block, you could have the result like the example below:

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdpVdZhDGomletDkcx4dE4Mc8efKQFwu2ZrPz4FFiG3VxiW1B72ofWWoW2RokGM9DVrJtuHsr4ibxdnaBaSOM3Qp3EcvlTFXHl9bVIbaxZT7Yt2OQ0zD_r3rJASHqSaXJDbgmaAmK-b_2B6NennE8aJp3Q5?key=UxIPxAd5bPKNJihWsLwzZQ" alt=""><figcaption></figcaption></figure>

