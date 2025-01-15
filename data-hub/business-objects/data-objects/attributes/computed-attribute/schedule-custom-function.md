---
description: Use formulas for advanced calculations based on computed attributes
---

# Schedule Custom Function

The Schedule Custom Function attribute allows attribute data to be built by schedule. It is strongly convenient and reduces the time to compute when there is a request from the user (Data Object Data-table, Segment, Journey, AM...)

## Schedule Custom Function Configure

<figure><img src="../../../../../.gitbook/assets/image (3749).png" alt=""><figcaption></figcaption></figure>

### General Information

* **Object:** the corresponding Object that you chose to create the attribute
* **Group attribute:** Group contains attributes that have the same characteristic or usage. [See more about Groups](../../groups.md)
* **Attribute type:** [type of attribute](schedule-custom-function.md#kieu-thuoc-tinh) you chose to create
* **Attribute name:** name of the attribute
* **Attribute internal code:** code of the attribute
* **Description:** information describes the attribute

{% hint style="warning" %}
Note: the attribute code does not allow prefixes: number\_, sgmt\_, aud\_&#x20;
{% endhint %}

<figure><img src="../../../../../.gitbook/assets/image (3750).png" alt=""><figcaption></figcaption></figure>

### Edit Info

* **Function**: You can enter functions or drag the suggested on the right of the Function list or Available Attributes
  * **Function list:** includes Operators, string, Math, Calendar/Date, Expression
  * **Available Attributes:** contains a list of available attributes that the user can use in Function
* **Data type of function output:** the data type of function output such as Number, String, Datetime. See more about [Data Type](../../../../../annotation/data-format.md#data-type)
* **Display function output**: display format for the output of the function, it depends on the data type of function output.  See more about [Display Format](../../../../../annotation/data-format.md#display-format)
* **Attribute usage setting:**&#x20;
  * **Enable Data Encryption:** mark data encoding for this attribute

{% hint style="info" %}
CDP 365 supports different functions corresponding with each data type
{% endhint %}

<figure><img src="../../../../../.gitbook/assets/image (3751).png" alt=""><figcaption></figcaption></figure>

### Computation schedule

The schedule that the attribute is computed

See more about the [Computation Schedule](broken-reference)

### Notification Setup

* **Account:** set up account(s) receiving notification&#x20;
* **Notify options**: the notification can be sent by email or pushed notification when the computation completes success or fail

<figure><img src="../../../../../.gitbook/assets/image (3752).png" alt=""><figcaption></figcaption></figure>
