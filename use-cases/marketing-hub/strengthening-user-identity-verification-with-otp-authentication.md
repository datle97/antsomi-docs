# Strengthening User Identity Verification with OTP Authentication

## I - INTRODUCTION

In the realm of digital services, verifying the identity of users is crucial for maintaining trust and security. Also, it plays an effective role in refining the lead data so that special offers are delivered to qualified audiences.

One effective method for verifying user information is through OTP (One-Time Password) authentication. This use case delves into how implement OTP Verification on CDP 365.&#x20;



<figure><img src="../../.gitbook/assets/[Monthly Training] - CDP 365&#x27;s New Features.png" alt=""><figcaption><p>OTP Verification Flow</p></figcaption></figure>

In order to create a complete OTP Verification flow, you need to prepare these things before hand:

* Connection to OTP Service Provider: These provider will be in charge of sending OTP to your audience (whether via SMS, Email or any other channels)
* Artwork of the three screen that will be displayed to user:&#x20;
  * User registration: Including a form allows users to provide their information (SMS, Email, etc)
  * Identity Verification: Including a form allows users to enter the code sent from the service provider
  * Successful screen: A final message to inform successful verification or any additional details

## II - INSTRUCTIONS

After having enough materials, you can either create a template inside a specific Customer Journeys or a template in Media Template. In general, you will have to get through these main steps:

### Step 1 - Create User Registration form

In the **Yes/No view** - the first screen to be displayed to user, there must include an Optin field block serving the purpose of collecting user information. Depending on the OTP Service Provider you connected to, the required form field will be vary.&#x20;

In this example, the service provider will send OTP via SMS, so having a **phone field** is obligatory.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXepEM5bOCSwB59TLxWFxTiulP3hgULmBQmBA2LxclWL8y169Fg-FzIk-cjah_RyBbJ6QFK0ZXyXjMaMTuhhUQ5nzt5rcQ9adpE8_dyayu0nOo4wHG5wojY0N6x87aXn7sUVS2D14O3PstI8kHc9jogOQcr4?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

In the setting of the **Submit** button, you should choose the configuration as below:

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfkHbD8x0mRl-lPwn2UTv9W7ckU0aeopkolmI3WutDhbSUMM-PbYiCdGYqHaAGtMVBwwVxVfn6IRwhrqE4q8hSurSZsOhKavU8IQ_8IoOvCWGKLAcTAY1Wzb2rbzdrIsIhyYAY7noDlpbfgFe_h-XhgBaOL?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

* Button Click Action: Send OTP & Go to View -> After the user click on the button, an OTP will be sent and the screen move to the next view
* Select Provider: Choose the partner that will send OTP to your audience. You can either choose an available one or create a new connection

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfOzBHCftO2fNrIUfAJ6TlCjWk1z2-P5lviOtYb67zDVmwmOumBWVGWTspHQfCBmET-m7DaclGqWMO8F1lDMFyEfaQc3JqVIGT3oOlkz-6Rh_rENE76hR0DZ1CTF5HR_13iKwFpDkhDZlWBzZH_iI7BsRBt?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

To connect with an **OTP Service Provider**, you need to fill in the authentication and necessary details which could be found in the provider platform. The number of character in the OTP & expiration time will be decide the layout of the OTP Verification code.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc3AzBw7kV0fMDBYhDT5KkcRpDdVAOtG_0W354F7UgzBKhyRRYnIegOqf6buJyTpn4uBRiJ4ynnUyXNE3OqKuAJKzHg3S6OoLH5n73GJmM2D3vfz61iBnfXoDu9h6S4b5hblOC1AqWxEalMDldAB1-pk-aL?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

* **Go to View**: Choose the screen to be displayed after the first one. You should choose the view which includes **OTP Verification** form

### Step 2 - Create Identity Verification form

In the **Optin view** - the second screen to be displayed to user, there must include an **OTP Verification** block serving the purpose of collecting & verifying the code sent to audience. To see detailed settings of  the block, read [here](../../marketing-hub/media-template/settings/blocks-and-settings/otp-verification.md).

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdSDMQB3DOkG-CctmgX-vu8wr4yefeMqnYI0JU_qUotisYg3EwyFMhcgd3FtdxjpYYnTwCGIpW49AAFZ1zVPuD5meQ9F4rgyL9ZvfRENQa_LTsE7Ez1XFbr3ZHmCAmNSbRfmC4JZ_C0KZhZFCVoV0_q_sO8?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### Step 3 - Create successful screen

This is the final screen to be appeared after user identification has been verified successfully. The content could be vary depending on your demand and objective.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfsGELdtFhhBHSmh4UEZ8YYxsCTmGetlem7tJPrwOWsz-8AmJT_hLl8hX98BibEFfVzD59Cn7UytpQmCnb4rEcdEDcXiZA4Pxnp7yB21843YAYAnkIPIjh9lUmJTqCGE0ej2zMauoVqSIUOOMu6Yfloxqc?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### Step 4 - Save & Apply the template

If you are designing the template in **Media Templates**, click **Save** to save the template&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfc4yIv64VgqwxK1Vx2rCgW9kTWEcMEiPup6ERd_fZdMD41qs_YHmv5FzObau6UUw1FFWj6jjxhzjffD1jAQBeIiu7CQBZy9CGOXZ8_8kv2Z7Elovms-hAdz0crSSTLgtHE9N0Nq7rwspD02XO80-1jG34?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

If you are designing in the **Customer Journeys**, click **Apply** to save and apply the template to the journey.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd_qstxMAlHVq_bo7xxX2Lgj1BWP4Y_Fx8fyKT4ARuX1qMI5-TeRLaUGeWrn4jcGrzQ6Tj825ig1adA2ASpJcv-XTyl-J816yZkVXXorF99lZjzoS0MOD42UBAP1340c85OaUT7jPvayr_CWXPuzXlCgoA?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

## III - DATA USAGE

When a user information has been verified successfully, an event will be fired. Therefore, you could use this event to categorize the Visitors/ Customers who have legit information in Segment.&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXf3GfEQcM9N-X3B4OuQiYwZWsiZnxQA9FuoEkAsEeC-0k70qEcR0sc3HmZtqLeIMhSng9_8N6re-sV7QNiW5NLzsvQHxFT_mtc7TO-e7SfGdnbrzAVi1hOfImL3ZIPBSp9IQXuo0193HWuVE_bENPX-Wc2K?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

Furthermore, this event could also be used to trigger a journey so that you could implement those post verification marketing scenarios.&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeQVVAypB2fhRzq8Bpq4V9WS1zGYfigSlp0UH1HKuD1aLdoyeJkGE8XqH8OJo0K8YDJWWMsxCaSUsZoMDmM8GWUNe9y0PU2mzpok60eGxxufgNbUeR6houGN-efGgnNLZuCwDw6_Y3Y-Cc4L9cmJNFjUr3v?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

