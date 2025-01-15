# Conversion Event

## I - Introduction

A conversion event is a specific user action which marketers want their campaign to convert. Depending on their purposes, CDP 365 users are able to define which Engagement event is the Conversion event and the order of contribution events - the interaction customers/ visitors make before they convert.

## II - Overview

To locate this function, hover your mouse over **Data**, then choose **Conversion**.

<figure><img src="../../.gitbook/assets/image (3649).png" alt=""><figcaption></figcaption></figure>

This app includes 2 tab:&#x20;

* Customer Conversion: The list of Conversion Events created for Customer object
* Visitor Conversion: The list of Conversion Events created for Visitor object

<figure><img src="../../.gitbook/assets/image (3650).png" alt=""><figcaption></figcaption></figure>

### How to create a new Conversion Event?

In order to create a new Conversion Event, click button <img src="../../.gitbook/assets/image (286).png" alt="" data-size="line"> and choose the type of conversion you want.

<figure><img src="../../.gitbook/assets/image (3651).png" alt=""><figcaption></figcaption></figure>

Then, configure the Conversion Event according to your demand.

#### General Information

* Event Group: The type of event you are creating. It's in Conversion group by default.
* Customer/ Visitor Conversion name: The name of the event
* Description: A short text describes your event
* Internal name: The internal code which is automatically generated when you type the Conversion event name
* Icon: Choose or upload an icon to symbolize your event

<figure><img src="../../.gitbook/assets/image (3653).png" alt=""><figcaption></figcaption></figure>

#### Attribution rule

These settings are the rule to calculate the Conversion.

* _Conversion event:_ It is the event which is marked as a conversion every time it happens. You could choose the event, event sources you want by clicking on the dropdown list.
* _When conversion event occurs, Conversion will be calculated:_

Immediately: The system will start calculating right after the data has synchronized&#x20;

Specific: The system will start calculating after a specific period set by user since the time data has synchronized

<figure><img src="../../.gitbook/assets/image (3655).png" alt=""><figcaption></figcaption></figure>

* _Attribution mod&#x65;_&#x6C; - The attribution model determines how much credit each ad interaction gets for your conversions. CDP 365 currently use Data-driven model.&#x20;
* _Contribute events:_ Define the events and its order from which the Conversion Event will be counted.&#x20;

<figure><img src="../../.gitbook/assets/image (3656).png" alt=""><figcaption></figcaption></figure>

The list of event includes 3 events:&#x20;

* _Ads might be viewed:_ The campaign that were sent to approach your customers/ visitors.
* _Ads clicked:_ The campaign that were clicked by your customers/ visitors.
* _Promotion code used:_ There is a code used in a transaction\\

Conversion window: The time range used to calculate the conversion (From the time the event happens). You could choose the time by days or by minutes.

There are **maximum 3 events**. To add a new event, click ![](<../../.gitbook/assets/image (3657).png>)

The order of the event is arrange from the top to the bottom.



After filling out all the necessary information, click **Save** to create the event.

<figure><img src="../../.gitbook/assets/image (3659).png" alt=""><figcaption></figcaption></figure>

### How a conversion event is used to set goal in Customer Journeys?

To measure the conversion in your Customer Journeys, use Journey goals field. Each Conversion event created in Data Hub module is considered a goal. You could add maximum two goals following a specific order (Record the First, then the Second goal).

Every time a goal is reached (In other words, a conversion event happened),  the system will calculate to see which event lead to this conversion following the attribution rule set in the [Conversion Event Config](conversion-event.md#attribution-rule).

<figure><img src="../../.gitbook/assets/image (3660).png" alt=""><figcaption></figcaption></figure>
