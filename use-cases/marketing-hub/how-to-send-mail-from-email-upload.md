---
description: >-
  When you have a data set of customers' emails as files and you want to send
  them emails for some purpose, for example: advertising, sending promotional
  codes,... Please follow this instructions:
---

# How to send mail from email upload?

## ![](<../../.gitbook/assets/image (2000).png>) Create attribute "Email" for Customer/ Visitor

First, you have to create an attribute containing the customer email data, which you want to upload.

&#x20;   1\. Log in to **CDP 365**.

&#x20;   2\. Hover your mouse over **Data.** Choose **Data Objects.**

<figure><img src="../../.gitbook/assets/image (3127).png" alt=""><figcaption></figcaption></figure>

3\. Select the **Customer/Visitor** Data object

<figure><img src="../../.gitbook/assets/image (3128).png" alt=""><figcaption></figcaption></figure>

&#x20;  4\. Choose **Attributes** tab -> Click **+** button -> Choose **Create New Attribute**

<figure><img src="../../.gitbook/assets/image (3129).png" alt=""><figcaption></figcaption></figure>

&#x20;  5\. Select **Custom Attributes** type

<figure><img src="../../.gitbook/assets/image (3130).png" alt=""><figcaption></figcaption></figure>

&#x20;  6\. Enter the information to create [attributes ](how-to-send-mail-from-email-upload.md#1.-mo-ta-cac-field-khi-tao-attribute).&#x20;

<figure><img src="../../.gitbook/assets/image (3133).png" alt=""><figcaption></figcaption></figure>

Note that the Datatype that must be selected is String.

<figure><img src="../../.gitbook/assets/image (3132).png" alt=""><figcaption></figcaption></figure>

&#x20;  7\. Click **Save**

&#x20;  8\. After finishing, you will be back on the **Customers/Visitors** object view in **Data Object** menu. You will see your newly created attribute here.&#x20;

<figure><img src="../../.gitbook/assets/image (3134).png" alt=""><figcaption></figcaption></figure>

## &#x20;![](<../../.gitbook/assets/image (2524).png>) Upload data for "Email" Attribute

&#x20;   1\. Log in to **CDP 365**.

&#x20;   2\. Hover your mouse over **Profiles.** Choose **Customers/Visitors.**

<figure><img src="../../.gitbook/assets/image (3135).png" alt=""><figcaption></figcaption></figure>

&#x20;  3\. Click **Import** icon

<figure><img src="../../.gitbook/assets/image (3136).png" alt=""><figcaption></figcaption></figure>

4\. Select **Browse**, then select the file containing the desired Email data set. Only .csv, .xls, .xlxs files are supported

<figure><img src="../../.gitbook/assets/image (3137).png" alt=""><figcaption></figcaption></figure>

6\. Select Import type **Update Only**

<figure><img src="../../.gitbook/assets/image (3138).png" alt=""><figcaption></figcaption></figure>

7\. Mapping the existing Attributes in the **Customers** Object with the columns in the uploaded file.

<figure><img src="../../.gitbook/assets/image (3139).png" alt=""><figcaption></figcaption></figure>

8\. Click **Save**

## ![](<../../.gitbook/assets/image (1420).png>) Create Destination to send mail

&#x20;   1\. Log in to **CDP 365**.

&#x20;   2\. Hover your mouse over **Settings.** Choose **Channel Integration.**

<figure><img src="../../.gitbook/assets/image (3140).png" alt=""><figcaption></figcaption></figure>

&#x20;  3\. Click the plus icon ![](<../../.gitbook/assets/image (1887).png>) and select **Email**

<figure><img src="../../.gitbook/assets/image (3141).png" alt=""><figcaption></figcaption></figure>

4\. Set up information to create [destination](how-to-send-mail-from-email-upload.md#create-attribute-email-for-customer-visitor). User can choose the corresponding mailing service in **Destination Catalog**. In this example, we choose **G Suite Email**.&#x20;

<figure><img src="../../.gitbook/assets/image (3299).png" alt=""><figcaption></figcaption></figure>

**Note:** choose Method as **Send**

<figure><img src="../../.gitbook/assets/image (3144).png" alt=""><figcaption></figcaption></figure>

5\. At field **Email**, click icon ![](<../../.gitbook/assets/image (787).png>) **Add Personalization**.&#x20;

<figure><img src="../../.gitbook/assets/image (3145).png" alt=""><figcaption></figcaption></figure>

&#x20; Select Attribute **Email** in list attribute of **Customer** Object -> Then click **Insert**

<figure><img src="../../.gitbook/assets/image (3300).png" alt=""><figcaption></figcaption></figure>

6\. Click **Save**

<figure><img src="../../.gitbook/assets/how to send email from email upload - 1.gif" alt=""><figcaption></figcaption></figure>

## ![](<../../.gitbook/assets/image (1747).png>) Setup Journey to send mail&#x20;

1\. Log into CDP 365 system. &#x20;

2\. Hover your mouse over **Marketing** on the left hand side menu.

<figure><img src="../../.gitbook/assets/image (3146).png" alt=""><figcaption></figcaption></figure>

We have 2 channels that supporting to send:

* Email
* Journey Orchestration

<figure><img src="../../.gitbook/assets/image (3149).png" alt=""><figcaption></figcaption></figure>

3\.  Select channel **Orchestration** -> Click icon ![](<../../.gitbook/assets/image (2258).png>)

<figure><img src="../../.gitbook/assets/image (3150).png" alt=""><figcaption></figcaption></figure>

Choose **Start From Scratch**

<figure><img src="../../.gitbook/assets/image (3151).png" alt=""><figcaption></figcaption></figure>

4\. Set up the necessary information for Journey.&#x20;

Click **+** button, choose the **Scheduled Trigger** node.

<figure><img src="../../.gitbook/assets/image (3152).png" alt=""><figcaption></figcaption></figure>

Note: it is necessary to select the set of segments corresponding to the Email data set that has just been uploaded in II (Details about segments can be found in the description of the segment).

5\.  Add **G Suite Email** node

<figure><img src="../../.gitbook/assets/image (3154).png" alt=""><figcaption></figcaption></figure>

6\.  Choose the correct destination that the user has set up to send mail in Journey settings to send mail to customers

<figure><img src="../../.gitbook/assets/image (3296).png" alt=""><figcaption></figcaption></figure>

7\. Click **Save**. By default, the newly created Journey's status is **In design.**

<figure><img src="../../.gitbook/assets/image (3156).png" alt=""><figcaption></figcaption></figure>

8\.  Select **Activate**. Journey's status will change from **In design** to **Active**.

<figure><img src="../../.gitbook/assets/image (3157).png" alt=""><figcaption></figcaption></figure>

## Note

### 1. Description of fields when creating Attribute

| Field                   | Description                                                                                                                                                                                                                                                                                                                                       |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Object                  | This field indicates which Business Object attribute is being created in. By default, Business Object selected in step 3 will be displayed (not edited)                                                                                                                                                                                           |
| Group attribute         | Group to which this "Email" attribute will be assigned. Clicking will open a list of existing groups belonging to Business Object                                                                                                                                                                                                                 |
| Attribute type          | Help the user know what type of attribute is creating/editing (not edited). Default value will be “Custom””                                                                                                                                                                                                                                       |
| Attribute name          | Name of attribute. For example: “Email”                                                                                                                                                                                                                                                                                                           |
| Attribute internal code | Attribute internal code will be automatically generated after the user enters the Attribute name and can be clicked by the user to change the internal code. For example: If the above name is "Email", then below the Attribute internal code will be "email".                                                                                   |
| Description             | Description of attribute                                                                                                                                                                                                                                                                                                                          |
| Data type               | The data type of attribute.Custom Attribute supports 7 types of data types including: number, string, text, datetime, boolean, object, array Example: For "Email" we will choose the data type as "String"                                                                                                                                        |
| Display Format          | For each selected Data type above, there will be a display as set corresponding to that data type. https://www.screencast.com/t/gZCm9JLpAP Example: For attribute “Email” will choose “Raw String”                                                                                                                                                |
| Is Required             | Mark this attribute as required for the "Business Object" under consideration. By default, this checkbox is unchecked                                                                                                                                                                                                                             |
| Auto suggestion         | <p>This field is only enabled when the data type of the attribute is string. For other data types that are not supported, this option will be disabled.<br>By default, this checkbox is unchecked</p>                                                                                                                                             |
| Enable Data Encryption  | Mark the data encoding for this attribute. By default, this checkbox is unchecked                                                                                                                                                                                                                                                                 |
| Is Identity Attribute   | If checked, the generated attribute will be marked with an identifier. Fields that are considered Identity are fields that can contain information such as: phone, email, device ID, ... Only "Business Object" is Customer and Visitor when creating Custom Attribute, there is a checkbox "Is Identity". By default, this checkbox is unchecked |

### 2. Download data example

{% file src="../../.gitbook/assets/Example Upload Email.xlsx" %}

### 3. Description of fields when creating a Destination - G Suite Email

| Field                                               | Description                                                                                                                                                                                                                            |
| --------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Destination Name                                    | Destination names are supported with multi-lang. By default, the language icon will display according to the language configured in Portal setting - Portal language setting, and this value is considered the default value.          |
| Description                                         | Description of destination, with multi-lang support                                                                                                                                                                                    |
| Destination Catalog                                 | Channel Email has catalogs like: Amazon SES, Onesignal Email, G Suite Email… → in this example we choose the catalog as G Suite Email                                                                                                  |
| Method                                              | Catalogs belonging to App Push, Web Push channels, the default method will be Push. Catalogs belonging to Email, Webhook, and Conversation channels, the default method will be Send. In this example, we will choose Send.            |
| Email                                               | <p>Click icon Add Personalization <img src="../../.gitbook/assets/image (1927).png" alt=""> </p><p>Personalization Attribute: List of attributes belonging to the selected Personalization type. In this example we choose “Email”</p> |
| From Email Name                                     | Sender name                                                                                                                                                                                                                            |
| Username                                            | Sender email                                                                                                                                                                                                                           |
| Password                                            | Sender email password                                                                                                                                                                                                                  |
| Ignore duplicate messages for the scheduled journey | Limit allocation frequency to 1 address in 1 scheduled iteration of a journey                                                                                                                                                          |
| Limit frequency for the journey (3 months duration) | Limit allocation frequency to 1 address in 1 journey                                                                                                                                                                                   |
| Limit frequency for destination                     | Limit allocation frequency to 1 address per unit of time (hour, day, ...)                                                                                                                                                              |





