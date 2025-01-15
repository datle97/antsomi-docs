---
description: >-
  This document offers valuable guidance if you intend to import data from
  external sources into CDP 365 for the purpose of generating segments or
  applying filters within customer journeys.
---

# Export to CDP 356 Events

## Step 1: Create a destination for the CDP 365 Event.

Please view the details [here](../../../data-destinations/data-destinations-connectors/cdp-event.md).

## Step 2: Generate a dataflow to preprocess the data.

You can use this information as a [reference ](../)for creating a dataflow.

## Step 3: Select the option 'Export data to Event'.

1. Add a node.
2. Choose the Destination channel.
3. Select the destination you have previously created for exporting the event.
4. Select the option '**Push Data to CDP Event**'.

<figure><img src="../../../../.gitbook/assets/image (2763).png" alt=""><figcaption><p>Push data to CDP event</p></figcaption></figure>

## Step 4: Select the event source.

After choosing the destination, it is imperative to select the **specific event source** through which the data originated.

<figure><img src="../../../../.gitbook/assets/image (2764).png" alt=""><figcaption><p>Select an event source</p></figcaption></figure>

## Step 5: Select the event.

After choosing the destination, it's essential to then **pick the precise event** that will be the recipient of the data.

<figure><img src="../../../../.gitbook/assets/image (2765).png" alt=""><figcaption><p>Select an event</p></figcaption></figure>

The checkbox governs whether your data will be **utilized within the journey or not**. Enabling the checkbox will prevent the **trigger function** of your data in customer journeys at a later time.

<figure><img src="../../../../.gitbook/assets/image (2766).png" alt=""><figcaption><p>Not trigger journey</p></figcaption></figure>

## Step 6: Set up the selected destination.

