# Collect data from TikTok Form to CDP 365

## I - Introduction

During your marketing journey, there will be time you want to enrich your customer data to better understand you audience and propose appropriate caring services. In order to do so, collecting leads through survey and form and then push to CDP 365 is significant.&#x20;

In this article, we will instruct step by step on how to connect with TikTok Form and collect data from it.

Before doing as instructions, there are some prerequisites you need to prepare:

*   The TikTok Form that you created on TikTok ads. For example:



    <figure><img src="../../.gitbook/assets/image (173).png" alt=""><figcaption></figcaption></figure>
* The information of Event & Event Attributes or Business Objects & Attributes you want to sync the data to **CDP 365** with. For example:&#x20;
  * Submit Lead event with event attributes: Id, Name, Email, Lead Source & sync to BO Lead
  * BO Customers with attributes: Customer ID, Name, Email, Sex Gender, is Tiktok

{% hint style="info" %}
You can create a new attribute for the data to be sent to if the current ones don’t meet your requirements.&#x20;

See the article on how to create:

* Event attributes
* Attributes
{% endhint %}

## II - DETAILS INSTRUCTION

In general, you will have to move through these steps:

[Step 1 - Create a Data Source](collect-data-from-tiktok-form-to-cdp-365.md#step-1-create-a-data-source)

[Step 2 - Create a Data Destination (Optional)](collect-data-from-tiktok-form-to-cdp-365.md#step-2-create-a-data-destination)

[Step 3 - Create a Data Flow](collect-data-from-tiktok-form-to-cdp-365.md#step-3-create-a-dataflow)

***

### STEP 1 - Create a Data Source

A data source is where you get the data from. In this case, it’s the form distributed on Tiktok.

* Hover your mouse over **Data** >> Choose **Source**, then click on <img src="https://lh7-us.googleusercontent.com/Xq1LLeEiAeaUqN2qsHAcozvF3UslLWa0QilDN0RPmGij4wPP4_BWc-4stsmEl1Mjpyc25WLnbVPVYZLKBGpvaDTChG8Op0g84LXF6IvyEWUtyMqrLivmn-gZKZH0F6CExC_2_W7OzugX1dNaG67m95o" alt="" data-size="line"> and select the Realtime option.

<figure><img src="../../.gitbook/assets/image (3452).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (3453).png" alt=""><figcaption></figcaption></figure>

* Select an account to be the owner of the Data Source (This only applies to accounts having Super Admin role).

<figure><img src="../../.gitbook/assets/image (3455).png" alt=""><figcaption></figcaption></figure>

* Select **TikTok Lead** as the connector. You can also name the data source.

<figure><img src="../../.gitbook/assets/image (3456).png" alt=""><figcaption></figcaption></figure>

* **Authenticate** your TikTok account for lead generation forms by signing in and clicking on **Confirm**.

<figure><img src="../../.gitbook/assets/image (3457).png" alt=""><figcaption></figcaption></figure>

* Select the **owner account of the TikTok Form** in Ad Accounts -> click **Get Forms**.&#x20;

<figure><img src="../../.gitbook/assets/image (3458).png" alt=""><figcaption></figcaption></figure>

Then select the TikTok form -> click on **Next**

<figure><img src="../../.gitbook/assets/image (3459).png" alt=""><figcaption></figcaption></figure>

* &#x20;Go over to confirm the fields in the form that you want to sync data to CDP 365 -> click on **Next** to finish creating a data source.

<figure><img src="../../.gitbook/assets/image (3460).png" alt=""><figcaption></figcaption></figure>

Decide who you want to share this Data Source with, then click **Save**.

<figure><img src="../../.gitbook/assets/image (3461).png" alt=""><figcaption></figcaption></figure>

### STEP 2 - Create a Data Destination

This step is optional because you could also create a Data Destination in a Dataflow. For Realtime Streaming flow, there are 2 types of Data Destinations will be used:

* Events Destination
* Business Objects Destination

### STEP 3 - Create a Dataflow

Every time an audience submit the form, the data will be captured and sent to CDP 365 in the real time, so the flow belongs to **Realtime Streaming** category

* Hover your mouse over Data >> Choose **Realtime Stream**

<figure><img src="../../.gitbook/assets/image (3462).png" alt=""><figcaption></figcaption></figure>

Click **+** button, choose **TikTok Lead** template, and click **Continue**

<figure><img src="../../.gitbook/assets/image (3463).png" alt=""><figcaption></figcaption></figure>

* The interface of a Realtime Streaming dataflow is different from the Batch one, but at the end, it still provides the same functions, typically:

<figure><img src="../../.gitbook/assets/image (3474).png" alt=""><figcaption></figcaption></figure>

#### **1. Select the Data Source**

* Select a TikTok Lead Source that was created before to be the data input

<figure><img src="../../.gitbook/assets/image (3464).png" alt=""><figcaption></figcaption></figure>

#### 2. Select and adjust the Data Destination

<figure><img src="../../.gitbook/assets/image (3475).png" alt=""><figcaption></figcaption></figure>

#### **2.1 - Streaming Destination**

* Choose where your data would be pushed to. By default, there is one destination of Submit Lead event  with chosen Event Attributes, you could customize it according to your demand or create a new destination which can be another Event or Business Object by clicking on **Add Destination.**
* Depending on the option you choose, the pop-up will display the list of Data Destination accordingly. If you have not created the desired Data Destination before (In step 2), you could click the button + Create new Event Destination / + Create new Business Object Destination to make a new one. The steps you need to get through would be the same in Step 2 (<img src="../../.gitbook/assets/image (172).png" alt="" data-size="line">)

<figure><img src="../../.gitbook/assets/image (3476).png" alt=""><figcaption></figcaption></figure>

#### 2.2 - Configure the chosen Data Destination

Depending on the type of Data Destination, the configuration fields will display accordingly, typically:

* <mark style="color:blue;">**Event Destinations**</mark>

<figure><img src="../../.gitbook/assets/tiktok form - 2.gif" alt=""><figcaption></figcaption></figure>

* **Event Source:** Choose the Source where an event happened. To read more details about Event Source, click here
* **Event Name:** Choose the event you want to sync the data to. To read more details about Event, click here

-> After choosing the Event, it will appear a list of Event attributes & Business Objects that have been assigned to this event, so you could choose the objects you want and  map its attributes in [2.3 ](collect-data-from-tiktok-form-to-cdp-365.md#2.3-mapping-the-attributes-on-cdp-365-with-the-column-on-tiktok)area

<figure><img src="../../.gitbook/assets/image (3478).png" alt=""><figcaption></figcaption></figure>

*   <mark style="color:blue;">**Business Objects Destination**</mark>

    * **Business Objects:** Choose the Business Objects you want & map its attribute in [2.3](collect-data-from-tiktok-form-to-cdp-365.md#2.3-mapping-the-attributes-on-cdp-365-with-the-column-on-tiktok) area

    <figure><img src="../../.gitbook/assets/tiktok form - 1.gif" alt=""><figcaption></figcaption></figure>

#### 2.3 - Map the attributes on CDP 365 with the column on TikTok

* Source column: The column from the data in the TikTok Form such as Form name, Ad id, etc and the information fields from the Form.

<figure><img src="../../.gitbook/assets/image (3479).png" alt=""><figcaption></figcaption></figure>

* Hash: To choose whether the data be hashed to provided algorithms or not

<figure><img src="../../.gitbook/assets/image (3480).png" alt=""><figcaption></figcaption></figure>

* Destination column: The column which will receive the data&#x20;

<figure><img src="../../.gitbook/assets/image (3481).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Each Business Object has its own required fields, so make sure you add it and map Source Column with Destination Column. If not, the data could not be pushed to the Business Object.

For example: **Name** and **ID** are required fields for BO Lead, Visitor, Customer, please also add and map Source Column with Destination Column for ID.&#x20;
{% endhint %}

After mapping the column, it should look like this

<figure><img src="../../.gitbook/assets/image (3482).png" alt=""><figcaption></figcaption></figure>

#### 3. Functional buttons

<mark style="color:blue;">**Save & Turn on**</mark>

* Click **Save** to save the changes made in the dataflow
* Click **Activate** to actually run the dataflow and start to record the data

<figure><img src="../../.gitbook/assets/image (3483).png" alt=""><figcaption></figcaption></figure>

<mark style="color:blue;">**Version History**</mark>

<mark style="color:blue;">**Bulk Process**</mark>

## III - INSPECTION

After having created the dataflow, you could test it by doing these following steps:

### Step 1 - Submit the TikTok Form

You could either submit the real form or make a demo by doing as below:

<figure><img src="../../.gitbook/assets/2023-12-03_15-53-29.gif" alt=""><figcaption></figcaption></figure>

### Step 2 - Check on CDP 365 data

After submitting the form, the data will be immediately pushed to CDP 365, you could check on these 3 objects:

#### 1. Streaming Log

The running process of the dataflow you just created. If it were success, the data has been pushed to the desired destinations.

<figure><img src="../../.gitbook/assets/image (3485).png" alt=""><figcaption></figcaption></figure>

#### 2. Event

In the dataflow, if there were an **Event Destination**, you could go to **Event log** of that Event to check up.

<figure><img src="../../.gitbook/assets/image (3486).png" alt=""><figcaption></figcaption></figure>

#### 3. Business Object

In the dataflow, if there were a **Business Object** Destination, you could go to **Data Table** tab of the specific Data Object

<figure><img src="../../.gitbook/assets/image (3450).png" alt=""><figcaption></figcaption></figure>
