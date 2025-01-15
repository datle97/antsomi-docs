# How to push notification using "Onesignal (App Push)" in CDP 365

### 1. Hover your mouse over Settings and go to the Channel Integration menu

<figure><img src="../../.gitbook/assets/image (3260).png" alt=""><figcaption></figcaption></figure>

### 2. Click + button and select App Push

<figure><img src="../../.gitbook/assets/image (3261).png" alt=""><figcaption></figcaption></figure>

### 3. Select Destination catalog: Onesignal (App Push)

<figure><img src="../../.gitbook/assets/image (3344).png" alt=""><figcaption></figcaption></figure>

### 4. Fill in the necessary information for the destination <a href="#id-4.-fill-in-the-necessary-information-for-the-destination" id="id-4.-fill-in-the-necessary-information-for-the-destination"></a>

<figure><img src="../../.gitbook/assets/image (3264).png" alt=""><figcaption></figcaption></figure>

| Field          | Description                                                                                                                                                                                                            |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| App ID         | ​[Get your App ID and secret key](https://app.gitbook.com/o/-LzunofLVjpTa_-p1PQt/s/mECwNqMNUmu6OXHSYgDv/quick-start-guide/how-to-push-notification-using-onesignal-app-push-in-cdp-365#get-your-app-id-and-secret-key) |
| App Secret Key | [Get your App ID and secret key](how-to-push-notification-using-onesignal-app-push-in-cdp-365.md#get-your-app-id-and-secret-key)                                                                                       |
| User Id        | <p>Click <img src="../../.gitbook/assets/image (456).png" alt=""> icon to add Personalization. </p><p><img src="../../.gitbook/assets/image (3263).png" alt="" data-size="original"></p>                               |

#### **Get your App ID and secret key**

1. Login OneSignal [https://app.onesignal.com/login](https://app.onesignal.com/login)

&#x20; 2\. On the navigation menu, choose **Settings -> Keys & IDs**

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2F6qyuU9QcoDmkBalmd8T4%2Fimage.png?alt=media&#x26;token=265bc2dd-3037-413e-96fa-baebad0705b1" alt=""><figcaption></figcaption></figure>

### 5. Click Save to finish creating the OneSignal (App Push) destination

<figure><img src="../../.gitbook/assets/image (3265).png" alt=""><figcaption></figcaption></figure>

### 6. Pushing notification using OneSignal App Push via Customer Journey

Log into CDP 365 system,  hover your mouse over **Marketing** and go to **All Channels** menu.

<figure><img src="../../.gitbook/assets/image (3266).png" alt=""><figcaption></figcaption></figure>

We have 2 channels that supporting to send:

* App Push
* Orchestration

<figure><img src="../../.gitbook/assets/image (3267).png" alt=""><figcaption></figcaption></figure>

Click **+** button to Create Journey, add **Destination** node and select **OneSignal (App Push)** destination

<figure><img src="../../.gitbook/assets/image (3268).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (3345).png" alt=""><figcaption></figcaption></figure>

Choose **Design from scratch** if you do not have existing design.&#x20;

<figure><img src="../../.gitbook/assets/image (3270).png" alt=""><figcaption></figcaption></figure>

Select the **OneSignal (App Push) destination** that you have created before

<figure><img src="../../.gitbook/assets/image (3271).png" alt=""><figcaption></figcaption></figure>

Fill out necessary information

<figure><img src="../../.gitbook/assets/image (3346).png" alt=""><figcaption></figcaption></figure>

Click **Save** button to finish setting journey

<figure><img src="../../.gitbook/assets/image (3347).png" alt=""><figcaption></figcaption></figure>

After finishing the setting, we can click **activate** to run the journey to send **OneSignal App Push** to audience.
