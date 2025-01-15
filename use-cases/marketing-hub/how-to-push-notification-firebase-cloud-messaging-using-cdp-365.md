# How to push notification "Firebase Cloud Messaging" using CDP 365

## I. Create a Firebase project

### 1. Create a project

#### - Log in [Firebase](https://console.firebase.google.com/) and create a new project

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FCBTUiyLEWSYPpTPizsHZ%2Fimage.png?alt=media&#x26;token=3a265353-ff69-4302-ae94-1737fc6b0846" alt=""><figcaption><p>Add new project</p></figcaption></figure>

#### - Enter the name of project and click "Continue"

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FjV9YKSQO8qGr8NzAapvc%2Fimage.png?alt=media&#x26;token=0fe128f2-af56-414f-99ce-4fc038797c5a" alt=""><figcaption><p>Enter Name of project</p></figcaption></figure>

#### - Accept the privacy and create project

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FprXDPLrEA3hLQDswyvIE%2Fimage.png?alt=media&#x26;token=1a59fdad-de43-492f-853b-7eff08616827" alt=""><figcaption><p>Create project</p></figcaption></figure>

### 2. Build "Cloud Messaging"

#### - Click dropdown "Build" and select "Cloud Messaging"

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FGthxeUJPF7GTUo34SAAQ%2Fimage.png?alt=media&#x26;token=69134f7b-5135-4395-ae17-2e071941c52d" alt=""><figcaption><p>Cloud Messaging</p></figcaption></figure>

#### - Add firebase to your web app

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FvlQDFOQBu7TG7IFOJ3jA%2Fimage.png?alt=media&#x26;token=c8f3a4ec-6708-40e9-a9f9-6fd0ba509666" alt=""><figcaption><p>Add firebase to web app</p></figcaption></figure>

#### - Click "Register app" <a href="#click-register-app" id="click-register-app"></a>

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FFPboyZ9tTmlyeWUU5BxA%2Fimage.png?alt=media&#x26;token=bc5735b2-a614-4578-8900-ad437d0d91c1" alt=""><figcaption><p>Register app</p></figcaption></figure>

#### - Copy "firebaseConfig" and Click "Continue to console"

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FVQnSw52KlNMMFlsqua10%2Fimage.png?alt=media&#x26;token=d5b3b20d-cb33-4ae8-a7d1-4fe378ed6460" alt=""><figcaption><p>Continue to Console</p></figcaption></figure>

#### - Firebase config:

```
apiKey: "AIzaSyBUJrgxGjFUWld-q_zr_cVzrN9IaB4KfmE",
  authDomain: "fir-clound-messaging-ab666.firebaseapp.com",
  projectId: "fir-clound-messaging-ab666",
  storageBucket: "fir-clound-messaging-ab666.appspot.com",
  messagingSenderId: "974234323980",
  appId: "1:974234323980:web:03d23bee74ed48eb5c7229",
  measurementId: "G-EE955NEBKJ"
```

#### - Click settings icon and select "Project settings"

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FRL59cIY0kufLEjkmzL0d%2Fimage.png?alt=media&#x26;token=ac7cd7cf-70e8-4711-97f3-f820302c09a1" alt=""><figcaption><p>Project settings</p></figcaption></figure>

#### - Click "Cloud Messaging"

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2Fy3MRDSspMP2jzGy5q7Hi%2Fimage.png?alt=media&#x26;token=c36e0b65-200b-4a0d-ad23-1a06368047b4" alt=""><figcaption><p>Cloud Messaging settings</p></figcaption></figure>

#### - Enable Cloud Messaging API

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FQLrIKIEAZhxBCmgSqED0%2Fimage.png?alt=media&#x26;token=b8b19a06-74c1-486a-9e1d-a7484b7cc750" alt=""><figcaption><p>Manage API</p></figcaption></figure>

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FIS3BhSLU8INTSOPVtryB%2Fimage.png?alt=media&#x26;token=f8f6dd40-0761-4f54-9fae-dc57d22b8bb4" alt=""><figcaption><p>Click Enable</p></figcaption></figure>

#### - After that, we have the data of Server Key

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FFYgMQBAgOmY3u0kOWo7Z%2Fimage.png?alt=media&#x26;token=378a14d8-4a7d-48c6-bebb-f55fa0a827d2" alt=""><figcaption><p>Server Key</p></figcaption></figure>

### 3. Add script to source code of website

#### - Copy and paste these scripts into the bottom of your \<body> tag

```
<!-- The core Firebase JS SDK is always required and must be listed first -->
    <script src="https://www.gstatic.com/firebasejs/7.16.1/firebase-app.js"></script>
    <!-- TODO: Add SDKs for Firebase products that you want to use https://firebase.google.com/docs/web/setup#available-libraries -->
    <script src="https://www.gstatic.com/firebasejs/7.16.1/firebase-analytics.js"></script>
    <script src="https://www.gstatic.com/firebasejs/7.16.1/firebase-messaging.js"></script>
    <script>
      // Your web app's Firebase configuration
      // For Firebase JS SDK v7.20.0 and later, measurementId is optional
      var firebaseConfig = {
        *firebaseConfig*
      };
      // Initialize Firebase
      firebase.initializeApp(firebaseConfig);
      firebase.analytics();
      const messaging = firebase.messaging()
      navigator.serviceWorker.register('firebase-messaging-sw.js')
      .then((register) => {
        messaging.requestPermission().then(() => {
          messaging.getToken()
          .then((fcmToken) => {
            console.log(fcmToken)
            messaging.onMessage((payload) => {
              console.log("onMessage event fired",payload)
            })
          });
        });
      })
    </script>
```

#### - Add file in source firebase-messaging-sw.js (located in public/global folder)

```
importScripts('https://www.gstatic.com/firebasejs/7.16.1/firebase-app.js');
importScripts('https://www.gstatic.com/firebasejs/7.16.1/firebase-messaging.js');

  var firebaseConfig = {
      *firebaseConfig*
  };// Initialize Firebase
  firebase.initializeApp(firebaseConfig);
  const messaging = firebase.messaging();
  messaging.onBackgroundMessage((payload) => {
    console.log('[firebase-messaging-sw.js] Received background message ', payload);
    const notificationTitle = payload.notification.title;
    const notificationOptions = {
      body: payload.notification.body,
    };
    return self.registration.showNotification(notificationTitle, notificationOptions);
  });
  self.addEventListener('notificationclick', event => {
     console.log(event)
  });
```

#### - \*firebaseConfig\* is the data of [firebase config](how-to-push-notification-firebase-cloud-messaging-using-cdp-365.md#firebase-config) in section 2

## II. Create destination "Firebase Cloud Messaging"

### 1. Hover your mouse over Settings and go to the Channel Integration menu

<figure><img src="../../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

### 2. Click + button and select Web Push

<figure><img src="../../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

### 3. Select Destination catalog: Firebase Cloud Messaging

<figure><img src="../../.gitbook/assets/image (3294).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>

* **Server Token**: we can copy server token as instruction in [previous section](how-to-push-notification-firebase-cloud-messaging-using-cdp-365.md#after-that-we-have-the-data-of-server-key)

#### - Get To Client Tokens

* Visit the website, press F12 and go to Console to get **To Client Tokens**

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2F6qWu38iOigvHOjYsCqMa%2Fimage.png?alt=media&#x26;token=62dd5fba-5d9e-47bb-b4f2-a2c375ef7ab2" alt=""><figcaption><p>To Client Tokens</p></figcaption></figure>



* Copy **To Client Tokens** and paste to destination setting
* Click **Save** to save destination

#### Note: After client finish creating Firebase Cloud Messaging, Antsomi team will collect the data and update To Client Tokens attribute in CDP system.

## III. Push "Firebase Cloud Messaging" notification via Journey

### 1. Hover your mouse over Marketing and go to All Channels menu

<figure><img src="../../.gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>

* We have 2 channels that supporting to send **Firebase Cloud Messaging**. These are **Web Push** and **Orchestration**

<figure><img src="../../.gitbook/assets/image (43).png" alt=""><figcaption></figcaption></figure>

### 2. Click + button to Create Journey, add Destination node and select Firebase Cloud Messaging destination

<figure><img src="../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (3295).png" alt=""><figcaption></figcaption></figure>

* Fill in the required information

<figure><img src="../../.gitbook/assets/image (46).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (47).png" alt=""><figcaption></figcaption></figure>

* Click **Save** to finish

### 3. Click Activate to activate the journey

<figure><img src="../../.gitbook/assets/image (48).png" alt=""><figcaption></figcaption></figure>
