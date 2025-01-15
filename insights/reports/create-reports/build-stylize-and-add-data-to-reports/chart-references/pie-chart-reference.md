---
description: How to configure pie charts.
---

# Pie chart reference

Pie charts display your data in a circular visualization, with sections (slices of the pie) representing your data series. The sizes of the slices are proportional to the quantity or relative value of the metric you are plotting. In general, pie charts are most useful when comparing a few data points with relatively large differences in proportion between the values. Pie charts that display large numbers of series with minor variations in the data can be confusing to viewers of the chart.

### Pie charts in Insights <a href="#about-chart" id="about-chart"></a>

Pie charts in Insights visualize the relative values for a single dimension/metric combination. The dimension determines the number and names of the slices, while the metric determines the proportion of each slice. Pie charts in Insights support as few as 1 to as many as 10 slices. Insights automatically aggregates any superfluous data points into an "others" slice. The pie can be solid, or it can be donut (ring) shaped.

**Example:**

Following are 2 pie charts, visualizing the same data: the percentage of the _Sales Quantity_ metric by _Material_ dimension. Each colored pie slice represents a material, identified in the legend at the right of the chart. The slice colors are assigned according to the metric value: highest is blue, 2nd highest is red, and so on. (You can change these colors in the _STYLE_ properties tab.) The percentage of sale quantity for each material appears as text labels on the larger slices. (You can see the percentages for the smaller slices by mousing over them.)

The chart on the left is configured to show 10 slices. The chart on the right shows just 2 slices, and is also using the donut style option. In the left hand chart, Insight uses the 5th slice to aggregate any remaining material into the "others" category. The right-hand chart compares the largest sale quantity material ("jean" in this case) to all the other material combined.

<figure><img src="../../../../../.gitbook/assets/image (419).png" alt=""><figcaption></figcaption></figure>

### Configure the chart <a href="#configure" id="configure"></a>

Select the chart, then on the right, use the properties panel to configure the chart options.

### Data properties <a href="#data-properties" id="data-properties"></a>

The options in a chart's data properties panel affect how the data is organized and displayed.

#### Data source <a href="#data-source" id="data-source"></a>

A data source provides the connection between the component and the underlying data set. Data source options are:

* To change the chart's data source, click the current data source name.
* To view or edit the data source, click <img src="../../../../../.gitbook/assets/image (1194).png" alt="" data-size="line">. (You must have at least view permission to see this icon.)
* Click **+BLEND DATA** to see data from multiple data sources in the same chart.[ Learn more about data blending.](broken-reference)

#### Dimension  <a href="#dimensions-metrics" id="dimensions-metrics"></a>

Dimensions are data categories. Dimension values (the data contained by the dimension) are names, descriptions or other characteristics of a category.

Add dimensions to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add dimension** in the _Data_ tab.

Pie charts can have 1 dimension.

#### Date range dimension <a href="#date-range-dimension" id="date-range-dimension"></a>

This option appears if your data source has a valid date dimension. For Google Ads and Analytics data sources, this option is automatically set to the _Date_ dimension.

The Date Range Dimension is used as the basis for limiting the date range of the chart. For example, this is the dimension used if you set a date range property for the chart, or if a viewer of the report uses a date range control to limit the time frame.

#### Metric

Metrics measure the things contained in dimensions and provide the numeric scale and data series for the chart.

Add metrics to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add metric** in the _Data_ tab.

Pie charts can have 1 metric.

#### Set the default sort <a href="#default-sort" id="default-sort"></a>

The **Sort** and **Secondary sort** options in the chart's _DATA_ properties panel control the default sorting behavior. You can select any metric in the chart's data source, or any dimension currently displayed in the chart, to use as the primary or secondary sorting field.

The **Secondary sort** option only appears when there is an appropriate combination of dimensions and metrics in the chart.

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

| Filter name   | Click an existing filter to edit it. Mouse over the filter name and click <img src="../../../../../.gitbook/assets/image (1332).png" alt="" data-size="line"> to delete it. |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| +Add a filter | Creates a new filter for the chart.                                                                                                                                         |

#### Interactions <a href="#interactions" id="interactions"></a>

When interactions are enabled on a chart, that charts acts like a filter controls. You can filter the report by clicking or "brushing" your mouse across the chart.[ Learn more about chart interaction filters](broken-reference).

### Style properties <a href="#style-properties" id="style-properties"></a>

A chart's style properties control the overall presentation and appearance of the chart.

#### Pie Chart

This section controls the overall appearance and layout of your chart.

| Slices           | Determines the number of slices to display. If your selected dimension contains more values than the number of slices, additional values will be aggregated into an "others" category.                                                                                                                                                                                                                                    |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Single Color     | When checked, the pie slices are displayed in shades of the same color. Otherwise, the chart displays in a veritable rainbow of happy colors (depending on your [report theme](https://app.gitbook.com/o/-LzunofLVjpTa_-p1PQt/s/13P8l3kHXpB6Md6CLuQh/insights/reports/create-reports/build-stylize-and-add-data-to-reports/report-layout-options)).You can change the series colors using the color pickers below.        |
| Slice order      | Use the current theme to color the data according to its position in the chart. This option emphasizes the ranking of the data over the identity of the data.You can set specific colors using each data series' color picker.                                                                                                                                                                                            |
| Dimension values | Colors each dimension value in the chart with the color specified in the dimension value color map. This option ensures that your data uses color consistently, regardless of the position of that data in the chart. Learn more about[ coloring your data](https://app.gitbook.com/o/-LzunofLVjpTa_-p1PQt/s/13P8l3kHXpB6Md6CLuQh/insights/reports/create-reports/build-stylize-and-add-data-to-reports/work-with-color). |
| Donut slider     | Changes a solid pie to a donut. Slide the control to increase or decrease the diameter of the donut hole.                                                                                                                                                                                                                                                                                                                 |

#### Label

These options control the appearance of the data labels.

| Slice font color  | Sets the color of the data labels inside the pie slices.                                                                                                                                                                                                                                                                                         |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Slice font size   | Sets the size of the data labels inside the pie slices.                                                                                                                                                                                                                                                                                          |
| Slice font family | Sets the font family of the data labels inside the pie slices.                                                                                                                                                                                                                                                                                   |
| Slice label       | <p>Determines the style of the slice labels. Options are:</p><ul><li>None - no label appears</li><li>Percentage (default) - displays the percentage value of each slice</li><li>Label - displays the dimension value. (You may need to increase the chart size to accommodate longer values)</li><li>Value - displays the metric value</li></ul> |
| Text contrast     | Sets the font color automatically to provide better readability of your data labels. Choose from 3 levels of contrast, low, medium, or high.                                                                                                                                                                                                     |

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

| Legend font color           | Sets the color of the legend labels.                                                                                                                          |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Legend font size            | Sets the size of the legend labels.                                                                                                                           |
| Legend font family          | Sets the font family of the legend labels.                                                                                                                    |
| _Legend placement options:_ | None - No legend appears                                                                                                                                      |
|                             | Right - Legend appears on the right.                                                                                                                          |
|                             | Bottom - Legend appears on the bottom.                                                                                                                        |
|                             | Top - Legend appears on the top.                                                                                                                              |
|                             | Alignment - Sets the alignment of the legend relative to the selected position.                                                                               |
|                             | Max lines - Set the number of lines to display the legend. If the number of strings requires more lines, additional items can be displayed by scrolling down. |

#### Chart Header <a href="#chart-header" id="chart-header"></a>

The chart header lets viewers perform various actions on the chart, such as exporting the data, drilling up or down. Chart header options are:

| Show on hover (default) | Three vertical dots appear when you mouse over the chart header. Click these to access the header options.           |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Always show             | The header options always appear.                                                                                    |
| Do not show             | The header options never appear. Note that report viewers can always access the options by right clicking the chart. |
| Color                   | Set the color of the chart header options.                                                                           |

### **Related resources** <a href="#pie-chart-data-tab-properties" id="pie-chart-data-tab-properties"></a>

* [Filter property](broken-reference)
