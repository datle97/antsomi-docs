---
description: >-
  Conversion attribution helps you find which value of the attribute (it can be
  channels, events, campaigns, etc) lead to the conversion event
---

# Conversion Attribution

The Data Object whose setting is '_**Treat as Conversion Object**_', will have the Conversion Attribution type

## Conversion Attribution Configure

<figure><img src="../../../../../.gitbook/assets/Conversion Attribution.png" alt=""><figcaption></figcaption></figure>

### General Information

* **Object:** the corresponding Object that you chose to create the attribute
* **Group attribute:** Group contains attributes that have the same characteristic or usage. [See more about Groups](../../groups.md)
* **Attribute type:** [type of attribute](conversion-attribution.md#kieu-thuoc-tinh) you chose to create
* **Attribute name:** name of the attribute
* **Attribute internal code:** code of the attribute
* **Description:** information describes the attribute

{% hint style="warning" %}
Note: the attribute code does not allow prefixes: number\_, sgmt\_, aud\_&#x20;
{% endhint %}

### Setting

* **Conversion event:** the event that leads to conversion
* **Sources**: sources that event is logged
* **Conversion condition:**  Condition that the conversion attribution attribute is computed. See more about [Conditions](../../../../../annotation/conditions.md)
* **Look-back model:** determines how credit for sales and conversions is assigned to touchpoints in conversion paths. For example, the Last Interaction model in Analytics assigns 100% credit to the final touchpoints (i.e., clicks) that immediately precede sales or conversions. In contrast, the First Interaction model assigns 100% credit to touchpoints that initiate conversion paths
  * **First touchpoint:** the first touchpoint occurring before conversion
  * **Last touchpoint:** the last touchpoint occurring before conversion
  * **Last Non-direct touch:** the touch point occurring most recently (the point before the last touchpoint) before conversion
* **Look-back window:** The time window used to look back from the conversion event to determine which touchpoint will be credited to the conversion
* **Look-back event:** the event lead to conversion
* **Look-back source:** sources that the data is logged lead to conversion
* **Look-back attribute:** attributes of Data objects lead to conversion
* **Display Format**: the displayed value of the attribute. See more about [Display Format](../../../../../annotation/data-format.md#display-format)
* **Look-back condition:** Advanced conditions of look-back event
* **Attribute usage setting**:
  * **Auto suggestion:** use this option if you want to use this attribute suggested in filters
  * **Enable Data Encryption**: mark data encoding for this attribute

{% hint style="warning" %}
Note:&#x20;

* The display format is corresponding with the selected event and event attribute
* You can edit the display format by clicking ![](<../../../../../.gitbook/assets/image (2297).png>)in the Display format field when the data type is Number or Date time
{% endhint %}

### Computation schedule

The schedule that the attribute is computed

See more about the [Computation Schedule](broken-reference)

### Notification Setup

* **Account:** set up account(s) receiving notification&#x20;
* **Notify options**: the notification can be sent by email or pushed notification when the computation completes success or fail

_**Example**_: Find the last Campaign ID which showed an SMS Ad that lead the customer to make a transaction in the last 7 days

![](<../../../../../.gitbook/assets/image (1772).png>)

![](<../../../../../.gitbook/assets/image (807).png>)
