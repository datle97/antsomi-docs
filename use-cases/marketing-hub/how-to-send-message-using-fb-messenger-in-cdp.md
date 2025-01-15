# How to send message using "FB Messenger" in CDP

## I. Create a new Data source to get the list of users who have sent messages to your page

### 1. Hover your mouse over Data on the left hand side menu and choose Sources

<figure><img src="../../.gitbook/assets/image (3170).png" alt=""><figcaption></figcaption></figure>

### 2. Click + button to create a new Data source

For Facebook Messenger, choose **Realtime**.

<figure><img src="../../.gitbook/assets/image (3171).png" alt=""><figcaption></figcaption></figure>

### 3. Select Facebook Messenger connector

<figure><img src="../../.gitbook/assets/image (3172).png" alt=""><figcaption></figcaption></figure>

### 4. Login your Facebook account

<figure><img src="../../.gitbook/assets/image (223).png" alt=""><figcaption></figcaption></figure>

### 5. Select the page that you want

<figure><img src="../../.gitbook/assets/image (3173).png" alt=""><figcaption></figcaption></figure>

### 6. Choose the fields and click Next

<figure><img src="../../.gitbook/assets/image (3175).png" alt=""><figcaption></figcaption></figure>

### 7. Choose Data Freshness and who to share. Then click Save to finish.

<figure><img src="../../.gitbook/assets/image (3176).png" alt=""><figcaption></figcaption></figure>



## II. Set up Dataflow to push Facebook User ID data to Visitor Object in the CDP 365 system

### 1. Hover your mouse over Data on the left hand side menu and choose Realtime Stream

<figure><img src="../../.gitbook/assets/image (3177).png" alt=""><figcaption></figcaption></figure>

### 2. Click + button to create a Dataflow. Choose Facebook Messenger template.

<figure><img src="../../.gitbook/assets/image (3178).png" alt=""><figcaption></figcaption></figure>

### 3. Select the Facebook Messenger data source that you created, then click the Save button

<figure><img src="../../.gitbook/assets/image (3603).png" alt=""><figcaption></figcaption></figure>

### 4. Select the field you want to get the data

<figure><img src="../../.gitbook/assets/image (3604).png" alt=""><figcaption></figcaption></figure>

Note:

* **User ID** is the ID of the Facebook account who have sent message to your page
* Facebook only returns a list of User id that have sent message to your page within 24 hours

### 5.  Add Destination channel node

<figure><img src="../../.gitbook/assets/image (3605).png" alt=""><figcaption></figcaption></figure>

You can see how to create a destination channel for a Business Object

Select Visitor Business Object, then map Facebook's User id with Visitor's User ID on CDP 365 system

<figure><img src="../../.gitbook/assets/image (3606).png" alt=""><figcaption></figcaption></figure>

You need to create a **Custom attribute** in the **Visitor** Business Object to know it's the Facebook user ID pushed from the dataflow

You can see how to create a **Custom attribute**

For example: Create a Custom attribute of "Is Facebook user\_id" with data type of Number

<figure><img src="../../.gitbook/assets/image (3607).png" alt=""><figcaption></figcaption></figure>

* If the value of this attribute is 1, it is the User ID of Facebook

Set value pushed from dataflow to 1 for this Customer attribute

<figure><img src="../../.gitbook/assets/image (3608).png" alt=""><figcaption></figcaption></figure>

Pre-selected write mode is **Insert all**.

### 6. Save Dataflow

<figure><img src="../../.gitbook/assets/image (3609).png" alt=""><figcaption></figcaption></figure>

### 7. P**REVIEW**

Used to view setup information in dataflows.

<figure><img src="../../.gitbook/assets/image (3610).png" alt=""><figcaption></figcaption></figure>

**Force Run:** Used to run immediately without timeout in dataflows

<figure><img src="../../.gitbook/assets/image (3611).png" alt=""><figcaption></figcaption></figure>

After the dataflow has finished running, you can go to the Visitor menu in Personas App to check the creation of Facebook User ID in **CDP 365**:

<figure><img src="../../.gitbook/assets/image (3612).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (3613).png" alt=""><figcaption></figcaption></figure>

## III. Create a new Visitor Segment to get a list of Facebook User IDs

The conditions you set in the segment are as follows:

<figure><img src="../../.gitbook/assets/image (3614).png" alt=""><figcaption></figcaption></figure>

Note: You can see how to create a new segment

## IV. Create a FB Messenger destination&#x20;

### 1. Hover your mouse over Settings and go to Channel Integration

<figure><img src="../../.gitbook/assets/image (3616).png" alt=""><figcaption></figcaption></figure>

### 2. Click + button and choose the channel FB Messenger

<figure><img src="../../.gitbook/assets/image (3617).png" alt=""><figcaption></figcaption></figure>

### 3. Select Destination catalog: Antsomi Facebook

<figure><img src="../../.gitbook/assets/image (3618).png" alt=""><figcaption></figcaption></figure>

### 4. Fill in the necessary information for the destination

<figure><img src="../../.gitbook/assets/image (3621).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="228">Field</th><th>Description</th></tr></thead><tbody><tr><td>Page scoped user id</td><td><p>User ID Facebook of the recipient of the message</p><p>You can click <img src="../../.gitbook/assets/image (246).png" alt=""> icon to add Personalization<br><img src="../../.gitbook/assets/image (3619).png" alt=""></p></td></tr><tr><td>Access token</td><td>Access token of your page on Facebook.</td></tr></tbody></table>

**Note: Currently, please share your page with us with the following permission: "Send and respond to message as the Page"**&#x20;

<figure><img src="../../.gitbook/assets/image (249).png" alt="" width="375"><figcaption></figcaption></figure>

**-> We will help you set up the necessary information in destination**



### V. Sending FB Messenger via Customer Journey

Log into **CDP 365** system, hover your mouse over **MARKETING** to see all the available channels.

<figure><img src="../../.gitbook/assets/image (3622).png" alt=""><figcaption></figcaption></figure>

We have 2 channels that supporting to send:

* FB Messenger
* Journey Orchestration

<figure><img src="../../.gitbook/assets/image (3623).png" alt=""><figcaption></figcaption></figure>

For this example, let's choose Orchestration

<figure><img src="../../.gitbook/assets/image (3624).png" alt=""><figcaption></figcaption></figure>

At the Schedule trigger node, select the segment containing the Facebook user id that you created

<figure><img src="../../.gitbook/assets/image (3625).png" alt=""><figcaption></figcaption></figure>

Click **+** button to add Destination node and select **Antsomi Facebook** destination

<figure><img src="../../.gitbook/assets/image (3626).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (3627).png" alt=""><figcaption></figcaption></figure>

Choose the destination that you created

<figure><img src="../../.gitbook/assets/image (3628).png" alt=""><figcaption></figcaption></figure>

Fill out necessary information

<figure><img src="../../.gitbook/assets/image (3629).png" alt=""><figcaption></figcaption></figure>

Click **Save** button to finish setting journey

<figure><img src="../../.gitbook/assets/image (3630).png" alt=""><figcaption></figcaption></figure>

After finishing the setting of the Journey, we can **activate** and send message to customer
