---
description: >-
  Highlight values of interest in your charts and visualize progress towards
  your goals.
---

# Add reference lines to charts

Reference lines show how the data in a chart compares to a reference value. For example, you can use reference lines to visualize daily sales against a target sales figure, or show the average revenue per store and compare each store to that average.

<figure><img src="../../../../.gitbook/assets/image (1999).png" alt=""><figcaption><p>Reference line example: weekly sales vs. target.</p></figcaption></figure>

### Reference lines vs. trend lines

Reference lines let you show target values and set thresholds and benchmarks so you can see how your data matches expectations or goals.

Trend lines reveal the overall direction of the data in a chart. Trend lines can help you see patterns and make predictions from otherwise random-appearing data. In Insights, you can add trend lines to [time series ](broken-reference)and [scatter charts](broken-reference).

### Add a reference line <a href="#add-a-reference-line" id="add-a-reference-line"></a>

You can add reference lines to time series, line and combo charts, bar and column charts, area charts, and scatter charts.

1. Edit your report.
2. Select a supported chart.
3. On the right, open the **STYLE** properties panel.
4. Click **Add a reference line**.
5. Select the reference line **Type**.\
   You can base a reference line on a constant value, a metric.
6. Configure the reference line using the options below.

You can add up to 10 reference lines per chart.

### Reference line options <a href="#options" id="options"></a>

#### Type

Determines the value upon which the reference line is based.

**Constant value**

Base the reference line on a value you type in. For example, if your sales target is $10,000 per day, enter 10000. For a percentage value, enter the number as a decimal (.5 equals 50%).

**Metric**

Base the reference line on a metric that appears in the chart.

#### Calculation

For metric-based reference lines, choose the aggregation to apply to the selected metric. For example, if the chart is visualizing _Users_ by _Week_, you can create a reference line showing the average number of weekly users by choosing the _Users_ metric and **Average** calculation.

Available calculations:

* Average
* Median
* Percentile
  * Enter the percentile as a whole number from 1 to 99.
* Min
* Max
* Total

#### Axis

Display the reference line on the chart's X, Y, Left-Y, or Right-Y axis. This option applies to constant value-based reference lines. The available axes depend on the chart type.

#### Label

Display a custom label for the reference line.

If you leave this blank, Insights supplies a default label. For constant value reference lines, the label is "Reference Line #n." For metric reference lines, the default label is the type of calculation applied.

#### Line color, weight and style

Set the appearance of the reference line.

<figure><img src="../../../../.gitbook/assets/image (2484).png" alt=""><figcaption><p>Chart showing 90th percentile of reading test scores.</p></figcaption></figure>

_Reference line example showing a 90th percentile calculation on a reading test scor&#x65;_&#x73; _metric, with line color, weight, and style options applied._

### View a reference line <a href="#view" id="view"></a>

Reference lines appear with either a default label, or a custom label you supply. Hover over the line to display a tooltip showing the reference value.

### Remove a reference line <a href="#remove" id="remove"></a>

To remove a reference line from a chart:

1. Edit your report.
2. Select the chart.
3. On the right, open the **STYLE** properties panel.
4. Locate the reference line you want to remove, then click <img src="../../../../.gitbook/assets/image (1701).png" alt="" data-size="line">.

### Edit charts with reference lines <a href="#edit-charts-with-reference-lines" id="edit-charts-with-reference-lines"></a>

If you change the chart type, Insights deletes any reference lines not supported by the new chart type.

If you remove a metric from the chart, Insights deletes any reference lines associated with that metric.

### Limits of reference lines <a href="#limits" id="limits"></a>

* Reference lines are only available for numeric axes. Reference lines on date axes aren't supported.
* Metric-based reference lines can only consider values currently displayed in the chart. For example, if you add a reference line to a bar chart with 10 bars, data from any additional bars aren't included in the calculation.
* You can't add a reference line to 100% stacked charts.
* Stacked column, stacked bar, and stacked area charts only support constant value and parameter reference lines.
