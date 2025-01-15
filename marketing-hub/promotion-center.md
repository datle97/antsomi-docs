---
description: This app manage the codes which will be distributed to your audiences
---

# Promotion Center

## OVERVIEW

The interface includes 3 tabs:&#x20;

1. Promotion pools: Provide the list of pools and its detailed information
2. Promotion Integration: Manage the Source where the promotion codes will be imported from
3. Process Histories: Manage the running histories every time codes are imported from a specific source

<figure><img src="../.gitbook/assets/image (1682).png" alt=""><figcaption><p>Promotion Center</p></figcaption></figure>

## DETAILS

### I. Promotion Pool

The data table displays a list of promotion pools created by the users.

<figure><img src="../.gitbook/assets/image (1556).png" alt=""><figcaption><p>Promotion pools</p></figcaption></figure>

You can perform some basic feature with the data table by using [Basic button](https://docs.antsomi.com/cdp-365-user-guide-en/cdp-365-introduction/cdp-365s-interface#basic-buttons).&#x20;

### A- Status of Promotion Pool

![](<../.gitbook/assets/image (1870).png>)In Process: The codes are uploading/ importing to the pool.

![](<../.gitbook/assets/image (455).png>)Active: The codes are uploaded/ imported successfully.

![](<../.gitbook/assets/image (764).png>)Deactive: The pool is disabled, users could not use it in Customer Journey. If a pool was used in a Journey but later was deactivated, the message would not be sent to the audience.

![](<../.gitbook/assets/image (544).png>)Expired: The promotion pool has expired, codes could not be allocated in Journey.

{% hint style="info" %}
You can change the status of a Promotion Pool by switching the button ![](<../.gitbook/assets/image (600).png>) or ![](<../.gitbook/assets/image (566).png>)
{% endhint %}

### B- The details of a pool

To see the details of a promotion pool, click on the name of the pool

<figure><img src="../.gitbook/assets/image (1571).png" alt="" width="375"><figcaption></figcaption></figure>

The pool's detailed information includes the list of promotion codes and the information of through which Journey/ Campaign/ Variant the code has been allocated, who has received the code, etc.

There are 3 tabs:&#x20;

1. **Promotion codes**

<figure><img src="../.gitbook/assets/image (1574).png" alt=""><figcaption><p>Pool's details</p></figcaption></figure>

#### Status of Promotion code

![](<../.gitbook/assets/image (455).png>)Available: The code has not been allocated yet

![](<../.gitbook/assets/image (1870).png>)Allocated: The code has been allocated to customer through Customer Journey (Eg: Through Media template, etc)

![](<../.gitbook/assets/image (2332).png>)Sent: The code has been sent to the customer though messages. (Eg: SMS, Email,...)

<img src="../.gitbook/assets/image (1312).png" alt="" data-size="original"> Used: A promotion code was used by the customer

#### Move codes

To move codes from a pool to another one, please follow these steps:

1. Select the codes you want to move (NOTE: Only codes having "Available" status could be moved out of the current pool)
2. Click _Edit_ and choose _Move to_

<figure><img src="../.gitbook/assets/image (1561).png" alt="" width="375"><figcaption></figcaption></figure>

3. Choose the pool where the codes will be moved to and click <img src="../.gitbook/assets/image (1584).png" alt="" data-size="line">

<figure><img src="../.gitbook/assets/image (1310).png" alt="" width="375"><figcaption></figcaption></figure>

2. **Settings**

This tab includes the configuration of the promotion pool, you could adjust any editable field and then click Save to change the settings.

<figure><img src="../.gitbook/assets/image (867).png" alt=""><figcaption></figcaption></figure>

3. **Process Histories**

This tab manages the histories every time a process of importing codes from the Promotion Source to CDP 365.

To immediately importing the codes, click Force Sync button on the right corner.

<figure><img src="../.gitbook/assets/image (930).png" alt=""><figcaption></figcaption></figure>

### C- Create a Promotion Pool

To create a new Promotion Pool, click on the ![](<../.gitbook/assets/image (2392).png>) button. There are two methods to create the pools:

* Manual Upload - The code will be imported to the pool by an uploaded file
* Automatically - The code will be imported from a specific [Promotion Source](promotion-center.md#create-a-promotion-source)&#x20;

<figure><img src="../.gitbook/assets/image (2398).png" alt=""><figcaption></figcaption></figure>



#### Manual Upload

<figure><img src="../.gitbook/assets/image (1724).png" alt=""><figcaption></figcaption></figure>



The setting of a Promotion Pool includes:

1. **General Information:** Input the name and description of the pool

<figure><img src="../.gitbook/assets/image (1872).png" alt="" width="375"><figcaption><p><em>General Information</em></p></figcaption></figure>

2. **Upload your file of promotion codes:** Browse the file from your local and then map the fields in CDP 365 with the fields in the file.

<figure><img src="../.gitbook/assets/image (1866).png" alt="" width="375"><figcaption><p><em>Upload your file of promotion codes</em></p></figcaption></figure>

3. **Advanced Settings**



<figure><img src="../.gitbook/assets/image (1907).png" alt="" width="375"><figcaption></figcaption></figure>

**Pool expiration**&#x20;

Set the expiration time of the pool, when it expires, the code in the pool will not be allocated in the Customer Journey

* **No expiration date:** Unlimited time for using the codes
* **All remaining codes expire on:** Choose a specific expiration date and time to use the Promotion pool (The selected time must be in the future compared to the present time)



**Allocation restriction type**&#x20;

Set a code allocation limit for each audience in Journey. Since 1 pool can be used in multiple Journeys, the limit will include the following 2 options:

* **Unique - only one code for every allocation:** In 1 Journey, each person can only receive 1 code in the pool. (For example: This option serves the need to only issue 1 code, no matter how many times submitted in the lead form)
* **Multiple - renew code for each allocation:** In 1 Journey, each person can get MULTIPLE codes in the pool.&#x20;
* **For example:**

\-- Use case: Issue code to customers with orders over 5 million.&#x20;

\-- Current situation: Customers buy 2 orders, each order is worth more than 5 million VND&#x20;

\-- Result: This customer will receive 2 codes.



**Set up alert** - Set up email notifications if:

<figure><img src="../.gitbook/assets/image (1904).png" alt="" width="375"><figcaption></figcaption></figure>

* **Remind code expiration before \_\_ day(s):** Only {x} days left, pool will expire
* **Remind when less than \_\_ code(s) left:** In the pool there are only {x} codes with the status "available"
* **Alert will be sent to:** Select an account to receive this notification email



#### Automatically&#x20;

After [creating a Promotion Source](promotion-center.md#create-a-promotion-source) successfully, it will add the Source in the Create pop-up. Please choose the Source you want to take the codes from.

<figure><img src="../.gitbook/assets/image (2409).png" alt=""><figcaption></figcaption></figure>

After choosing the Source, the screen shows as below:

<figure><img src="../.gitbook/assets/image (2445).png" alt=""><figcaption></figcaption></figure>

The setting includes:

_**General Information:**_ Fill in the name and the description of the pool

_**Setting**_

<figure><img src="../.gitbook/assets/image (914).png" alt="" width="375"><figcaption></figcaption></figure>

* **Source:** Select the Source that will be used to pull the code to the pool being created. To change to another source, click on the dropdown to select Source or create a new Source <img src="https://lh5.googleusercontent.com/xSm67tMYv-whYySN723bWVqul0BMDb7n5EWaR5OuRD_MB5Vt4PF1De0e5dW5psXN4pGUoGr0VK43VzeOfR9C96anNXYxR0R5fO5DHY8F0m55SnmMNceKQRBejHH8rfbrM8pX_B8gOcYt5JPd4zB6F_g" alt="" data-size="line">
* **Scheme ID:** The ID of the pool in the Source
* **Interval:** Frequency of pulling code from Source to CDP 365. There are 2 options to choose:&#x20;

&#x20;    \--> Manually: The codes will be pulled to CDP 365 when users click [Force Sync](promotion-center.md#iii.-process-histories) button

&#x20;    \--> Repeat by time: Set  a schedule to import the promotion codes. Besides, you could determine the amount of remaining codes in the Source from which the import process would start if that  amount were reached.

For example: In the picture above, the process of importing code will ONLY start if the twon conditions are met (The date and time is 11:55 AM on July 28th and there is 10 codes left in the pool from the Source)

* **Code quantity:** Adjust the amount of code that will be pulled each time. (NOTE: The number of codes entered in the pool in CDP 365 must be less than the number of codes available in the Source. If it is larger, the process will be failed.)

_**Advanced Settings**:_ It is similar to [Advanced Settings](promotion-center.md#manual-upload) when upload codes from a file.

## II. Promotion Integration

This tab allows you connect with a promotion code storage system to automatically import the code to CDP 365.

<figure><img src="../.gitbook/assets/image (2435).png" alt=""><figcaption><p><em>Promotion Integration</em></p></figcaption></figure>

### Create a Promotion Source

To connect with your code storage system, please follow these steps:

1. Click on the <img src="../.gitbook/assets/image (2441).png" alt="" data-size="line"> button
2. Choose the Source you want to connect and then click <img src="../.gitbook/assets/image (2411).png" alt="" data-size="line">

<figure><img src="../.gitbook/assets/image (2406).png" alt=""><figcaption></figcaption></figure>

3. Input authentication information and click ![](broken-reference)

<figure><img src="../.gitbook/assets/image (2450).png" alt=""><figcaption></figcaption></figure>

After connecting successfully, the newly created Promotion Source will display in the Data table as follows:

<figure><img src="https://lh4.googleusercontent.com/5bdbuIyxjDhhPUzcD_5SbStUL03cTsj86TTxSQto4v3c6bOBeCMtHswQ7x8v7UeX83s0zAV-qA4uD0biaUJCcQwibf_1KskoNcBujlf_5fr9oYWDVCGSsZDqOzhNC__545xR8FEDKjZHFgp6LjlfNAM" alt=""><figcaption></figcaption></figure>

## III. Process Histories

This tab manages the histories of all running processes every time the promotion codes were imported from the Promotion Source to the Promotion Pool.

<figure><img src="../.gitbook/assets/image (2413).png" alt=""><figcaption><p>Process Histories</p></figcaption></figure>

## EXPLORATION

<figure><img src="../.gitbook/assets/image (2026).png" alt=""><figcaption></figcaption></figure>

The explore function gives you an overview of the data of each object. Here you can analyze objects by creating charts yourself or using the system's built-in templates.

### Explore all promotion pool

1. Click on <img src="../.gitbook/assets/image (1167).png" alt="" data-size="line"> button.
2. Select Create custom template to create template explore or Use a available template.
3. In Explore pop up, you can add charts or drag and drop to change the dimensions and metrics as desired.
4. Click on <img src="../.gitbook/assets/image (2388).png" alt="" data-size="line"> to Save this explore become Private template (only you can view and edit) or Public template (everyone can view and use.)  Or select Manage template to view all template you can view.

### Explore a promotion pool

* Click on <img src="../.gitbook/assets/image (2507).png" alt="" data-size="line"> button.
* In Explore pop up, you can add charts or drag and drop to change the dimensions and metrics as desired.
* Click on <img src="../.gitbook/assets/image (2388).png" alt="" data-size="line"> to Save this explore become Private template (only you can view and edit) or Public template (everyone can view and use.)  Or select Manage template to view all template you can view.
* In Explore pop up, you can add charts or drag and drop to change the dimensions and metrics as desired.

##
