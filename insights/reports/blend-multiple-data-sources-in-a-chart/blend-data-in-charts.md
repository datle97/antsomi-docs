---
description: Learn how to create blended charts and configure blended data sources.
---

# Blend data in charts

You can create charts that show data from multiple data sources. In Insights, this is called _blending data_. There are two ways to create a chart with blended data:

### Add data sources to an existing chart <a href="#add-data-sources-to-an-existing-chart" id="add-data-sources-to-an-existing-chart"></a>

This method blends new data sources into an existing, single data source chart.

1. Edit your report.
2. Select an existing unblended chart.
3. On the right, in the _Data Source_ section of the _DATA_ properties panel, click **+BLEND DATA**.

This creates a blended data source. The _Blend Data_ panel opens, where you can configure the blended chart by adding more data sources, specifying the [join keys](https://support.google.com/datastudio/answer/9194315), adding or removing fields, etc. See below for details.

### Edit a blended data source <a href="#edit-a-blended-data-source" id="edit-a-blended-data-source"></a>

Blending data in a chart creates a blended data source and attaches it to the chart. To edit the blended data source:

1. Edit the report.
2. Select the chart that uses the blended data source.
3. In the _DATA_ properties tab, under _Data Source_, click <img src="../../../.gitbook/assets/image (2401).png" alt="" data-size="line"> to the left of the data source name.

This opens the _Blend Data_ panel, where you can configure the blended data source.

#### Add a new data source <a href="#add-a-new-data-source" id="add-a-new-data-source"></a>

You can blend up to five data sources in a single chart.

To add a data source, click **ADD ANOTHER DATA SOURCE** in an empty data source panel.

#### Select a different data source <a href="#select-a-different-data-source" id="select-a-different-data-source"></a>

Click the data source name in a panel to select a different data source. You can select any data source that has already been added to the report. You can also add any data source to which you have access.

If the new data source has different fields from the old one, you may see [missing fields in the join key](https://support.google.com/datastudio/answer/9061421?hl=en\&ref_topic=9061419#missing-fields-in-join-keys).

#### Shift a data source <a href="#shift-a-data-source" id="shift-a-data-source"></a>

The position of a data source in the Blend Data panel matters: data sources to the left take precedence over those to the right when selecting records to join. The leftmost data source provides the master set of records to include in the blend, while records in data sources to the right are included only if they match the join keys.

To shift a data source, in that data source's panel, click **More** <img src="https://lh3.googleusercontent.com/oLoRPrHJd7m46sWijX6zBWnEnfslP62AxJSwt5Nj0bNbpaYHz2pyscExleiofsH2kQ=h36" alt="More" data-size="line">, then click **Shift left/right**.

#### Remove a data source <a href="#remove-a-data-source" id="remove-a-data-source"></a>

To remove a data source, in that data source's panel, click **More** <img src="https://lh3.googleusercontent.com/oLoRPrHJd7m46sWijX6zBWnEnfslP62AxJSwt5Nj0bNbpaYHz2pyscExleiofsH2kQ=h36" alt="More" data-size="line">, then click **Remove data source**.

Removing a data source only removes it from the blended data, not from the report.

#### Edit the join key <a href="#edit-the-join-key" id="edit-the-join-key"></a>

When you create a blend from a set of charts, Insights automatically creates a join key for you. You can change how the data sources are joined by adding to or removing dimensions from the join key.

When customizing the join key, only select fields that exist in all the data sources. The field names can differ, but the data must match in order to establish the relationship between the data sources. For example, you could use fields called "Date" in one data source, and "Day" in another as long as both fields contain matching dates.

To add a dimension, drag it from the _Available Fields_ list to the right of each data source panel. (If the _Available Fields_ panel is hidden, expand it by clicking **>**.)

To remove a dimension, hover over it and click ![Close](https://lh3.googleusercontent.com/BI114XQ7VNuh_Sl-WpTcIozPJM0D4I8lBRsd7us-kLUr1VxBiGFZCDr6K6q84MgNQuI=w18).

<figure><img src="../../../.gitbook/assets/image (621).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (626).png" alt=""><figcaption></figcaption></figure>

**Missing fields in join keys**

If Insights can't join your data with the currently selected dimensions, you will see one or more pink "Missing" fields in the join key. To fix this, add different dimensions to the key, or remove the missing fields.

<figure><img src="../../../.gitbook/assets/image (1696).png" alt=""><figcaption><p>Example of missing join keys.</p></figcaption></figure>

#### Add fields to the blended data source <a href="#add-fields-to-the-blended-data-source" id="add-fields-to-the-blended-data-source"></a>

A blended data source contains only the fields you specify. The _Fields to include in data source_ section of each data source panel shows the fields contributed by that data source. You can see the complete list of fields in the blended data source on the far right, under _Included Fields_.

To add fields to the blended data source, drag them from the _Available Fields_ panel in the selected data source to an open slot under _Fields to include in data source_. To replace an existing field, drop the new field on top of the old one.

You can edit field names, aggregations, and date display types by clicking the field's data type icon (to the left of the field name).

#### Limit the number of records in the blended data source <a href="#limit-the-number-of-records-in-the-blended-data-source" id="limit-the-number-of-records-in-the-blended-data-source"></a>

To improve performance, as well as help you focus on the data that's most important to you, limit the size of the blended data by applying a[ filter](broken-reference) or [date range](broken-reference). These options appear below the _Fields to include in data source_ section of each data source in the blend.&#x20;

Restricting the records in the leftmost data source controls the overall selection of records for the blended data source.

#### Rename the blended data source <a href="#rename-the-blended-data-source" id="rename-the-blended-data-source"></a>

Edit the **Data source name** field at the top right of the _Blend Data_ panel.
