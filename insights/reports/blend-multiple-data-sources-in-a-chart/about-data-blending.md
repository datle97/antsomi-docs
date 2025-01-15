---
description: >-
  Join information from multiple sources to get a more unified view of your
  data.
---

# About data blending

By default, charts in Insights get their information from a single data source. Blending lets you create charts based on multiple data sources, called a _blended data source_. For example, you can blend two different Google Analytics data sources to measure the performance of your app and website in a single visualization.

Blending can reveal valuable relationships between your data sets. Creating blended charts directly in Insights removes the need to manipulate your data in other applications first, saving you time and effort.

### How blending works <a href="#how-blending-works" id="how-blending-works"></a>

You create a blended data source by joining the records in one data source to the records of up to 4 other data sources. To join the data, each data source in the blend must share a set of one or more dimensions, known as a _join key_. Blended data sources include all the records from the leftmost data source in the _Blend Data_ panel, and the records from the data sources to the right that share the same values across the join key.

For example, the screenshot below shows the _Blend Data_ panel with 3 data sources: Website A, Website B, and Mobile Apps A. The join key is the _Source_ dimension. The blended data source created from this includes all the records from Website A, along with any records from Website B and Mobile Apps A that share the same _Source_ values as Website A.

<figure><img src="../../../.gitbook/assets/image (959).png" alt=""><figcaption><p>Example of joining 3 data sources.</p></figcaption></figure>



#### Blending is a left outer join

In data science terms, a blended data source is the product of a _left outer join_ operation. In a left outer join of table A and table B, the result is all the records of Data source A and those records in Data source B that share the same key values.

The diagram below illustrates a left outer join of data sources A and B. The blended data source includes all the records contained by the green circle.

<figure><img src="../../../.gitbook/assets/image (1947).png" alt=""><figcaption><p>Venn diagram of a left outer join.</p></figcaption></figure>

#### Blended data sources are report-only

Blended data sources only exist in reports: you won't see them in your DATA SOURCES Home page.

#### **Blending may return more rows than the original data**

Blended data sources include all the records from the leftmost data source in the _Blend Data_ panel, as well as all the records from the data sources to the right that share the same values across the join key. When there are multiple matches for the join condition, this can result in more rows appearing in the blended data than exist in the leftmost data source.

### Blend using multiple dimensions

You can blend data sources using multiple dimensions as the join key. Each data source in the blend must have the same set of dimensions used in the key. Here's an example:

<figure><img src="../../../.gitbook/assets/image (1233).png" alt=""><figcaption><p>Example of a multi key join.</p></figcaption></figure>

In this blend, only the records from Store Orders that match both Sales Rep ID and Region in Sales Reps will be included in the data source.

### Blend a data source with itself <a href="#blend-a-data-source-with-itself" id="blend-a-data-source-with-itself"></a>

You can blend a data source with itself. To do this, add the same data source more than once in the _Blend Data_ panel.

For example, the Google Analytics connector contains metrics for _1 day active users_, _7 day active users_, and _28 day active users_. But, due to a limitation of Analytics, you can only have one of these metrics in a chart at a time. By joining the same Analytics data source with itself, you can add each of these metrics to the blended data source. You can then compare each of these active users metrics in the same chart.

### Use blending to reaggregate data

Calculated fields that are the result of aggregation functions generally can't be reaggregated (they have a type of Auto, which can't be changed). You can work around this by using data blending. [Learn how](https://support.google.com/datastudio/answer/9429470).

### Manage blended data sources <a href="#manage-blended-data-sources" id="manage-blended-data-sources"></a>

Blended data sources in a report are listed in the DATA tab of the properties panel, under Component Data Sources.

Removing a blended data source will break any charts that depend on it, but will not remove the underlying data sources themselves. Any data sources you've added will still be attached to the report.

### Limits of blending data <a href="#limits-of-blending-data" id="limits-of-blending-data"></a>

Blended data sources belong to the report in which they were created. To reuse a blended data source in another report, copy and paste a component with blended data into the new report.

You can blend up to 5 data sources in a chart.

Blending data currently only supports left outer join operations.
