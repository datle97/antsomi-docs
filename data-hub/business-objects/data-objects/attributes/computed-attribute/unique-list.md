---
description: Unique List returns a list of unique values ​​of an event attribute
---

# Unique List

## Unique List Configure

### General Information

* **Object:** the corresponding Object that you chose to create the attribute
* **Group attribute:** Group contains attributes that have the same characteristic or usage. [See more about Groups](../../groups.md)
* **Attribute type:** [type of attribute](unique-list.md#kieu-thuoc-tinh) you chose to create
* **Attribute name:** name of the attribute
* **Attribute internal code:** code of the attribute
* **Description:** information describes the attribute

{% hint style="warning" %}
Note: the attribute code does not allow prefixes: number\_, sgmt\_, aud\_&#x20;
{% endhint %}

<figure><img src="../../../../../.gitbook/assets/image (3737).png" alt=""><figcaption></figcaption></figure>

### Setting

* **Time range**: time range that this attribute is computed
* **Events:** the event will be computed
* **Sources**: sources that event is logged
* **Event Attribute**: attribute of the event
* **Sort by**: you can sort by _**Tracked time**_ or _**Frequency**_
* **Sort order**: you can sort by _**Ascending**_ or _**Descending**_
  * **Get all elements (Maximum 100 elements):** the list contains all elements (Maximum 100 elements)
  * **Get the top \_\_ elements (Maximum 100 elements):** the list contains the top \_\_ of elements (Maximum 100 elements). For instance, get _**the top 3 elements**_
* **Add condition**: Condition that the unique list attribute is computed. See more about [Conditions](../../../../../annotation/conditions.md)
* **Attribute usage setting**:
  * **Enable Data Encryption**: mark data encoding for this attribute

<figure><img src="../../../../../.gitbook/assets/image (3738).png" alt=""><figcaption></figcaption></figure>

### Computation schedule

The schedule that the attribute is computed

See more about the [Computation Schedule](broken-reference)

### Notification Setup

* **Account**: set up account(s) receiving notification&#x20;
* **Notify options**: the notification can be sent by email or pushed notification when the computation completes success or fail

<figure><img src="../../../../../.gitbook/assets/image (3739).png" alt=""><figcaption></figcaption></figure>

_**For example**_, find the top 3 most purchased brands of the year

<figure><img src="../../../../../.gitbook/assets/image (3740).png" alt=""><figcaption></figcaption></figure>
