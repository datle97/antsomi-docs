---
description: >-
  This document proves to be valuable if you intend to transfer data from
  dataflow to the segment.
---

# Export to CDP 365 Segment

## Step 1: Create a destination for CDP 365 Segment.

Please view the details [here](../../../data-destinations/data-destinations-connectors/cdp-segment.md).

## Step 2: Generate a dataflow to preprocess the data.

You can use this information as a [reference ](../)for creating a dataflow.

## Step 3: Select the option 'Export data to Segment'.

1. Add a node.
2. Choose the Destination channel.
3. Select the destination you have previously created for exporting the segment.
4. Select the option '**Export data to Segment**'.

<figure><img src="../../../../.gitbook/assets/image (394).png" alt=""><figcaption><p>Select the Export data to Segment</p></figcaption></figure>

## Step 4: Set up the selected destination.

It has 3 parts of settings.

1. [The condition of the data inputted into the segment](export-to-cdp-365-segment.md#1.-the-condition-of-the-data-inputted-into-the-segment.).
2. [The matching attributes and corresponding values are required to create the segment](export-to-cdp-365-segment.md#2.-the-matching-attributes-and-corresponding-values-are-required-to-create-the-segment.).
3. [The method used for updating the segment](export-to-cdp-365-segment.md#3.-the-method-used-for-updating-the-segment.).

<figure><img src="../../../../.gitbook/assets/image (2647).png" alt=""><figcaption><p>Set up the 'Export data to Segment'</p></figcaption></figure>

### 1. The condition of the data inputted into the segment.

It has&#x20;

* [Source](export-to-cdp-365-segment.md#source)
* [Select Segment](export-to-cdp-365-segment.md#select-segment)
* [Logic](export-to-cdp-365-segment.md#logic)

<figure><img src="../../../../.gitbook/assets/image (2648).png" alt=""><figcaption><p>Conditions</p></figcaption></figure>

1.  #### Source

    To create a **Customer segment**, choose the '**Customer**' option; otherwise, select the '**Visitor**' option to create a **Visitor segment**.
2.  #### Select Segment

    To **update the data into a segment** in CDP 365, please **select** the desired segment from the available options.

    * **Create new audience**: To create a new segment, simply **input** the desired **name** into the 'Segment name' placeholder.
    *   **Existing segment**: If you wish to upload data to an existing segment, please **select** the appropriate segment name from the **available options**.&#x20;

        _**Please find the&#x20;**<mark style="color:red;">**notices for the 'existing segment'**</mark>**&#x20;option below**_.

        <figure><img src="../../../../.gitbook/assets/image (2649).png" alt=""><figcaption><p>Select an existing segment</p></figcaption></figure>

        * _The available options include segments created using **various methods**, such as Conditions, Matching files, and empty segments._
        * _When you select a condition segment or an empty segment, the member update method will **be changed to the 'Matching file' method**._
3.  #### Logic

    Utilizing the data result from the dataflow to create a segment is equivalent to creating a segment using the '**Matching file**' method.

    * OR
    * AND

<figure><img src="../../../../.gitbook/assets/image (2653).png" alt=""><figcaption><p>Logic</p></figcaption></figure>

### 2. The matching attributes and corresponding values are required to create the segment.

You specify the **values** that the **segment** members will **possess**.

* None: null value.
* Set value: input a specific value.

<figure><img src="../../../../.gitbook/assets/image (2654).png" alt=""><figcaption><p>Column matching</p></figcaption></figure>

### 3. The method used for updating the segment.

* **Replace the current audiences**: All members in the selected (existing) segment will be substituted with new members who meet the specified conditions.
* **Add more audiences**: All existing members in the selected (existing) segment will be retained, and new members who meet the conditions will be included as well.

<figure><img src="../../../../.gitbook/assets/image (2655).png" alt=""><figcaption><p>Write mode</p></figcaption></figure>
