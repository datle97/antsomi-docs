---
description: >-
  If you're interested in gaining an understanding of the Dataflows feature,
  this document could provide assistance.
---

# Creating a Dataflows

How to navigate to the Dataflows?

For creating a dataflow or managing existing dataflows, please&#x20;

1. Proceed to the Data module&#x20;
2. Then, choose the Batch Stream/Realtime Stream menu.

<figure><img src="../../../.gitbook/assets/image (3561).png" alt=""><figcaption></figcaption></figure>

## How to create your dataflow?

Before creating your dataflows, it's important to have a well-defined understanding of your data requirements. This will enable you to choose the appropriate type of dataflow ([Batch Streaming](./#batch-streaming-dataflows) or [Real-time Streaming](./#real-time-streaming-dataflows)) that aligns with your specific use cases.

Nevertheless, you can only construct a dataflow once you have both the [data source](../../data-source/data-source-connectors/) and [data destination](../../data-destinations/) already established.

The **creation steps** for dataflows **vary significantly** depending on the [**type of dataflow**](./#dataflow-options) you choose.

## Dataflow options

The Dataflows module offers two data transformation options that you can choose based on your requirements.

1. **Batch Streaming**: The option allows you to have data transformed on a **scheduled basis**.
2. **Realtime Streaming**: The option permits data transformation in **real time**.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXccMl1EtszJSPbH7kLs3FNyN2DieBry0o9qG8FIL6KUDlKThhvOyran4-QXpD3QRJlBpIQMYCAGE79tKlF8baWL0OZAjAdJR7YWdKhkI7ohyZKM5bICaMnHJfxP5jivHPqwZitBtfxRC4jlU0dpgq4leC0?key=bWlE_LQFbm2AYaugXff8jA" alt=""><figcaption></figcaption></figure>

For instance,&#x20;

* If you **regularly update** transaction data into CDP 365, opting for a **Batch Streaming** dataflow would be ideal.&#x20;
* However, if you intend to **send order confirmations promptly** after a Messenger message, it is recommended to utilize a **Real-time Streaming** dataflow.

### Batch Streaming Dataflows

* **Step 1:** Choose the Batch Streaming option.&#x20;
* **Step 2:** Then proceed to click on "**Blank Dataflow**".

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdhnq4vZb9VkEoPUDvxGkEpaJaJVvvUA9DOyw2oiqdgSMBpd2syZB6Ikd54h8SZvpdL3LKf4OLp36uvV6eaSdYcoMFoA-WsSFB3dlyJSBQqL-mr6aDWy2_Qts4u-adRoefemZGXRmnlyIc9sJProZ3EFZs?key=bWlE_LQFbm2AYaugXff8jA" alt=""><figcaption></figcaption></figure>

* **Step 3**: Now, please select your data source.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfOY3jKN1G4TwZf-3PnY81dgXn4DktSFD9fI4Oy0CIFDCi9COHZrKrkIiEOtHJqpFEJtLtC6XpVQZuTB3Efz44HQ0p17FQWHSMwkFFBtHXNeGmF2H5OkpHiBcpG4KkM6qvIktBRFkR3moK6IUYtfXfNBpQ?key=bWlE_LQFbm2AYaugXff8jA" alt=""><figcaption></figcaption></figure>

* **Step 4**: Within the dataflow, there are multiple nodes ([action nodes](action-node/) and [destination channels](destination-channel/)) available to assist in the transformation of the input data.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXf_yz6BzAJ_FmtQmeoLF2fxzUwM8MCmiKgEr970S2essisD9KzysgPlJ4v8AAaN_1t-eA3cdIChB2F8lit2hq5k50ZwttjRSULz77NHcTWmE8lJsvsvr-P58eY3n1O9Z6_b4GXt5lpRMf0sVsZJaBypDteJ?key=bWlE_LQFbm2AYaugXff8jA" alt=""><figcaption></figcaption></figure>

_Notes:_

1. _**Action nodes**: Nodes process data in the dataflow._
2. _**Destination channels**: Nodes push data out of the dataflow._

_(_[_An example of the Batch Streaming dataflow_](./#a-batch-streaming-dataflow)_)_

### Real-time Streaming Dataflows

* **Step 1**: Choose the Real-time Streaming option.&#x20;
* **Step 2**: Then proceed to click on either "**Facebook Lead**" or "**Facebook Messenger**" as your chosen data source.&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc7loBMA-kKvmZ2DgY1MVJPCHIQvGVDeici4THNL7d36bBG18d8bZ9A2Jfe_8CETqxaBcnBvktr3XrmBsmn8quch4vx6qt5nZbcF-_w94BfZE-XlluSaJfltAjcd66DDrGgHx29iDf4NGHzTb5WYCXZNCo?key=bWlE_LQFbm2AYaugXff8jA" alt=""><figcaption></figcaption></figure>

* **Step 3**: You can configure your destination channels, which could be either a CDP 365 **event** or a CDP 365 **Business Object**.

<figure><img src="../../../.gitbook/assets/image (3564).png" alt=""><figcaption></figcaption></figure>

_(_[_An example of the Real-time Streaming dataflow_](./#a-real-time-streaming-dataflow)_)_

## Explanation of the Streaming Log tab

While performing data transformations, a dataflow maintains a log. However, it's important to note that the Streaming log for each type of dataflow conveys distinct meanings.

* **In Batch Streaming**: a log documents **the time of data updates** based on the schedule.
* **In Real-time Streaming**: a log keeps track of when **a data record** is updated into CDP 365.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcr5QmO2MScFuYMsa0VvCw4Tq4Arbu3SpPO4k-rkK7BxR-eAwiioQ1yZ5Dr_eSb-xtoO83GxR-4vH0giX_0nBvxpQzx3tNc7JFUe3F6JImJG8insHjJmxotooEV2hDlzlojUoJO9QKS2L_wC9O3HDDn4KQ?key=bWlE_LQFbm2AYaugXff8jA" alt=""><figcaption></figcaption></figure>

For instance,&#x20;

* In the case of a dataflow meant for **routine transaction data updates** of a **Batch Streaming**, the log will document **daily updates**.&#x20;
* On the other hand, for **Real-time Streaming** involving **Facebook Messenger**, the log will record **exchanged messages from your account**.

## An example of a Batch Streaming dataflow

1. **Data source nodes** allow you to configure your data inputs.&#x20;
2. **Action nodes** enable you to define data transformation conditions.&#x20;
3. **Destination channels** are where you configure your data outputs.

In a **Batch Streaming dataflow**, the sequence typically **begins** with one or several **data source** nodes, **followed** by the **action nodes**, and **concludes** with one or several **destination channels**.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfJxIm4XKk-RCeQA95qAilalyQnaHu82KZUFk8zQxX-K-pItf6zIGATjzCWt_rkXzJm7eWc9blyrxzk4Cr8CJfM36uMxdPYiR-xfnCGJKn7ZFfeWjzh3fGJSUnUGUc6qiUWyqE91nbgIq7mIiXdwnEu1mFG?key=bWlE_LQFbm2AYaugXff8jA" alt=""><figcaption></figcaption></figure>

## An example of a Real-time Streaming dataflow

In a **Real-time Streaming dataflow**, you choose **a single data input** and have the option to establish **multiple destination channels**, which can be either events or Business Objects.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd4VKkjhwGPYignli3jVxFt8G-7ZX4Yc5SRN5L5miYtmIrnoUwJ50fmNE63j-js2CUT9cI4EyO5qEuytjxuuke6tONXfvcmTIJjiFHbuESMGBvmbNtGmC-mR72whvJKXNb-0WSFkL3fSmHzP10rdbXZE1Q?key=bWlE_LQFbm2AYaugXff8jA" alt=""><figcaption></figcaption></figure>

## Feature Explanation

### Version History

Every time you save your dataflow, a new version is generated.&#x20;

You can access the Version History to review your past configurations and restore them as needed.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc8II-Qiz5GwBJN9Gi-Hj760BStDRnV6xXovcjd-J8nFaFAsI90T3kMKnMD9nxIGMG2b-ylQIy1Rkr3uCThjG9q-J2JgIjTllNtPTrUDPS8TF2Jca-AjkEpca9rarHCn-YZ2Cw1wdXFxD66jyh_jq83TG8?key=bWlE_LQFbm2AYaugXff8jA" alt=""><figcaption></figcaption></figure>

### Force Run

If you want to **initiate the execution** of your dataflow outside of its scheduled time, click on "Force Run".

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfPsT5Wqjkwh1IYPvP1izr8wlf5o40TV1mM2aqbVEAD3e811K9KmrLoL6JB-36WBipz1W_NNk6jKv1uUkeWYPypcKycIn-6qYYUa1VKMAkKtbttxt0qmadEyOHW5LtJJBtSbXa3Pdtl8ti_mn7xzQr3Zxcs?key=bWlE_LQFbm2AYaugXff8jA" alt=""><figcaption></figcaption></figure>

### Save

When you're ready to save the current settings, simply click on **Save**.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd9Zw6WQdrXft8aUs-J1ze6iy3ajD4YaJgPDOKXMZnuhq-F-8iibtj_5722SKy8g3VsOxqUiAEOKxvcERn6HiOlEXxMPYmDs6UPC7pM48x-LUvPiBDtf0C33xYD4w74v5tMhPBXfaFOkP2Al59Pe9JSpR0i?key=bWlE_LQFbm2AYaugXff8jA" alt=""><figcaption></figcaption></figure>

### Activate&#x20;

To activate your dataflow, click on **Activate**.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeAgXh2baVTN5Yu5NHXuy1ShtZafy7_PdIOA-blCJfJuIgZtVPT3HKqc9SBFoZmeoWcxLFJM2lUHVRMzMPSvFAZ9d_c9s0SQ_FF35q3zFEjPW3UcuKTCE9NJskjPt4NfixnF_crs8SGRLUnxwxxzhIYSEdT?key=bWlE_LQFbm2AYaugXff8jA" alt=""><figcaption></figcaption></figure>
