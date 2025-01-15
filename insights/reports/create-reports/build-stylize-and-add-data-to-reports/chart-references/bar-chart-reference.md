---
description: How to use and configure bar charts.
---

# Bar chart reference

A bar chart uses horizontal or vertical bars to show comparisons among categories. The longer the bar, the greater the value it represents. One axis of the chart shows the specific categories (dimensions) being compared, and the other axis represents a discrete value (metric).

### Bar charts in Insights <a href="#about-chart" id="about-chart"></a>

You can use a bar chart in **Insights** to look at your data in 2 distinct ways, depending on the number of dimensions in the chart. When your chart includes a single dimension, the data series come from your metrics. You can show up to 6 metrics in a single dimensional bar chart.

When a bar charts includes 2 dimensions, the data series come from the second dimension. Two dimensional charts can show any number of data series but only 1 metric.

Either kind of chart can be displayed as a grouped graph, which makes it easy to compare values within a series, or as a stacked graph, which is better at showing the cumulative effect of the series values.

#### Bar chart example

The bar charts below show 2 different views of specific device. The base dimension for both charts is _Product ID_. The left hand chart uses stacked bars to show several metrics (_Quantity sold_, _Quantity return_) for Product ID. The right hand chart uses a second dimension, _Size_, to breakdown each product according to size. Instead of stacked bars, this chart use grouped bars: each bar is a data series corresponding to one of the product ID. Two dimensional charts can only plot a single metric (_Quantity sold_ again in this example).

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F13P8l3kHXpB6Md6CLuQh%2Fuploads%2FFvBuMizR8g2ZTFGAHcZ6%2Fimage.png?alt=media&#x26;token=9cd94d20-40f4-4c55-9518-61bb6a3f16b3" alt=""><figcaption></figcaption></figure>

#### Drill down <a href="#drill-down" id="drill-down"></a>

This option appears on charts that support drill down.

Drilling down gives viewers a way to reveal additional levels of detail within a chart. When you turn on **Drill down,** each dimension you add becomes another level of detail you can drill into. [Learn more about chart drill down](broken-reference).

#### Breakdown dimension <a href="#breakdown-dimension" id="breakdown-dimension"></a>

The Breakdown Dimension displays the metric data broken down according to the selected dimension. For example, a chart showing annual sales data could be broken down by a Sales Region dimension to show sales by region, or by an Employee ID dimension to show sales by sales associate.

#### Date range dimension <a href="#date-range-dimension" id="date-range-dimension"></a>

This option appears if your data source has a valid date dimension.

The Date Range Dimension is used as the basis for limiting the date range of the chart. For example, this is the dimension used if you set a date range property for the chart, or if a viewer of the report uses a date range control to limit the time frame.

#### Metric

Metrics measure the things contained in dimensions and provide the numeric scale and data series for the chart.

Add metrics to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add metric** in the _Data_ tab.

At least 1 metric is required. For charts with a single dimension, you can have up to 20 metrics. For charts with 2 dimensions, you can have 1 metric.

#### Set the default sort <a href="#default-sort" id="default-sort"></a>

The **Sort** and **Secondary sort** options in the chart's _DATA_ properties panel control the default sorting behavior. You can select any metric in the chart's data source, or any dimension currently displayed in the chart, to use as the primary or secondary sorting field.

_The **Secondary sort** option only appears when there is an appropriate combination of dimensions and metrics in the chart._

#### Default date range <a href="#default-date-range" id="default-date-range"></a>

The default date range property lets you set a timeframe for an individual char&#x74;_._

**Default date range options**

| Auto              | Use the default date range determined by the chart's data source.             |
| ----------------- | ----------------------------------------------------------------------------- |
| Custom            | Lets you use the calendar widget to select a custom date range for the chart. |
| Date compare type | Displays comparison data for the selected time period.                        |

#### Filter <a href="#filter" id="filter"></a>

The filter property restricts the data displayed in the component by including or excluding the values you specif&#x79;_._ [Learn more about the filter property.](broken-reference)

**Filter options**

| Filter name   | Click an existing filter to edit it. Mouse over the filter name and click **X** to delete it. |
| ------------- | --------------------------------------------------------------------------------------------- |
| +Add a filter | Creates a new filter for the chart.                                                           |

#### Interactions <a href="#interactions" id="interactions"></a>

When interactions are enabled on a chart, that charts acts like a filter controls. You can filter the report by clicking or "brushing" your mouse across the chart. [Learn more about chart interaction filters](broken-reference).

### Style properties <a href="#style-properties" id="style-properties"></a>

A chart's style properties control the overall presentation and appearance of the chart.

#### Bar Chart

This section controls the overall appearance and layout of your chart.

| Vertical         | Displays the data series as vertical bars.                                                                                                                                                                                                          |
| ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Horizontal       | Displays the data series as horizontal bars.                                                                                                                                                                                                        |
| Bars             | Determines the number of data series shown in the chart. If the number of series selected is less than the number of series in your data, only the top N series will be shown (where N equals the number of series you've selected).                |
| Series           | Determines the number of secondary dimension series shown in the chart. If the number of series selected is less than the number of series in your data, only the top N series will be shown (where N equals the number of series you've selected). |
| Stacked Bars     | When checked, the chart displays stacked bars. Otherwise, the chart displays grouped bars.                                                                                                                                                          |
| 100% Stacking    | When checked, stacked charts show the contribution of each data series to 100% of the total value.                                                                                                                                                  |
| Show Data Labels | When checked, displays the value for each series in chart.                                                                                                                                                                                          |
| Compact Numbers  | Turn on **Show data labels** to see this option: Rounds numbers and displays the unit indicator. E.g., 553,939 becomes 553.9K.                                                                                                                      |

#### Color by <a href="#color-by" id="color-by"></a>

This section controls how your data is colored. Learn more about [coloring your data](broken-reference).&#x20;

These options appear when you have a secondary (breakdown) dimension in your chart.

| Single Color     | <p>When checked, the data series are displayed in shades of a single color. Otherwise, the chart displays in a veritable rainbow of happy colors (depending on your <a href="broken-reference">report theme</a>).</p><p>You can change the series colors using the color pickers below.</p> |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Series order     | <p>Use the current theme to color the data according to its position in the chart. This option emphasizes the ranking of the data over the identity of the data.</p><p>You can set specific colors using each data series' color picker.</p>                                                |
| Dimension values | Colors each dimension value in the chart with the color specified in the dimension value color map. This option ensures that your data uses color consistently, regardless of the position of that data in the chart.                                                                       |

#### Axes <a href="#axes" id="axes"></a>

These options control the display of the chart axes titles and scales. A right Y-axis section appears when you have more than 1 metric in your chart.

**Axis options**

| Show axes                | Shows or hides the chart axes.                                  |
| ------------------------ | --------------------------------------------------------------- |
| Reverse Y-Axis direction | Controls the vertical display of the Y-axis.                    |
| Reverse X-Axis direction | Controls the horizontal display of the X-axis.                  |
| Show axis title          | Shows or hides the axis labels.                                 |
| Axis min and max         | Set minimum and maximum values for the Y-axes.                  |
| Custom tick interval     | Controls the interval between axis ticks.                       |
| Custom distance          | Control the distance between the label of the axis and the axis |

#### Grid <a href="#grid" id="grid"></a>

These options control the look of the chart grid.

| Axis color         | Sets the color of the x-axis line.        |
| ------------------ | ----------------------------------------- |
| Grid color         | Sets the color of the grid lines.         |
| Chart background   | Sets the color of the chart background.   |
| Chart border color | Sets the color of the inner chart border. |

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

#### Legend <a href="#legend" id="legend"></a>

These options determine the placement of the chart legend.

| None      | No legend appears                                                                                                                                                 |
| --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Right     | Legend appears on the right.                                                                                                                                      |
| Bottom    | Legend appears on the bottom.                                                                                                                                     |
| Top       | Legend appears on the top.                                                                                                                                        |
| Alignment | Sets the alignment of the legend relative to the selected position.                                                                                               |
| Max lines | Sets the number of lines used by the legend. If the number of series requires more lines, overflow items can be displayed by clicking the **<** and **>** arrows. |

#### Chart Header <a href="#chart-header" id="chart-header"></a>

The chart header lets viewers perform various actions on the chart, such as exporting the data, drilling up or down, and viewing the chart in the Explorer tool. Chart header options are:

| Show on hover (default) | Three vertical dots appear when you mouse over the chart header. Click these to access the header options.           |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Always show             | The header options always appear.                                                                                    |
| Do not show             | The header options never appear. Note that report viewers can always access the options by right clicking the chart. |
| Color                   | Set the color of the chart header options.                                                                           |



### **Related resources** <a href="#related-resources" id="related-resources"></a>

* [Filter property](broken-reference)

