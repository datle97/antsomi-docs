---
description: How to configure time series charts.
---

# Time series reference

A time series chart shows how your data changes over a period of time. For example, you can display the count of website sessions daily over the course of a week, or your company's profit margin quarter by quarter for the last 4 years.

### Time series in Insights <a href="#about-chart" id="about-chart"></a>

A time series chart displays the time dimension as the X-axis (horizontal axis), with the Y-axis (vertical axis) representing the measurement scale. Individual metrics are plotted as a series of data points (also called "markers") between the 2 axes. You can have separate left and right Y-axes in a Insights time series chart, if desired.

You can show up to 16 metrics in your time series chart. Each series can be shown as either a line or bar in the chart.

#### Time series example <a href="#time-series-example" id="time-series-example"></a>

The chart below shows the Sales Quantity metric broken down by the Material dimension. The chart has a date range of "7 days ago".

<figure><img src="../../../../../.gitbook/assets/image (1790).png" alt=""><figcaption></figcaption></figure>

### Data properties <a href="#data-properties" id="data-properties"></a>

The options in a chart's data properties panel affect how the data is organized and displayed.

#### Data source <a href="#data-source" id="data-source"></a>

A data source provides the connection between the component and the underlying data set. Data source options are:

* To change the chart's data source, click the current data source name.
* To view or edit the data source, click <img src="../../../../../.gitbook/assets/image (1377).png" alt="" data-size="line">. (You must have at least view permission to see this icon.)
* Click **+BLEND DATA** to see data from multiple data sources in the same chart. [Learn more about data blending](broken-reference).

#### Dimension  <a href="#dimensions-metrics" id="dimensions-metrics"></a>

Dimensions are data categories. Dimension values (the data contained by the dimension) are names, descriptions or other characteristics of a category.

Add dimensions to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add dimension** in the _Data_ tab.

#### Date range dimension <a href="#date-range-dimension" id="date-range-dimension"></a>

This option appears if your data source has a valid date dimension.

The Date Range Dimension is used as the basis for limiting the date range of the chart. For example, this is the dimension used if you set a date range property for the chart, or if a viewer of the report uses a date range control to limit the time frame.

#### Time dimension <a href="#time-dimension" id="time-dimension"></a>

A time dimension provides a time-based X-axis for your chart. The data type of this dimension determines the granularity of the time series. For example, to visualize daily data, use the Date data type with full year, month, and day. To group the data by calendar quarter, change the data type to Year Quarter.

#### Breakdown dimension <a href="#breakdown-dimension" id="breakdown-dimension"></a>

The Breakdown Dimension displays the metric data broken down according to the selected dimension. For example, a chart showing annual sales data could be broken down by a Sales Region dimension to show sales by region, or by an Employee ID dimension to show sales by sales associate.

#### Metric

Metrics measure the things contained in dimensions and provide the numeric scale and data series for the chart.

Add metrics to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add metric** in the _Data_ tab.

You can display up to 16 metrics in a time series.

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

| Filter name   | Click an existing filter to edit it. Mouse over the filter name and click <img src="../../../../../.gitbook/assets/image (1780).png" alt="" data-size="line"> to delete it. |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| +Add a filter | Creates a new filter for the chart.                                                                                                                                         |

### Style properties <a href="#style-properties" id="style-properties"></a>

A chart's style properties control the overall presentation and appearance of the chart.

#### Color by <a href="#color-by" id="color-by"></a>

This section controls how your data is colored. Learn more about [coloring your data](broken-reference).&#x20;

These options appear when you have a secondary (breakdown) dimension in your chart.

| Single Color     | <p>When checked, the data series are displayed in shades of a single color. Otherwise, the chart displays in a veritable rainbow of happy colors (<a href="broken-reference">depending on your report theme</a>).</p><p>You can change the series colors using the color pickers below.</p> |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Series order     | <p>Use the current theme to color the data according to its position in the chart. This option emphasizes the ranking of the data over the identity of the data.</p><p>You can set specific colors using each data series' color picker.</p>                                                |
| Dimension values | Colors each dimension value in the chart with the color specified in the dimension value color map. This option ensures that your data uses color consistently, regardless of the position of that data in the chart.                                                                       |

#### Series <a href="#series" id="series"></a>

This section repeats for each metric displayed in the chart. The order of sections matches the order of the metrics listed in the DATA tab.

| Line or Bars      | Displays the data points for this series as a line or bar.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Line weight       | Determines the thickness of line series.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| Series color      | Sets the color for the series line or bar.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Cumulative        | When checked, data for this series is summed over time. Otherwise, the data is shown with no additional aggregation.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Show points       | Displays individual data points on a line series. Viewers can mouse over a data point to display its value.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Show data labels  | Displays individual values on for the data points in the series.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| Compact Numbers   | Turn on **Show data labels** to see this option: Rounds numbers and displays the unit indicator. E.g., 553,939 becomes 553.9K.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Decimal Precision | <p>Turn on <strong>Show data labels</strong> to see this option:<br>Sets the number of decimal places in metric values.</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Trendline         | <p>A trendline is a line superimposed on a chart revealing the overall direction of the data. Insights supports three types of trendlines: linear, polynomial, and exponential.</p><p>A <strong>linear trendline</strong> is the straight line that most closely approximates the data in the chart. (To be precise, it's the line that minimizes the sum of squared distances from every point to it.)</p><p>If your data is best explained by an exponential of the form <em>eax+b</em>, you can use an <strong>exponential trendline</strong> to show the direction of your data.</p><p>A <strong>polynomial trendline</strong> displays data directionality as a curved line. It can be useful for analyzing large, highly variable data series.</p><p>Options for setting the trendline color and weight appear when you select one of the above options.</p> |

#### Missing data <a href="#missing-data" id="missing-data"></a>

This option appears when your time dimension is missing data. Insights offers 3 ways of dealing with this situation.

Note: this option has no effect on bar series. The Line to Zero option will affect a trendline, however.

| Line to Zero         | When you select this option, a line series will drop to zero for the missing dates. This is the default option.                   |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| Line Breaks          | When this option is selected, missing data appears as breaks in the data series.                                                  |
| Linear Interpolation | When this option is selected, Insights will continue the series by connecting the data points on either side of the missing data. |

#### Legend <a href="#legend" id="legend"></a>

These options determine the placement of the chart legend.

| None      | No legend appears                                                                                                                                 |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| Right     | Legend appears on the right.                                                                                                                      |
| Bottom    | Legend appears on the bottom.                                                                                                                     |
| Top       | Legend appears on the top.                                                                                                                        |
| Alignment | Sets the alignment of the legend relative to the selected position.                                                                               |
| Max lines | Set the number of lines to display the legend. If the number of strings requires more lines, additional items can be displayed by scrolling down. |

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

### Related resources <a href="#related-resources" id="related-resources"></a>

* [Filter property](broken-reference)
