# Attributes

<figure><img src="../../../../.gitbook/assets/image (3566).png" alt=""><figcaption></figcaption></figure>

## Create a new attribute

1. Click ![](<../../../../.gitbook/assets/image (1649).png>)to create a new attribute&#x20;

<figure><img src="../../../../.gitbook/assets/image (3568).png" alt=""><figcaption></figcaption></figure>

2. Choose Attribute Types&#x20;

<figure><img src="../../../../.gitbook/assets/image (3575).png" alt=""><figcaption></figcaption></figure>

3. Input the necessary information

<figure><img src="../../../../.gitbook/assets/image (3574).png" alt=""><figcaption></figcaption></figure>

* **General Information:** The basic & descriptive information about the attribute
* **Setting**
* _Data Type_: The type of data to be recorded in the attribute
* _Display Format:_ The format that the data will be displayed. The format will depend on the chosen Data Type
* _Is required_: Mark this attribute as required meaning in the data pushed to the BO, this attribute must have value, if not it will be rejected.
* _Personal Identifiable Information_: Mark the attribute as PII and encrypt the data recorded in the data table. Only accounts having the [decrypt permissions](https://docs.antsomi.com/cdp-365-user-guide-en/portal-settings/data-encryption#decrypt-permission) are able to decrypt it.&#x20;
* _Enable Data Encryption_: Encrypt the data in the attribute
* _Is Identity Attribute:_&#x20;

4. Click **Save** to save

### Attribute Types&#x20;

<table><thead><tr><th width="81">No</th><th>Attribute Types </th><th>Description </th><th>Setting of attribute</th></tr></thead><tbody><tr><td>1</td><td>Custom Attribute</td><td>The attribute in which data does not need to compute</td><td><a href="custom-attribute.md">Custom Attribute Setting</a></td></tr><tr><td>2</td><td>Computed Attribute</td><td>The attribute in which data need to compute by the system</td><td></td></tr><tr><td>2.1</td><td>Event Counter</td><td>Count occurrences of an event</td><td><a href="computed-attribute/event-counter.md">Event Counter Setting</a></td></tr><tr><td>2.2</td><td>Aggregation</td><td>Aggregate functions include min, max, sum, and average. It is calculated based on values ​​of an event attribute</td><td><a href="computed-attribute/aggregation.md">Aggregation Setting</a></td></tr><tr><td>2.3</td><td>Most Frequent</td><td>Returns the most common value of an event attribute</td><td><a href="computed-attribute/most-frequent.md">Most Frequent Setting</a></td></tr><tr><td>2.4</td><td>First</td><td>Returns the first received value of an event attribute</td><td><a href="computed-attribute/first.md">First Setting</a></td></tr><tr><td>2.5</td><td>Last</td><td>Returns the last received value of an event attribute</td><td><a href="computed-attribute/last.md">Last Setting</a></td></tr><tr><td>2.6</td><td>Unique List</td><td>Stores a list of unique values of an event attribute </td><td><a href="computed-attribute/unique-list.md">Unique List Setting</a></td></tr><tr><td>2.7</td><td>Unique List Count</td><td>Counts the number of elements in a unique list</td><td><a href="computed-attribute/unique-count.md">Unique List Count Setting</a></td></tr><tr><td>2.8</td><td>Conversion Attribution</td><td>Finds winner of a conversion event using attribution models</td><td><a href="computed-attribute/conversion-attribution.md">Conversion Attribution Setting</a></td></tr><tr><td>2.9</td><td>Virtual Custom Function</td><td>Returns output of your custom function</td><td><a href="computed-attribute/virtual-custom-function.md">Virtual Custom Function Setting</a></td></tr><tr><td>2.10</td><td>Schedule Custom Function</td><td>Returns a scheduled-updated output of your custom function</td><td><a href="computed-attribute/schedule-custom-function.md">Schedule Custom Function Setting</a></td></tr></tbody></table>

{% hint style="info" %}
Each Attribute type has particular information, go to a specific attribute type to see its setting&#x20;
{% endhint %}

## Attribute Action

Select at least one Attribute and click on Edit will show possible actions for the selected Attribute

<figure><img src="../../../../.gitbook/assets/image (3572).png" alt=""><figcaption></figcaption></figure>

### Enable attribute

When enabling the attribute will change the state of the attribute to Enabled.

If within a specified time the attribute is not used anywhere, the state is changed to disabled

### Disable attribute

Disabling the attribute changes the state of the attribute to Disabled. This will then block the input of the attribute. Attribute cannot be used in any function.&#x20;

If, within a specified time, the attribute is not re-enabled, the attribute will automatically change its state to archived.

### Archive attribute

When archive attribute will block all output and input of attribute. Then the attribute will not show up in any attribute selector list.

If within a specified time period, the attribute is not enabled, it will be deleted forever.

### Recover

Restore archived attribute.

During recovery, the attribute's state can be changed to enabled or disabled.

### Copy an attribute

CDP 365 allows you to make a copy of an attribute. This helps you quickly create a new attribute based on the original with flexible customize

<figure><img src="../../../../.gitbook/assets/image (3573).png" alt=""><figcaption></figcaption></figure>

Following the steps below to make a copy of an attribute:

1. Select an attribute that you want to make a copy
2. Click **Edit** and select **Make a copy**&#x20;
3. Customize the setting&#x20;
4. Click **Save** to save&#x20;

For example, you have an attribute that is a list of keywords searched for 30 days. You need to create an attribute that is a list of keywords searched for 14 days; now you just make a copy and customize the date range instead of creating and setting whole attribute information

## Edit an attribute setting

Following these steps:

1\. Click the name of the attribute that you want to change information on the data table

2\. Enter the changed information

3\. Click **Save**

## Add attributes to a group&#x20;

You can add attributes that have the same characteristic or usage to a group. See more about [Groups](../groups.md)

## Display the newly created attribute on the Data table&#x20;

To display the newly created attribute on the [Data table](../data-table.md), use the [Modify Column](../../../../cdp-365-introduction/cdp-365s-interface.md#customize-display-columns) utility

## Attribute Computation Histories&#x20;

### View Attribute Computation Histories

Click the icon ![](<../../../../.gitbook/assets/image (857).png>)on the attribute display to view the Attribute Computation Histories

### Attribute Computation Histories Data table

It presents a data table containing information about attribute computation

* **Computation ID:** Every time attribute is computed, it will have an ID
* **Name:** name of the attribute
* **Attribute Type:** type of the attribute
* **Computation trigger:** Trigger by the user or Scheduled Update
* **Computation status:** Status of the computation (Success, Computing, Unsuccess, Paused, Waiting)
* **Computation started on:** the date and time that the computation starts
* **Computation ended on:** the date and time that the computation ends
* **Computation duration (sec):** The duration of computation (in seconds)
* **Computation output:** Number of outputs that satisfy the condition after finishing computation
* **Error info:** Error code that caused compute failed

## Status of attribute

You can change the status of an attribute by switching the button![](<../../../../.gitbook/assets/image (3565).png>)or ![](<../../../../.gitbook/assets/image (3773).png>)

## Use cases of Attribute
