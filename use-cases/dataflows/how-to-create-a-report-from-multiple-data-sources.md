---
description: >-
  This document will assist you in joining two tables - one from a Google Sheet
  file and another from SQL Workspace - to create a comprehensive report.
---

# How to create a report from multiple data sources?

This is your data table from the **SQL Workspace**:

<figure><img src="../../.gitbook/assets/image (3487).png" alt=""><figcaption></figcaption></figure>

This is your data table from **Google Sheets**:

<figure><img src="../../.gitbook/assets/image (2576).png" alt=""><figcaption><p>Google Sheets</p></figcaption></figure>

Below is a **step-by-step guide** on how to create a **data flow that joins these sources** together.

## Step 1: Create data sources

To create a data source, please refer to[ this guide](../../dataflows/data-source/create-a-data-source.md).

_Notes: Please proceed to create **two distinct data sources** - one for the SQL data table and another for the Google Sheets document._

## Step 2: Create data destinations

To create a data destination, please refer to [this guide](../../dataflows/data-destinations/create-a-data-destination.md).&#x20;

_Notes: To create a **data source for a report**, choose the corresponding option in the data flow settings, and **refrain from creating a data destination for it**._

## Step 3: Create the data flow&#x20;

Hover your mouse over **Data**, choose **Batch stream.**&#x20;

<figure><img src="../../.gitbook/assets/image (3488).png" alt=""><figcaption></figcaption></figure>

Click on the **+** button to initiate the creation of a new data flow.

<figure><img src="../../.gitbook/assets/image (3489).png" alt=""><figcaption></figcaption></figure>

Choose 1 of the 2 data sources that you created.

<figure><img src="../../.gitbook/assets/image (3490).png" alt=""><figcaption></figcaption></figure>

Choose the fields you need in the **first data source**.

<figure><img src="../../.gitbook/assets/image (3494).png" alt=""><figcaption></figcaption></figure>

To incorporate **additional data sources** into your dataflow, choose the **Add Data** node. Then select the expected data sources.

<figure><img src="../../.gitbook/assets/image (3491).png" alt=""><figcaption></figcaption></figure>

_Notes: Please refer to_ [_this guide_](../../dataflows/dataflows/creating-a-dataflows/action-node/add-data.md) _for working on the **data source** node._

Also choose the fields you need in the **second data source**.

<figure><img src="../../.gitbook/assets/image (3495).png" alt=""><figcaption></figcaption></figure>

Once you have set up the required data sources, utilize the **Join** action node to combine these sources based on specific conditions.

<figure><img src="../../.gitbook/assets/image (3496).png" alt=""><figcaption></figcaption></figure>

_Notes: Please refer to_ [_this guide_](../../dataflows/dataflows/creating-a-dataflows/action-node/join.md) _for working on the '**Join**' action node._

Once you have joined the data sources, utilize the '**Branch**' function to divide the joined data into separate data destinations.

<figure><img src="../../.gitbook/assets/image (3497).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (3498).png" alt=""><figcaption><p>Add 'Branch' node to break the data destinations</p></figcaption></figure>

_Notes: Please refer to_ [_this guide_](../../dataflows/dataflows/creating-a-dataflows/action-node/branch.md) _for working on the '**Branch**' action node._

To push the joined data for creating a **report**, utilize the (**1**) data destination. Alternatively, if you intend to push the joined data to a **Business Object**, use the (**2**) data destination.

<figure><img src="../../.gitbook/assets/image (3500).png" alt=""><figcaption></figcaption></figure>

To add a **Business Object** destination, click the **+** button at a branch, and choose the destination.

<figure><img src="../../.gitbook/assets/image (3499).png" alt=""><figcaption></figcaption></figure>

To **filter data** and direct it to the **appropriate data destination**, you can achieve this by writing queries using the **Filter** node.

Before proceeding to apply filters, it's essential to grasp the context. Your objective is to join data from multiple sources, where **unmatched data** will be imported to Business Object, and **matched data** will be used to create the report.

This matching result is achieved by applying an **All Row** condition, which matches data based on **email addresses**.

<figure><img src="../../.gitbook/assets/image (3501).png" alt=""><figcaption></figcaption></figure>

To filter out **customers** who **do not exist** in the **SQL data table** but **exist** in **Google Sheets**, apply the filter condition **Email is null**.

<figure><img src="../../.gitbook/assets/image (3502).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (3504).png" alt=""><figcaption></figcaption></figure>

To filter out **customers who exist** in the **SQL data table** but **do not exist** in **Google Sheets**, apply the filter condition **Email address is null**.

<figure><img src="../../.gitbook/assets/image (3505).png" alt=""><figcaption></figcaption></figure>

_Notes: Exercise caution while applying filtering conditions using "**include**" and "**exclude**" to avoid unintended data omissions._

## Result&#x20;

Navigate to the Data Sources of Insights, and find your **Save Data**.

<figure><img src="../../.gitbook/assets/image (3506).png" alt=""><figcaption></figcaption></figure>
