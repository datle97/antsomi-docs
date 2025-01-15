# Text

## Editor

* You can edit by selecting the text (Font Family, Font Size, Bold, Iatic, Underline, etc.)
* There are 2 dynamic options:&#x20;

_**Insert Link and Smart Tags,**_ you can select the text and insert Link or Smart Tags

<figure><img src="../../../../.gitbook/assets/image (3999).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (4000).png" alt=""><figcaption></figcaption></figure>

* _**Add Personalization**_: Click on Smart Tags, it provides 5 types of Personalization: _**Visitor Attribute, Customer Attribute, Event Attribute, Promotion Code, Product**_
  *   _**Visitor/Customer Attribute**_

      * _**Personalization Attribute**_: Attribute of Visitor/Customer
      * _**Display Format:**_ It depends on the data type of attributes, you can also adjust the date display format

      <figure><img src="../../../../.gitbook/assets/image (4001).png" alt=""><figcaption></figcaption></figure>

      *   _**Event Attribute**_

          * _**In any source of**_: Select the event source
          * _**Select event**_: Select the event corresponding with the source
          * _**Select event attribute:**_ Attribute of the event
          * _**Display Format**_: It depends on the data type of attributes, you can also adjust the date display format

          <figure><img src="../../../../.gitbook/assets/image (4002).png" alt=""><figcaption></figcaption></figure>
      *   _**Promotion Code**_

          * _**Promotion pools**_: The pool contains promotion codes
          * _**Promotion code attribute**_: The attribute of the promotion code

          <figure><img src="../../../../.gitbook/assets/image (4003).png" alt=""><figcaption></figcaption></figure>
      *   _**Product**_

          * _**Personalization attribute**_: The attribute of the Product
          * _**Index**_: The number of the row in the Product attribute data

          <figure><img src="../../../../.gitbook/assets/image (4004).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
When you insert the link, it can be static or dynamic
{% endhint %}

## Settings

<figure><img src="../../../../.gitbook/assets/image (4005).png" alt=""><figcaption></figcaption></figure>

### Display condition

<figure><img src="../../../../.gitbook/assets/image (4006).png" alt=""><figcaption></figcaption></figure>

* _**Condition**_: It includes _**None, Show when, Hidden when**_
* _**Field**_: It contains _**Business Object attributes**_
* _**Index**_: The number of the row in the Business Objects Data table
* _**Operator**_: It includes _**contains, does not contain, starts with, doesn't start with, ends with, doesn't end with**_, etc.
* _**Value**_: you can input the value or select an _**attribute from Business Object or Event**_

### Dynamic Content

When you insert a dynamic link or smart tag, you can also add or remove or highlight Dynamic Content

<figure><img src="../../../../.gitbook/assets/image (4007).png" alt=""><figcaption></figcaption></figure>

#### Add Dynamic Content

Clicking ![](<../../../../.gitbook/assets/image (1353).png>)to change the setting of **Dynamic Content**

<figure><img src="../../../../.gitbook/assets/image (4008).png" alt=""><figcaption></figcaption></figure>

**Dynamic Content** type includes **Visitor Attribute**, **Customer Attribute**, **Promotion code**, **Event Attribute**

* Visitor Attribute and Customer Attribute allows using the attributes of Visitor or Customer Business Object to make dynamic content
* Promotion code uses the attributes of a promotion pool to make dynamic content. For example, if demanding to show the promotion code a customer spin won.&#x20;
* Event attribute uses the event attributes of an event to make dynamic content. For example, if demanding to show the number of items a customer purchased.&#x20;

<figure><img src="../../../../.gitbook/assets/image (4009).png" alt=""><figcaption></figcaption></figure>

#### Visitor Attribute and Customer Attribute

If Personalization type was selected Visitor Attribute or Customer Attribute

* Personalization attribute is the attribute of the Visitor or Customer Business Object
* Display Format is the value format of the attribute

#### Promotion code

If Personalization type was selected Promotion code

* Promotion pool is the promotion pool created in [Promotion Center](../../../promotion-center.md)&#x20;
* Promotion code attribute is the attribute which contains promotion code value sent in the template
* Display Format is the value format of the promotion code attribute

<figure><img src="../../../../.gitbook/assets/image (4010).png" alt=""><figcaption></figcaption></figure>

#### Event Attribute

If Personalization type was selected Event Attribute

* Select event is the event that is required an audience to satisfy to show the dynamic content
* In any source of is the source in which the event happens
* Select event attribute is the event attribute of the selected event that contains values making dynamic content
* Index _(this setting is of the event attribute selected)_ is the position of the values want to show
* Display Format is the value format of the event attribute

<figure><img src="../../../../.gitbook/assets/image (4011).png" alt=""><figcaption></figcaption></figure>

#### Remove Dynamic Content

Clicking ![](<../../../../.gitbook/assets/image (1313).png>)to remove a Dynamic Content

#### Highlight Dynamic Content

Turning on the status to highlight Dynamic Content

<figure><img src="../../../../.gitbook/assets/image (4012).png" alt=""><figcaption></figcaption></figure>

### Text styling

The number of lines displayed in the Preview or Delivery mode.

### Container Styling

<figure><img src="../../../../.gitbook/assets/image (4013).png" alt=""><figcaption></figcaption></figure>

#### **Background color**

Apply background color of Text block.

#### **Border**

It allows adding border, the style, width, and color of an element's border.

#### Rounded Corners

This setting allows make the border of the text rounded.

#### Height

If applying dynamic content, without Height, the height of text blocks could be out of place. With this feature, users could set the certain height for text blocks and the texts are neat.&#x20;

#### **Spacing**

* _**Inner Spacing (Padding):**_ \
  Padding is inside the border (or edge) of your element. Increasing the padding will “push” your content into the middle of your box, away from your borders. If you remove the padding, your content will take up the entire box
* _**Outer Spacing (Margin):**_ \
  Margin is on the outside of the border of your element. If you increase the margin, it will increase the space between this element and the ones next to it. If you remove your margin, there will be no extra space between your elements

#### Z-Index

* The z-index property specifies the stack order of an element
* An element with greater stack order is always in front of an element with a lower stack order

#### Custom ID attribute

The ID of a block, which is used in _**Custom CSS, Custom Javascript**_

#### Custom Class attribute

The class of a block, which is used in _**Custom CSS, Custom Javascript**_

### **Responsive Design**

The specific settings in this section will vary depending on device type designing

**Desktop mode**:

<figure><img src="../../../../.gitbook/assets/image (4014).png" alt=""><figcaption></figcaption></figure>

Hide on Desktop: Hide the Column block when recipient reads the email template on Desktop.

&#x20;

**Mobile mode**:

<figure><img src="../../../../.gitbook/assets/image (4015).png" alt=""><figcaption></figcaption></figure>

Hide on Mobile: Hide the Column block when recipient reads the email template on Mobile.

