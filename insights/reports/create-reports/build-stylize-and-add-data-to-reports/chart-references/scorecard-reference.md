---
description: How to use and configure scorecards.
---

# Scorecard reference

Scorecards display a summary of a single metric. Scorecards are commonly used to visualize key performance indicators: some variable that measures the relative health or performance of your business or area of activity. For example, a scorecard can summarize total sales, average bounce rate, count of ad impressions, maximum hold time, minimum failure rate, etc.

### Scorecards in Insight <a href="#about-chart" id="about-chart"></a>

Scorecards in Insight appear as numbers, and, optionally, the name of the metric being summarized. The format of the displayed number depends on how the metric is configured in your data source.

**Example:**

The data source for a fictional pet store contains the following metrics. The _Qty Sold_ metric is simply a number coming from the data set. The _Avg Qty Sold_ metric is a duplicate of the _Qty Sold_ field, with the Average aggregation type. _Total Items_, and _Unique Items_ are calculated fields.

| Name         | Calculation            | Aggregation Type |
| ------------ | ---------------------- | ---------------- |
| Qty Sold     | none                   | Sum              |
| Avg Qty Sold | none                   | Average          |
| Total Items  | COUNT(Items)           | Auto             |
| Unique Items | COUNT\_DISTINCT(Items) | Auto             |

Scorecards for these metrics might look like this:

<figure><img src="../../../../../.gitbook/assets/image (2536).png" alt=""><figcaption></figcaption></figure>

### Configure the chart <a href="#configure" id="configure"></a>

Select the chart, then on the right, use the properties panel to configure the chart options.

### Data properties <a href="#data-properties" id="data-properties"></a>

The options in a chart's data properties panel affect how the data is organized and displayed.

#### Data source <a href="#data-source" id="data-source"></a>

A data source provides the connection between the component and the underlying data set. Data source options are:

* To change the chart's data source, click the current data source name.
* To view or edit the data source, click <img src="../../../../../.gitbook/assets/image (1392).png" alt="" data-size="line">. (You must have at least view permission to see this icon.)
* Click **+BLEND DATA** to see data from multiple data sources in the same chart. [Learn more about data blending.](broken-reference)

#### Date range dimension <a href="#date-range-dimension" id="date-range-dimension"></a>

This option appears if your data source has a valid date dimension. For Google Ads and Analytics data sources, this option is automatically set to the _Date_ dimension.

The Date Range Dimension is used as the basis for limiting the date range of the chart. For example, this is the dimension used if you set a date range property for the chart, or if a viewer of the report uses a date range control to limit the time frame.

#### Metric

Metrics measure the things contained in dimensions and provide the numeric scale and data series for the chart.

Add metrics to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add metric** in the _Data_ tab.

#### Default date range <a href="#default-date-range" id="default-date-range"></a>

The default date range property lets you set a timeframe for an individual char&#x74;_._

**Default date range options**

| Auto              | Use the default date range determined by the chart's data source.             |
| ----------------- | ----------------------------------------------------------------------------- |
| Custom            | Lets you use the calendar widget to select a custom date range for the chart. |
| Date compare type | Displays comparison data for the selected time period.                        |

#### Filter <a href="#filter" id="filter"></a>

The filter property restricts the data displayed in the component by including or excluding the values you specif&#x79;_._ [Learn more about the filter property](broken-reference).

**Filter options**

| Filter name   | Click an existing filter to edit it. Mouse over the filter name and click ![](<../../../../../.gitbook/assets/image (1997).png>) to delete it. |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| +Add a filter | Creates a new filter for the chart.                                                                                                            |

### Style properties <a href="#style-properties" id="style-properties"></a>

A chart's style properties control the overall presentation and appearance of the chart.

#### Primary metric

These options control the appearance of the scorecard's current data.

| Compact Numbers   | Rounds numbers and displays the unit indicator. E.g., 553,939 becomes 553.9K. |
| ----------------- | ----------------------------------------------------------------------------- |
| Decimal Precision | Sets the number of decimal places in metric values.                           |

**Comparison metric**

These options control the appearance of the scorecard's previous period comparison data.

| Positive change color | This option appears when date comparison is enabled. Changes the font color used to indicate positively changing (i.e., upward trending) data.   |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| Negative change color | This option appears when date comparison is enabled. Changes the font color used to indicate negatively changing (i.e., downward trending) data. |
| Show absolute change  | This option appears when date comparison is enabled. Changes the comparison display from percentage of change to absolute numeric difference.    |
| Hide comparison label | Hides the label that shows the comparison period.                                                                                                |

#### Labels

This section controls the appearance of the chart labels.

| Font color       | Changes the font color of the scorecard label.                                                                            |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------- |
| Font size        | Changes the font size of the scorecard label.                                                                             |
| Font family      | Changes the font family of the scorecard label.                                                                           |
| Hide Metric Name | Hides the default metric name (which comes from the data source). You can use the Text tool to add a custom metric label. |
| Alignment        | Align the metric name, primary value, and comparison value.                                                               |

#### Missing data <a href="#missing-data" id="missing-data"></a>

This option controls how to display missing values. For example, when data is missing from the table, you can choose to show blanks, hyphens, or the words "no data."

#### Background and border <a href="#background-and-border" id="background-and-border"></a>

These options control the appearance of the chart background container.

| Background        | Sets the chart background color.                                                                                                                           |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Border Radius     | Adds rounded borders to the chart background. When the radius is 0, the background shape has 90° corners. Border radius of 100° produces a circular shape. |
| Opacity           | Sets the chart's opacity. 100% opacity completely hides objects behind the chart. 0% opacity makes the chart invisible.                                    |
| Border Color      | Sets the chart border color.                                                                                                                               |
| Border Weight     | Sets the chart border line thickness.                                                                                                                      |
| Border Style      | Sets the chart border line style.                                                                                                                          |
| Add border shadow | Adds a shadow to the chart lower and right borders.                                                                                                        |

**Padding**

Use these options to control the line height and left, right, and top padding within the chart.

**Chart Header**

The chart header lets viewers perform various actions on the chart such as exporting the data or viewing the chart in the Explorer tool. Chart header options are:

| Show on hover (default) | Three vertical dots appear when you mouse over the chart header. Click these to access the header options.           |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Always show             | The header options always appear.                                                                                    |
| Do not show             | The header options never appear. Note that report viewers can always access the options by right clicking the chart. |
| Color                   | Set the color of the chart header options.                                                                           |

#### **Related resources** <a href="#related-resources" id="related-resources"></a>

* ​[Filter property](https://app.gitbook.com/o/-LzunofLVjpTa_-p1PQt/s/13P8l3kHXpB6Md6CLuQh/insights/reports/filter-your-data/about-filters)
