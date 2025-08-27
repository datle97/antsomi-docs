# How to create "Attribute" for "Customer"/"Visitors"?

{% embed url="https://app.gitbook.com/o/-LzunofLVjpTa_-p1PQt/s/mECwNqMNUmu6OXHSYgDv/quick-start-guide/how-to-create-attribute-for-customer-visitors" %}

&#x20;1\. Hover your mouse over **Data** → Choose **Data Objects**

<figure><img src="../../.gitbook/assets/image (102).png" alt=""><figcaption></figcaption></figure>

&#x20; 2\. Select **Customer/Visitors** Data Object

<figure><img src="../../.gitbook/assets/image (103).png" alt=""><figcaption></figcaption></figure>

3\. Choose **Attributes** tab -> Click **+** button, choose Create New Attribute

<figure><img src="../../.gitbook/assets/image (104).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (105).png" alt=""><figcaption></figcaption></figure>

4\. List of Attribute type that the system is supporting:

<figure><img src="../../.gitbook/assets/image (106).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (108).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="72">No</th><th>Computed Attribute Types</th><th>Description</th></tr></thead><tbody><tr><td>1</td><td>Event Counter</td><td>Stores a count of a certain event over some time</td></tr><tr><td>2</td><td>Aggregation</td><td>Aggregates (min, max, sum, average) values of an event attribute into a single value</td></tr><tr><td>3</td><td>Most Frequent</td><td>Returns the most common value of an event attribute</td></tr><tr><td>4</td><td>First</td><td>Returns the first received value of an event attribute</td></tr><tr><td>5</td><td>Last</td><td>Returns the last received value of an event attribute</td></tr><tr><td>6</td><td>Unique List</td><td>Stores a list of unique values of an event attribute</td></tr><tr><td>7</td><td>Unique count</td><td>Counts the number of elements in a unique list</td></tr><tr><td>8</td><td>Conversion  Attribution</td><td>Finds winner of a conversion event using attribution models</td></tr><tr><td>9</td><td>Virtual Customer Function</td><td>Returns output of your custom function</td></tr><tr><td>10</td><td>Schedule Customer Function</td><td>Returns a scheduled-updated output of your custom function</td></tr><tr><td>11</td><td>Custom Attribute</td><td>For labeling or input data</td></tr></tbody></table>

Create **Virtual Custom Function**

<figure><img src="../../.gitbook/assets/image (107).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="199">Group</th><th width="160">Fields</th><th>Description</th></tr></thead><tbody><tr><td>General Information</td><td>Object</td><td>Name of chosen business objects. System fills in automatically and you can not edit.</td></tr><tr><td></td><td>Group attribute</td><td>Select one of group attribute of chosen object above. System fills in automatically and you can edit.</td></tr><tr><td></td><td>Attribute type</td><td>Name of attribute type you chosen in Step 1</td></tr><tr><td></td><td>Attribute name</td><td>Name of new attribute</td></tr><tr><td></td><td>Attribute internal code</td><td>Code of new attribute is automatically added by the system but you can edit it.</td></tr><tr><td></td><td>Description</td><td>More descriptions to make clear your new attribute information.</td></tr><tr><td>Edit Info</td><td>Function</td><td>Enter functions to calculate</td></tr><tr><td></td><td>Data type of function output</td><td>Select the data type for the function's output. The data types that the system supports: number, string, datetime</td></tr><tr><td></td><td>Display function output</td><td><p>Display format of data output: </p><p>  + Number: Number, percentage, currency </p><p>  + String: Raw string, image, link </p><p>  + Date time: Datetime</p></td></tr><tr><td></td><td>Function list</td><td>List of functions that user can use</td></tr><tr><td></td><td>Available Attributes</td><td>List of Customer/Visitor Attributes</td></tr><tr><td></td><td>Enable Data Encryption</td><td>Encrypt and protect your data</td></tr></tbody></table>

Create **Schedule Custom Function**

<figure><img src="../../.gitbook/assets/image (109).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="203">Group</th><th width="188">Fields</th><th>Description</th></tr></thead><tbody><tr><td>General Information</td><td>Object</td><td>Name of chosen business objects. System fills in automatically and you can not edit.</td></tr><tr><td></td><td>Group attribute</td><td>Select one of group attribute of chosen object above. System fills in automatically and you can edit.</td></tr><tr><td></td><td>Attribute type</td><td>Name of attribute type you chosen in Step 1</td></tr><tr><td></td><td>Attribute name</td><td>Name of new attribute</td></tr><tr><td></td><td>Attribute internal code</td><td>Code of new attribute is automatically added by the system but you can edit it.</td></tr><tr><td></td><td>Description</td><td>More descriptions to make clear your new attribute information.</td></tr><tr><td>Edit Info</td><td>Function</td><td>Enter functions to calculate</td></tr><tr><td></td><td>Data type of function output</td><td>Select the data type for the function's output. The data types that the system supports: number, string, datetime</td></tr><tr><td></td><td>Display function output</td><td><p></p><p>Display format of data output:</p><ul><li>Number: Number, percentage, currency</li><li>String: Raw string, image, link</li><li>Date time: Datetime</li></ul></td></tr><tr><td></td><td>Function list</td><td>List of functions that user can use</td></tr><tr><td></td><td>Available Attributes</td><td>List of Customer/Visitor Attributes</td></tr><tr><td></td><td><strong>Compute schedule</strong></td><td><p>Choose a schedule to compute this attribute. The default value is 1/hours </p><p>  + Hours: Allow input from 1 to 23 </p><p>  + Days: Allow input from 1 to 365</p></td></tr></tbody></table>

Create **Custom Attribute**

<figure><img src="../../.gitbook/assets/image (110).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="178">Group</th><th width="190">Fields</th><th>Description</th></tr></thead><tbody><tr><td>General Information</td><td>Object</td><td>Name of chosen business objects. System fills in automatically and you can not edit.</td></tr><tr><td></td><td>Group attribute</td><td>Select one of group attribute of chosen object above. System fills in automatically and you can edit.</td></tr><tr><td></td><td>Attribute type</td><td>Name of attribute type you chosen in Step 1</td></tr><tr><td></td><td>Attribute name</td><td>Name of new attribute</td></tr><tr><td></td><td>Attribute internal code</td><td>Code of new attribute is automatically added by the system but you can edit it.</td></tr><tr><td></td><td>Description</td><td>More descriptions to make clear your new attribute information.</td></tr><tr><td>Setting</td><td>Data type</td><td>Select the data type for the function's output. The data types that the system supports: Number, String, Text, Datetime, Boolean, Array (Array Numbers, Array Strings, Array Datetimes), Object</td></tr><tr><td></td><td>Display format</td><td><p>Display format of data type: </p><p>  + Number: Number, percentage, currency </p><p>  + String: Raw string, image, link </p><p>  + Date time: Datetime</p></td></tr><tr><td></td><td>Is Required</td><td>Mark this attribute as required for the Customer/Visitor business object</td></tr><tr><td></td><td>Enable Data Encryption</td><td>Encrypt and protect your data</td></tr><tr><td></td><td>Is Identity Attribute</td><td>Attribute identifier. Fields considered Identity are fields that can contain information such as phone, email, device ID, ...</td></tr></tbody></table>

You can check data of the **Customer/Visitor attribute** in menu: **Profiles -> Customers/Visitor**

<figure><img src="../../.gitbook/assets/image (112).png" alt=""><figcaption></figcaption></figure>
