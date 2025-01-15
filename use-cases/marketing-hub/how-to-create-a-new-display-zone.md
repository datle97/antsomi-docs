# How to create a new "Display Zone"

### 1. Hover your mouse over Settings and go to the Web Personalize menu

<figure><img src="../../.gitbook/assets/image (3218).png" alt=""><figcaption></figcaption></figure>

### 2. Click + to create a Display Zone

<figure><img src="../../.gitbook/assets/image (3219).png" alt=""><figcaption></figcaption></figure>

### 3. Input the necessary information to create a Display Zone

<figure><img src="../../.gitbook/assets/image (3220).png" alt=""><figcaption></figcaption></figure>

| Field             | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| ----------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Display Zone name | Input the name that you want                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| Domain            | Input your website domain                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Zone Code         | Code of new Zone is automatically added by the system but you can edit it                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Zone type         | <p><strong>Get Zone script:</strong> After creating Zone successfully, the system will generate Zone script. Put this Zone script in the position where you want to display the ad on the website. You can see how to get the Zone script <a href="how-to-create-a-new-display-zone.md#get-the-zone-script">here</a>.</p><p><strong>Use CSS Selector:</strong> Input Class or ID of the div tag where you want to show the Ad. You can see how to get the class or id <a href="how-to-create-a-new-display-zone.md#get-id-or-class-on-the-websites">here </a></p><p><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2F1E5YKf2YaoiPtSSD0wMt%2Fimage.png?alt=media&#x26;token=39dbbde7-8e4d-4a54-bad1-686a2de260b7" alt="" data-size="original"></p><p></p> |

### 4. After filling in the info, click Save button to finish creating the Display Zone

<figure><img src="../../.gitbook/assets/image (3229).png" alt=""><figcaption></figcaption></figure>

### **Get the Zone script**

1. Hover your mouse over **Settings** -> Choose **Web Personalize**
2. At the Display Zone listing, hover your mouse over the zone you want to get the script -> Click ![](<../../.gitbook/assets/image (1085).png>) icon

<figure><img src="../../.gitbook/assets/image (3230).png" alt=""><figcaption></figcaption></figure>

&#x20;   3\.  Click **Copy to clipboard** to copy your Zone Script

<figure><img src="../../.gitbook/assets/image (3231).png" alt=""><figcaption></figcaption></figure>

### **Get id or class on the Website**

1. Go to your website
2. Press **F12 (or Fn + F12)** to open **Developer Tools**
3. Click ![](<../../.gitbook/assets/image (2601).png>) icon

<figure><img src="../../.gitbook/assets/image (3226).png" alt=""><figcaption></figcaption></figure>

&#x20;  4\.  Find the location where you want to display the Ad, then click on that location to display **id** or **class**

For example:

<figure><img src="../../.gitbook/assets/image (3228).png" alt=""><figcaption></figcaption></figure>

&#x20;   5\.  Copy the **id** or **class** into the **Create Display Zone** interface.&#x20;

&#x20;   **NOTE:**&#x20;

&#x20;        **+** Add **"#"** in front of the **id** (Example: #maincontent)

&#x20;        **+** Add **"."** in front of the **class** (Example: .page-main)

&#x20;   **For example:**&#x20;

<figure><img src="../../.gitbook/assets/image (3232).png" alt=""><figcaption></figcaption></figure>

**Note: If there are many classes in a div tag, you must replace the space with a "."**

<figure><img src="../../.gitbook/assets/image (3234).png" alt=""><figcaption></figcaption></figure>

**Get the "CSS selector" - this way is used when the class names are duplicated in many places on this page**

&#x20; \- Right click on the div tag -> Copy -> Copy selector

<figure><img src="../../.gitbook/assets/image (3235).png" alt=""><figcaption></figcaption></figure>

Paste the content you just copied into the **CSS Selector** field in the **Create Display** zone interface

<figure><img src="../../.gitbook/assets/image (3236).png" alt=""><figcaption></figcaption></figure>

**In case the level of div is not determined, you can use the following way:**

**Code example:**

```
<div class="class-cha class-cha-02">
  <div class="class-con class-con-02">
    <div class="class-chau class-chau-02"></div>
  </div>
</div>
```

Like the above example, there are ways to get the **"**&#x63;lass-chau" div

1. .class-cha.class-cha-02 > .class-con > .class-chau
2. .class-cha.class-cha-02 .class-chau

#### Locate class or id on the website

1. Go to your website
2. Press **F12 (or Fn + F12)** to open **Developer Tools**
3. Press **Ctrl + F** to open search box at **Elements** tab

<figure><img src="../../.gitbook/assets/image (3237).png" alt=""><figcaption></figcaption></figure>

&#x20;   4\.  Input id or class that you want

&#x20;  5\.  Search results will be highlighted, hover over the search results to see the location on the website&#x20;

<figure><img src="../../.gitbook/assets/image (3238).png" alt=""><figcaption></figcaption></figure>
