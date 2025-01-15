# How to push notification using Antsomi Web Push in CDP 365?

Antsomi Web Push destination allows Antsomi to send web-push notification on you website. To do so, follow the instruction below:

<figure><img src="../../.gitbook/assets/image (540).png" alt=""><figcaption></figcaption></figure>

## STEP 1 - Create Antsomi Web Push destination

### 1. Log in to **CDP 365**. Hover your mouse over **Settings**. Choose **Channel Integration**.

<figure><img src="../../.gitbook/assets/image (3302).png" alt=""><figcaption></figcaption></figure>

### 2. Click ![](<../../.gitbook/assets/image (896).png>) button and select Web Push

<figure><img src="../../.gitbook/assets/image (3303).png" alt=""><figcaption></figcaption></figure>

### 3. Choose the Destination Catalog: Antsomi Web Push.&#x20;

{% hint style="info" %}
You could create ONLY one Antsomi Web Push destination. "Antsomi Web Push" option will disappear if you already created one.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (3304).png" alt=""><figcaption></figcaption></figure>

Then **fill in the necessary information** for the destination.

<figure><img src="../../.gitbook/assets/image (3306).png" alt=""><figcaption></figcaption></figure>

#### General Information

* **Destination name:** Input destination name. Destination name can be entered in multiple languages. This is required field.
* **Description:** Input destination description. Destination description can be entered in multiple languages. This is optional field.
* **Destination catalog:** In the dropdown list, select **Antsomi Web Push**.
* **Method:** Select **Push** in the dropdown list

#### **Configuration**

After filling General Information, the screen will display the Configuration of this destination as below

<figure><img src="../../.gitbook/assets/image (3308).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (3311).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (3312).png" alt=""><figcaption></figcaption></figure>

Follow the below instructions to complete the configuration:

**1. General Information:** The descriptive fields for this destination

**2. Configure fields:** Choose audiences who will receive the web-push notification. For this destination, follow below steps to choose _**antsomi webpush uid**_ attribute in _**Visitor**_**&#x20;Data Object**.

* Click on icon personalization<img src="../../.gitbook/assets/image (1888).png" alt="" data-size="line">
* After clicking on the icon, pop up **Add Personalization** is displayed as shown below. Select the appropriate information.

<figure><img src="../../.gitbook/assets/image (3313).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**antsomi\_webpush\_uid** may have different name but the internal code must be **antsomi\_webpush\_uid**
{% endhint %}

#### 3. Site Setup

<figure><img src="../../.gitbook/assets/image (3314).png" alt=""><figcaption></figcaption></figure>

**Site name:** Input website name. This is required field. The default name to call your site used in push notifications.

**Site URL:** Input website URL. This is required field. Your website URL including:&#x20;

* `http://` or `https://`
* `www` or non-www links (e.g. `https://example.com`, `https://www.example.com`)

**Auto Re-subscribe (HTTPS Only):** Allows push subscribers to automatically re-subscribe upon returning to your site without being prompted if they clear their browser data

**Default Icon URL:**&#x20;

* Icon used for the [Slide Prompt](how-to-push-notification-using-antsomi-web-push-in-cdp-365.md#2.4.4.-permission-prompt-setup) and default for push notifications.
* Enter an `https` icon URL or upload file that is square `256x256` pixels.
* The file must be `.png`, `.jpg`, or `.gif`.

#### 4. **Permission Prompt Setup**

* This section allows you to set up the permission and frequency to prompt the notification. To edit Permission, click on ![](<../../.gitbook/assets/image (1498).png>) and adjust the setting in the pop-up appeared.

<figure><img src="../../.gitbook/assets/image (3315).png" alt=""><figcaption></figcaption></figure>

**Prompt type**

**Push Slide Prompt**

_a. Customize Slide Prompt Text:_ Turn it on to edit the content of your notification

_b. Auto Prompt:_ Customize the time to show the notification.

* Show after: Show the notification after {x} amount of a page is viewed/loaded on the screen
* And delay: Show the notification {x} seconds after user visits the amount of page adjusted above

_c. Auto Repeat after click on Later:_ Adjust the time to show the notification again if user click Button 1 (Later)&#x20;

_d. Categories:_ This feature allows you to add many checkbox options in the notification so you could the categories to be presented to the audience. After clicking _Positive button,_ the selected options will be recorded.

<figure><img src="../../.gitbook/assets/image (3316).png" alt=""><figcaption></figcaption></figure>

* Label: The description of the option
* Tag Key: The name of the option to be recorded in the data
* Update instructions: Input the new instructions for the notification
* Positive button: Input the text of the button which will record the data after user click
* Negative button: Input the text of the button which will skip the notification

#### 5. Welcome Notification

Customize a push notification which is sent immediately to current user upon subscribing to your site for the first time.

<figure><img src="../../.gitbook/assets/image (3317).png" alt=""><figcaption></figcaption></figure>

* **Title:** The title of the notification
* **Message:** The content of the notification
* **Link:** Enter a landing page you want to direct user after clicking on the notification

#### **6. Advanced Push Settings (Optional)**

<figure><img src="../../.gitbook/assets/image (3321).png" alt=""><figcaption></figcaption></figure>

**Click Behaviour**

Supports several different possible browser behaviors when users click on your notifications.

{% hint style="info" %}
Support: Chorme, Firefox, Safari (on mobile only support Safari version greater than 16.3.1)
{% endhint %}

If users **do not have your site open on any browser tabs**, and click on a notification that takes them to your site, the browser will open a new tab and navigate to the notification's URL.

If users **have your site open on one or more browser tabs**, and click on a notification that takes them to your site, there are several possible ways the browser can behave that you can configure:

* **Exact Navigate** (default) - If the notification's exact URL (e.g. `example.com/product`) matches a tab that the browser already has open, the browser will navigate to the notification's URL in that tab.
* **Origin Navigate** - If the notification's origin (e.g. `example.com`) matches a tab that the browser already has open, the browser will navigate to the notification's URL in that tab.
* **Exact Focus** - If the notification's exact URL (e.g. `example.com/product`) matches a tab that the browser already has open, the browser will focus on that tab, but _not_ refresh the page.
* **Origin Focus** - If the notification's origin (e.g. `example.com`) matches a tab that the browser already has open, the browser will focus on that tab, but _not_ refresh the page

**Website Tracking Script**

* This script is used to attach to the source of the website to push notifications

### 4. Click&#x20;

### Save to finish creating the Antsomi Web Push destination

<figure><img src="../../.gitbook/assets/image (3320).png" alt=""><figcaption></figcaption></figure>

## STEP 2 - Attach Website Tracking Script of Antsomi Web Push Destination to Website Source&#x20;

Copy this tracking script and paste into your website's `<head>`

<figure><img src="../../.gitbook/assets/image (3322).png" alt=""><figcaption></figcaption></figure>

## STEP 3 - Add service workers for the website.

* The sw.js file must be publicly accessible and can be placed at the top-level root of your site.
* If sw.js file already exists then add below script to file:

```
importScripts('https://st-a.cdp.asia/antsomiSDKsw.js');
```

## STEP 4 - Create Visitor Subscribed Segment

### 1. Hover your mouse over Profiles and go to the Segments menu

<figure><img src="../../.gitbook/assets/image (3323).png" alt=""><figcaption></figcaption></figure>

### 2. Click <img src="../../.gitbook/assets/image (1401).png" alt="" data-size="line"> button and select Visitor Segment

<figure><img src="../../.gitbook/assets/image (3324).png" alt=""><figcaption></figcaption></figure>

### 3. Fill in the necessary information for the segment <a href="#id-4.-fill-in-the-necessary-information-for-the-destination" id="id-4.-fill-in-the-necessary-information-for-the-destination"></a>

Fill in the necessary information for the segment.

Condition: The attribute record subscriber ID (example: antsomi webpush uid) is exists.

<figure><img src="../../.gitbook/assets/image (3326).png" alt=""><figcaption></figcaption></figure>

### 4. Click Save to finish creating the Visitor Subscribed segment

<figure><img src="../../.gitbook/assets/image (3327).png" alt=""><figcaption></figcaption></figure>

## STEP 5 - Pushing notification using Antsomi Web Push via Customer Journey

* Log into **CDP 365** system. Hover your mouse over **Marketing** and go to **All Channels** menu.

<figure><img src="../../.gitbook/assets/image (3328).png" alt=""><figcaption></figcaption></figure>

*   We have 2 channels that supporting to send:

    * Web Push
    * Orchestration



    <figure><img src="../../.gitbook/assets/image (3329).png" alt=""><figcaption></figcaption></figure>
* Click on <img src="../../.gitbook/assets/image (768).png" alt="" data-size="line"> to create journey.

<figure><img src="../../.gitbook/assets/image (3330).png" alt=""><figcaption></figcaption></figure>

* In **Schedule trigger node**, **Include Audience** section, select **Visitor Segment** then choose **Visitor subscribed** segment has created.

<figure><img src="../../.gitbook/assets/2024-08-08_15-05-11.gif" alt=""><figcaption></figcaption></figure>

* Add **Destination** node and select **Antsomi Web Push** destination

<figure><img src="../../.gitbook/assets/image (3301).png" alt=""><figcaption></figcaption></figure>

* Select the **Antsomi Web Push** destination that you have created before

<figure><img src="../../.gitbook/assets/image (3332).png" alt=""><figcaption></figcaption></figure>

* Fill out necessary information

<figure><img src="../../.gitbook/assets/image (3333).png" alt=""><figcaption></figcaption></figure>

* Click **Save** button to finish setting journey

<figure><img src="../../.gitbook/assets/image (3334).png" alt=""><figcaption></figcaption></figure>

After finishing the setting, we can click **activate** to start running the journey.
