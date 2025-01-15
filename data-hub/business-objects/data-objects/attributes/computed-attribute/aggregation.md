---
description: It helps you aggregate values ​​of an event attribute into a single value
---

# Aggregation

## Aggregation Configure

<figure><img src="../../../../../.gitbook/assets/image (3715).png" alt=""><figcaption></figcaption></figure>

### General Information

* **Object:** the corresponding Object that you chose to create the attribute
* **Group attribute:** Group contains attributes that have the same characteristic or usage. [See more about Groups](../../groups.md)
* **Attribute type:** [type of attribute](aggregation.md#kieu-thuoc-tinh) you chose to create
* **Attribute name:** name of the attribute
* **Attribute internal code:** code of the attribute
* **Description:** information describes the attribute

{% hint style="warning" %}
Note: the attribute code does not allow prefixes: number\_, sgmt\_, aud\_&#x20;
{% endhint %}

<figure><img src="../../../../../.gitbook/assets/image (3716).png" alt=""><figcaption></figcaption></figure>

### Setting

* **Time range**: time range that this attribute is computed
* **Aggregation type:** Sum, Max, Min, Average
* **Events:** the event will be computed
* **Sources**: sources that event is logged
* **Event Attribute**: attribute of the event
* **Add condition**: Condition that the aggregation attribute is computed. See more about [Conditions](../../../../../annotation/conditions.md)
* **Display Format**: the displayed value of the attribute. See more about [Display Format](../../../../../annotation/data-format.md#display-format)
* **Attribute usage setting**:
  * **Enable Data Encryption**: mark data encoding for this attribute

{% hint style="warning" %}
Note:&#x20;

* The display format is corresponding with the selected event and event attribute
* You can edit the display format by clicking ![](<../../../../../.gitbook/assets/image (2297).png>)in the Display format field when the data type is Number or Date time
{% endhint %}

<figure><img src="../../../../../.gitbook/assets/image (3717).png" alt=""><figcaption></figcaption></figure>

### Computation schedule

The schedule that the attribute is computed

See more about the [Computation Schedule](broken-reference)

### Notification Setup

* **Account:** set up account(s) receiving notification&#x20;
* **Notify options**: the notification can be sent by email or pushed notification when the computation completes success or fail

<figure><img src="../../../../../.gitbook/assets/image (3718).png" alt=""><figcaption></figcaption></figure>

_**For example**_, calculate the average number devices of Smartphones and Tablets used when clicking on ads in campaigns Campaign 1, Campaign 2

<figure><img src="../../../../../.gitbook/assets/image (3719).png" alt=""><figcaption></figcaption></figure>
