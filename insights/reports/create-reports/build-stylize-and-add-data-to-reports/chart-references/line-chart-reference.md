---
description: Plot your data using lines and bars.
---

# Line chart reference

Line charts are useful when you want to see how your data changes or fluctuates, either over time, or when measured against a non-time dimension. Line charts can display your data series as either lines, bars, or both.

Line charts can plot a single dimension with up to 16 metrics, or 2 dimensions with 2 metrics.

### Line charts vs. Time series <a href="#about-chart" id="about-chart"></a>

Line charts differ from Time series charts in the following ways:

* You can use any type of dimension as the X-axis in a Line chart. Time series only allow a Date or Date & Time dimension as the X-axis.
* Line charts based on Date or Date & Time dimensions will display gaps in the X-axis if those fields are missing data for the selected date range. By comparison, Time series provide a continuous X-axis of dates, and give you options on how to handle missing data.
* You can limit the number of data points displayed by the Line chart. Time series show all the data for the specified date range.
* Line charts don't display trendlines. Time series do.

#### Line chart example

For example you have sales data of a fictitious store that includes dimensions: Date, Product ID and metrics: Sales Quantity, Quantity Entered. The chart on the left shows the sales volume of each product code in the last 7 days. The chart on the right shows the sale and import volume in the last 7 days (The number of imports is shown in columns)

<figure><img src="../../../../../.gitbook/assets/image (2453).png" alt=""><figcaption><p>Combo chart example</p></figcaption></figure>

### Configure the chart <a href="#configure" id="configure"></a>

Select the chart, then on the right, use the properties panel to configure the chart options.

### Data properties <a href="#data-properties" id="data-properties"></a>

The options in a chart's data properties panel affect how the data is organized and displayed.

#### Data source <a href="#data-source" id="data-source"></a>

A data source provides the connection between the component and the underlying data set. Data source options are:

* To change the chart's data source, click the current data source name.
* To view or edit the data source, click <img src="broken-reference" alt="" data-size="line">. (You must have at least view permission to see this icon.)
* Click **+BLEND DATA** to see data from multiple data sources in the same chart.[ Learn more about data blending.](broken-reference)

#### Dimension  <a href="#dimensions-metrics" id="dimensions-metrics"></a>

Dimensions are data categories. Dimension values (the data contained by the dimension) are names, descriptions or other characteristics of a category.

Add dimensions to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add dimension** in the _Data_ tab.

At least 1 dimension is required. The first dimension you specify serves as the primary data series in the chart. If you specify a breakdown dimension, the chart is limited to 2 metrics.

#### Drill down <a href="#drill-down" id="drill-down"></a>

This option appears on charts that support drill down.

Drilling down gives viewers a way to reveal additional levels of detail within a chart. When you turn on **Drill down,** each dimension you add becomes another level of detail you can drill into. [Learn more about chart drill down](broken-reference).

#### Breakdown dimension <a href="#breakdown-dimension" id="breakdown-dimension"></a>

The Breakdown Dimension displays the metric data broken down according to the selected dimension. For example, a chart showing annual sales data could be broken down by a Sales Region dimension to show sales by region, or by an Employee ID dimension to show sales by sales associate.

#### Date range dimension <a href="#date-range-dimension" id="date-range-dimension"></a>

This option appears if your data source has a valid date dimension. For Google Ads and Analytics data sources, this option is automatically set to the _Date_ dimension.

The Date Range Dimension is used as the basis for limiting the date range of the chart. For example, this is the dimension used if you set a date range property for the chart, or if a viewer of the report uses a date range control to limit the time frame.

#### Metric

Metrics measure the things contained in dimensions and provide the numeric scale and data series for the chart.

Add metrics to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add metric** in the _Data_ tab.

At least 1 metric is required. For charts with a single dimension, you can have up to 16 metrics. For charts with 2 dimensions, you can have 2 metrics.

#### Set the default sort <a href="#default-sort" id="default-sort"></a>

The **Sort** and **Secondary sort** options in the chart's _DATA_ properties panel control the default sorting behavior. You can select any metric in the chart's data source, or any dimension currently displayed in the chart, to use as the primary or secondary sorting field. The **Secondary sort** option only appears when there is an appropriate combination of dimensions and metrics in the chart.

#### Default date range <a href="#default-date-range" id="default-date-range"></a>

The default date range property lets you set a timeframe for an individual char&#x74;_._

**Default date range options**

| Auto              | Use the default date range determined by the chart's data source.             |
| ----------------- | ----------------------------------------------------------------------------- |
| Custom            | Lets you use the calendar widget to select a custom date range for the chart. |
| Date compare type | Displays comparison data for the selected time period.                        |

**Filter**

The filter property restricts the data displayed in the component by including or excluding the values you specif&#x79;_._ [Learn more about the filter property.](https://app.gitbook.com/o/-LzunofLVjpTa_-p1PQt/s/13P8l3kHXpB6Md6CLuQh/insights/reports/filter-your-data/about-filters)

**Filter options**

| Filter name   | Click an existing filter to edit it. Mouse over the filter name and click <img src="broken-reference" alt="" data-size="line"> to delete it. |
| ------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| +Add a filter | Creates a new filter for the chart.                                                                                                          |

#### Interactions <a href="#interactions" id="interactions"></a>

When interactions are enabled on a chart, that charts acts like a filter controls. You can filter the report by clicking or "brushing" your mouse across the chart.[ Learn more about chart interaction filters.](broken-reference)

### Style properties <a href="#style-properties" id="style-properties"></a>

A chart's style properties control the overall presentation and appearance of the chart.

#### Color by <a href="#color-by" id="color-by"></a>

This section controls how your data is colored. Learn more about [coloring your data](broken-reference).&#x20;

These options appear when you have a secondary (breakdown) dimension in your chart.

| Single Color     | When checked, the data series are displayed in shades of a single color. Otherwise, the chart displays in a veritable rainbow of happy colors (depending on your [report theme).](https://app.gitbook.com/o/-LzunofLVjpTa_-p1PQt/s/13P8l3kHXpB6Md6CLuQh/insights/reports/create-reports/build-stylize-and-add-data-to-reports/report-layout-options)​You can change the series colors using the color pickers below. |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Series order     | Use the current theme to color the data according to its position in the chart. This option emphasizes the ranking of the data over the identity of the data.You can set specific colors using each data series' color picker.                                                                                                                                                                                       |
| Dimension values | Colors each dimension value in the chart with the color specified in the dimension value color map. This option ensures that your data uses color consistently, regardless of the position of that data in the chart.                                                                                                                                                                                                |

#### Series

This section repeats for each metric displayed in the chart. The order of sections matches the order of the metrics listed in the DATA tab.

| Line or Bars      | Displays the data points for this series as a line or bar.                                                                     |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| Line weight       | Determines the thickness of line series.                                                                                       |
| Series color      | Sets the color for the series line or bar.                                                                                     |
| Cumulative        | When checked, data for this series is summed over time. Otherwise, the data is shown with no additional aggregation.           |
| Show points       | Displays individual data points on a line series. Viewers can mouse over a data point to display its value.                    |
| Show data labels  | Displays individual values on for the data points in the series.                                                               |
| Compact Numbers   | Turn on **Show data labels** to see this option: Rounds numbers and displays the unit indicator. E.g., 553,939 becomes 553.9K. |
| Decimal Precision | <p>Turn on <strong>Show data labels</strong> to see this option:<br>Sets the number of decimal places in metric values.</p>    |

#### General

| Smooth           | Display series lines as curves.                                                                                                                                                                                                                                                                              |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Stacked bars     | Display bars as stacked bars.                                                                                                                                                                                                                                                                                |
| Number of points | Determines the number of data elements shown in the chart's X-axis. If the number of points selected is less than the number of values in the X-axis dimension, only the top N points will be shown (where N equals the number of points you've selected).                                                   |
| Number of series | Determines the number of secondary dimension series shown in the chart. If the number of series selected is less than the number of series in your data, only the top N series will be shown (where N equals the number of series you've selected). Remaining series will be grouped in an "other" category. |

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

| None      | No legend appears                                                                                                                                 |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| Right     | Legend appears on the right.                                                                                                                      |
| Bottom    | Legend appears on the bottom.                                                                                                                     |
| Top       | Legend appears on the top.                                                                                                                        |
| Alignment | Sets the alignment of the legend relative to the selected position.                                                                               |
| Max lines | Set the number of lines to display the legend. If the number of strings requires more lines, additional items can be displayed by scrolling down. |

#### Chart Header <a href="#chart-header" id="chart-header"></a>

The chart header lets viewers perform various actions on the chart, such as exporting the data, drilling up or down, and viewing the chart in the Explorer tool. Chart header options are:

| Show on hover (default) | Three vertical dots appear when you mouse over the chart header. Click these to access the header options.           |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Always show             | The header options always appear.                                                                                    |
| Do not show             | The header options never appear. Note that report viewers can always access the options by right clicking the chart. |
| Color                   | Set the color of the chart header options.                                                                           |

### Related resources <a href="#related-resources" id="related-resources"></a>

* F[ilter property](broken-reference)
