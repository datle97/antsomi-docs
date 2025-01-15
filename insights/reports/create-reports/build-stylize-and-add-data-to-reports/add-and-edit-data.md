# Add and edit data

## Fields in reports

Learn how dimensions and metrics work in your reports.

This article describes how dimensions and metrics are handled in reports.

In Insights, a [chart ](broken-reference)displays data from one or more fields. These fields are the dimensions and metrics provided by the data source attached to that chart. How the data appears depends on the type of chart and how you've styled it.

### How data appears in your charts <a href="#how-data-appears-in-your-charts" id="how-data-appears-in-your-charts"></a>

In **tables**, the data appears in rows and columns, such as in this example based on a Google Sheet data source:

| Sale date    | Product ID | Sale Quantity | Unit Price |
| ------------ | ---------- | ------------- | ---------- |
| Jan 01, 2021 | P001XL     | 280           | 100.000    |
| Jan 01, 2021 | A102XS     | 300           | 250000     |
| Jan 02, 2021 | P002L      | 528           | 245000     |
| Jan 02, 2021 | P002M      | 210           | 230000     |
| Jan 02, 2021 | A102XXL    | 321           | 241000     |
| ...          |            |               |            |

In **Cartesian charts**, dimensions are typically laid out along the horizontal (X) axis, while metrics values provide the vertical (Y) axis positioning. In a time series, the date range dimension provides the X axis and a breakdown dimension provides the data series.

<figure><img src="../../../../.gitbook/assets/image (897).png" alt=""><figcaption></figcaption></figure>

In a **pie chart**, a dimension defines the number of segments, while a metric determines the size of each segment.

<figure><img src="../../../../.gitbook/assets/image (2456).png" alt=""><figcaption></figcaption></figure>

**Geo charts** use a dimension that contains geographic information (such as a country code, latitude and longitude, or Google Ads Criteria ID) to display your data on a map. The relative values of the metric determine the intensity of color on the chart, as show in this example showing that the majority of website sessions occurred in the United States:

<figure><img src="../../../../.gitbook/assets/image (2534).png" alt=""><figcaption><p>Example geo chart showing Sessions.</p></figcaption></figure>

\
​[Learn more about the charts you can use in Data Studio](https://app.gitbook.com/o/-LzunofLVjpTa_-p1PQt/s/13P8l3kHXpB6Md6CLuQh/insights/reports/create-reports/build-stylize-and-add-data-to-reports/chart-references).

#### Use breakdown dimensions to group data <a href="#use-breakdown-dimensions-to-group-data" id="use-breakdown-dimensions-to-group-data"></a>

Many charts allow you to group your data by multiple dimensions. Each dimension you add to the chart groups the data into ever finer levels of detail. The first dimension in the chart is the primary; additional dimensions are called _breakdown_ _dimensions_ (because they allow you to breakdown or sub-categorize your data into smaller chunks).For example, in the following table, the primary dimension is _Country_, and the breakdown dimension is _Year_. The metrics in the table are aggregated first by country, then by year. (See below for more on how grouping affects metric calculation).

| Country | Year | Population | Internet Users | Internet % |
| ------- | ---- | ---------- | -------------- | ---------- |
| Iceland | 2013 | 323,764    | 312,583        | 96.55%     |
| Iceland | 2012 | 320,716    | 308,560        | 96.21%     |
| Bermuda | 2013 | 65,001     | 61,945         | 95.30%     |
| Norway  | 2013 | 5,079,623  | 4,828,354      | 95.05%     |
| Iceland | 2011 | 319,014    | 302,488        | 94.82%     |
| ...     | ​    | ​          | ​              | ​          |

Making sense of multi-dimensional data in a table can be challenging. Using other visualization types, such as this stacked bar chart, can help make sense of complex data.

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F13P8l3kHXpB6Md6CLuQh%2Fuploads%2Fssy5SwYg0Xznral40tUR%2Fimage.png?alt=media&#x26;token=fb6503f9-3026-4896-a607-7a333c220491" alt=""><figcaption></figcaption></figure>

### How metrics are calculated <a href="#how-metrics-are-calculated" id="how-metrics-are-calculated"></a>

In Insights, metrics are calculated in two basic ways:

**As overview totals**

Metrics can be displayed as a summary statistic for the entire column (field) in your data set using the [Scorecard](broken-reference) chart.

The example below shows simplified data from Google Analytics. Here, the _Avg. Time on Site_ metric is summarized for all users, regardless of any other consideration, such as whether they are new or returning visitors. The calculations for time on site are computed using the time difference between each user's initial session and the exit, with the sum of each session length averaged across three sessions.

![Metric example: overview totals](https://lh3.googleusercontent.com/K0oBuLgmAJskdwobkjfWIEQMW7qdRHkVUo2m9KB5qEeAlpQAW6IaD5I3X1ZKgu93FZA=w366)

**In association with one or more dimensions**

Metric values can be qualified by selected dimension(s). All the other chart types fall into this category.

In the following example, the bar chart pairs the _Avg. Time On Site_ metric with the _User Type_ dimension. This visualization lets you analyze this metric via _returning_ vs _new_ users, where the calculations are modified by the requested dimension.

<figure><img src="../../../../.gitbook/assets/image (1871).png" alt=""><figcaption><p>Metric example: associated with a dimension</p></figcaption></figure>

Adding multiple dimensions to a chart refines your view of the data. For example, suppose you use both the _User Type_ dimension and the _Language_ dimension in a table to analyze time on site for your website. In this case, the calculation for _new_ versus _returning_ users is the same, but that calculation is aggregated per language. Your table might look like this:

| User Type         | Language | Avg. Session Duration |
| ----------------- | -------- | --------------------- |
| Returning Visitor | zh-tw    | 00:04:54              |
| New Visitor       | zh-tw    | 00:04:02              |
| Returning Visitor | en-us    | 00:03:51              |
| New Visitor       | en-us    | 00:03:45              |
| Returning Visitor | en-gb    | 00:03:33              |
| ...               |          |                       |

### Related resources <a href="#related-resources" id="related-resources"></a>

* [Chart references](broken-reference)

## Edit fields in your reports

Change field names, aggregations, data types, and analytical functions at the chart level.

By default, the definition of the fields in your reports matches how those fields are defined in the underlying data source. Specifically, fields in the report have the same name, data type, and aggregation as in the data source.

The **Field Editing in Reports** data source option allows report editors to change field definitions at the chart level. Editing field definitions in the report makes customizing your reports faster and easier. It reduces or even eliminates the need to duplicate fields in the data source in order to apply different aggregations or functions to the same data. It also allows you to have canonical field definitions in the data source, while tailoring the fields to fit different report requirements.

### How editing fields in reports works <a href="#how-editing-fields-in-reports-works" id="how-editing-fields-in-reports-works"></a>

When you create a report based on a data source that has the **Field Editing in Reports** setting turned on, all the fields in the report that use the data source become editable. This option applies to all reports that use that data source. To edit a field definition in a report:

1. Edit the report
2. Select a chart
3. In the chart's _DATA_ properties panel, click the field's data type icon on the left-hand portion of the field.

<figure><img src="../../../../.gitbook/assets/image (4103).png" alt=""><figcaption></figcaption></figure>

#### What you can edit

Editing a field lets you change the following :

* The field's **name**. For example, you can rename _Order Value_ to _Average Order Value_.
* A metric's **aggregation**. For example, you can recalculate _Order Value_ from **Sum** to **Average**.
  * This option isn't available if the field is a metric with Auto aggregation type.
* The field's **data type**. For example, you can convert a **Number** to a **Percent**, or **Text** to a **URL**, or full **Date** to a date part.
* A metric's **comparison calculation**. For example, you can apply a **Percentage of Total** function to your orders.

Learn more about [comparison](add-and-edit-data.md#add-comparison-metrics-and-running-totals)

Any changes you make to a given field only apply to that instance of the field in that chart. For example, if the _Average Order_ field appears in a table and a bar chart in the same report, changing any of the attributes of that field in the table has no effect on the _Average Order_ field in the bar chart.

### Rename a field <a href="#rename-a-field" id="rename-a-field"></a>

You can change a field's display name in the selected chart. This lets you have multiple instances of the same field in a chart. For example, you can add 2 instances of the Order Value field to a table, and change the name of the second instance to _Average Order Value_. Use the aggregation options described below to change how the field is calculated.

### Change the field aggregation <a href="#change-the-field-aggregation" id="change-the-field-aggregation"></a>

A field's aggregation determines how its data is calculated in the chart. You can select from the following aggregations:

* Average
* Count Distinct
* Count
* Max
* Median
* Min
* Sum

Metrics with an aggregation of Auto can't be changed.

### Change the field data type <a href="#change-the-field-data-type" id="change-the-field-data-type"></a>

A field's data type tells Insights what kind of data to expect as input. For example, Insights displays Text fields "as is," with no other processing. Even if the field contains numbers, Insights won't apply any numeric aggregation to it. A field defined as a URL, on the other hand, is displayed as hyperlinks.

When the specified data type and actual data don't match, unexpected results can occur. You can adjust a field's data type in circumstances when the data source hasn't been correctly configured and you don't have edit access to it. For example, converting a dimension containing valid data but defined as Text to a Date type can let you use it as date range dimension.

### Change the date granularity <a href="#show-as-date-options" id="show-as-date-options"></a>

Changing a Date or Date & Time type aggregates the data by the new type. For example, instead of grouping your data by year, month, and day, you can group by year and month.

For example, if the date field contains the complete year, month, and day, you can group by year quarter.

#### Example

The tables below show the same data. The table on the right has the granularity set to YEAR QUARTER. Notice how the data has been aggregated according to the new time unit:

<figure><img src="../../../../.gitbook/assets/image (1783).png" alt=""><figcaption></figcaption></figure>

To change how compatibility mode dates group the data, use the **Granularity** option, **NOT** the Type option.

### Related resources <a href="#related-resources" id="related-resources"></a>

[Dates and Times](broken-reference)

## Add comparison metrics

Compare row data to total in your charts.

You can add metrics that compare each row of your data to the total value of a column.

### Add comparison metrics to a chart

1. Edit your report.
2. Select a chart.
3. In the DATA properties panel, select a metric and click its edit pencil <img src="../../../../.gitbook/assets/image (1873).png" alt="" data-size="line">.
4. Click the **Comparison calculation** menu and select the desired comparison. See below.
5. To display the metric's native value, change the **Comparison calculation** selection to **None**.

#### Compare to total <a href="#compare-to-total" id="compare-to-total"></a>

You can compare each row of data to the overall total for that field:

1. **Percent of total** shows the current row's value divided by the total for that field.

#### Example

The table below shows the results of applying different "compare to total" options to the Order Value field. This lets you evaluate each order's contribution to overall sales.

<figure><img src="../../../../.gitbook/assets/image (704).png" alt=""><figcaption></figcaption></figure>

## Replace the data source for a component

Learn how to switch data sources in your reports.

You can replace the data source for selected charts and controls. Reasons you might want to do this include:

* Copying a report and replacing your data source with a client's data source.
* Switching the data source for a selected component from one account, sheet, or database table to another.

### What happens when you replace a data source

When you replace a data source in your report, Insights tries to map the fields in the old data source to the fields in the new data source based on a number of matching criteria, including field ID, field name, and other configuration information from the report itself. Insights won't try to map your old fields in calculated fields and filters.

If no suitable match is found, your report may display components with the message: **Chart configuration incomplete**\
Invalid/Missing dimensions, metrics, filters.

To fix this, edit the incomplete components and select new dimension, metric, sorting, and/or date range fields.

We strongly recommend you review your entire report for accuracy after replacing any data sources used in the report.

### Replace a component data source

1. Edit your report.
2. Select a charts or controls.
3. On the right, in the selected component's property panel, select the **DATA** tab.
4. At the top of the left-hand panel, click the current data source name.
5. Select an existing data source, or, at the bottom, click **NEW DATA SOURCE**.

Replacing the data source for one component has no effect on the other components in your report.

### Related resources <a href="#related-resources" id="related-resources"></a>

[Blend multiple data sources in a chart.](broken-reference)

## Add data to a report

Create and add data sources to reports and explorations.

The data in your reports comes from a data source. Here's how to add new and existing data sources to your reports.

### Add data to a new report <a href="#add-data-to-a-new-report" id="add-data-to-a-new-report"></a>

1. Sign in Insights
2. Select Report menu
3. In the top left, click <img src="../../../../.gitbook/assets/image (469).png" alt="" data-size="line">
4. Select a datasource from the list of available datasources.
5. Click **Create report**

### Add data to an existing report <a href="#add-data-to-an-existing-report" id="add-data-to-an-existing-report"></a>

1. Edit your report.
2. On the right, in the properties panel of the selected component, select the DATA tab.
3. At the top of the left panel, click the current data source name.
4. Select an existing data source or at the bottom click **+ CREATE NEW DATA SOURCE**
5. If you select **Create New Data Source**, the **Create Data Source dialog box** is displayed.
6. Select the type of data you want to connect. Select a specific dataset and provide your authorization, if necessary. In the upper right, click Connect.

### Create a reusable data source <a href="#create-a-reusable-data-source" id="create-a-reusable-data-source"></a>

Data sources you create from the home page can be used across multiple reports. To create a reusable data source:

1. Sign in Insights
2. Select **Data Source** menu
3. In the upper left, click <img src="../../../../.gitbook/assets/image (1681).png" alt="" data-size="line">
4. Select Data Source, select the type of data you want to connect.
5. Select the specific data set and provide your authorization, if necessary.
6. In the upper right, Click **CONNECT**.
7. In the page that appears, you'll see the list of fields provided by this data source.

To add this data source to a report, in the upper right, click **CREATE REPORT**.

### Rename a data source <a href="#rename-a-data-source" id="rename-a-data-source"></a>

1. Edit the data source
2. In the upper left, next to the Insights logo, click the current name.
3. Enter a new name.
