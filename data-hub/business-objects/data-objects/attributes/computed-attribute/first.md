---
description: First returns the first received value of the event attribute
---

# First

## First Configure

<figure><img src="../../../../../.gitbook/assets/image (3726).png" alt=""><figcaption></figcaption></figure>

### General Information

* **Object:** the corresponding Object that you chose to create the attribute
* **Group attribute:** Group contains attributes that have the same characteristic or usage. [See more about Groups](../../groups.md)
* **Attribute type:** [type of attribute](first.md#kieu-thuoc-tinh) you chose to create
* **Attribute name:** name of the attribute
* **Attribute internal code:** code of the attribute
* **Description:** information describes the attribute

{% hint style="warning" %}
Note: the attribute code does not allow prefixes: number\_, sgmt\_, aud\_&#x20;
{% endhint %}

<figure><img src="../../../../../.gitbook/assets/image (3727).png" alt=""><figcaption></figcaption></figure>

### Setting

* **Time range**: time range that this attribute is computed
* **Events:** the event will be computed
* **Sources**: sources that event is logged
* **Event Attribute**: attribute of the event
* **Add condition**: Condition that teh first attribute is computed. See more about [Conditions](../../../../../annotation/conditions.md)
* **Display Format**: the displayed value of the attribute. See more about [Display Format](../../../../../annotation/data-format.md#display-format)
* **Attribute usage setting**:
  * **Enable Data Encryption**: mark data encoding for this attribute

{% hint style="warning" %}
Note:

* The display format is corresponding with the selected event and event attribute
* &#x20;You can edit the display format by clicking ![](<../../../../../.gitbook/assets/image (2297).png>)in the Display format field when the data type is Number or Date time
{% endhint %}

<figure><img src="../../../../../.gitbook/assets/image (3728).png" alt=""><figcaption></figcaption></figure>

### Computation schedule

The schedule that the attribute is computed

See more about the [Computation Schedule](broken-reference)

### Notification Setup

* **Account**: set up account(s) receiving notification&#x20;
* **Notify options**: the notification can be sent by email or pushed notification when the computation completes success or fail

<figure><img src="../../../../../.gitbook/assets/image (3729).png" alt=""><figcaption></figcaption></figure>

_**For example**_, find the URL of the first product purchased by the audience in the last 30 days

<figure><img src="../../../../../.gitbook/assets/image (3730).png" alt=""><figcaption></figcaption></figure>
