---
description: How to use and configure scatter and bubble charts.
---

# Scatter and bubble chart reference

You can use scatter and bubble charts to look for relationships between variables. These charts show your data as points or circles on a graph using X (left to right) and Y (top to bottom) axes. Scatter charts can include a _trendline_ that shows how the variables in the chart are related.

### Scatter and bubble charts in Insights <a href="#about-chart" id="about-chart"></a>

Scatter charts in Insights let you see the relationship between 2 metrics for up to 3 dimensions. For example, a scatter chart can show if there's a correlation between ad spend and conversion rate for a specific campaign, letting you answer questions such as "Do more expensive ads result in better conversions?"

Use a bubble chart to show data with 3 dimensions. It's similar to a scatter plot where the first 2 dimensions are the horizontal (X) and vertical (Y) coordinates, but it adds a 3rd dimension which is represented in the chart as the size of the bubble.

You can include a trendline that uses one of 3 different calculation types (linear, exponential, or polynomial - see below for an explanation of these types). The general direction of slope of the trendline shows the type of relationship ("correlation") between the variables: a slope upwards from left to right indicates a positive correlation. In other words, the more X, then the more Y. A slope downwards from upper left to lower right can mean a negative correlation: the more X, the less Y. Lack of slope can mean there is little or no correlation between the variables. Data points nearer the trendline are more closely correlated than those farther away from the line.

#### Scatter chart example

The scatter charts below give you 2 different views of the performance for a fictional online university. The left-hand chart compares the average course completion rate with the average activity rate (a measurement of how engaged the students were, in terms of forum posts, class activities completed, etc.) The linear trendline in this chart slopes upwards from left to right, indicating that there is a positive relationship between activity rate and completion rate. I.e., the more engaged the student, the more likely they are to complete the course.

The chart on the right compares the average student grade with the number of hours of homework for each course. The trendline in this chart slopes downwards from left to right, indicating there is a negative correlation between the metrics: the less homework assigned, the better the average grade.

The right hand chart also shows the presence of 2 outliers: the course in the bottom left had few hours of homework but also had a low average grade, while the course at the top of the graph had the highest amount of homework, yet still had close to a 3.0 grade average. (You might want to investigate your own chart outliers to see if you can discover why they don't fit the norm.)

<figure><img src="../../../../../.gitbook/assets/image (1480).png" alt=""><figcaption><p>Scatter chart example</p></figcaption></figure>

_Scatter chart examples showing trendlines and outliers_

### Configure the chart <a href="#configure" id="configure"></a>

Select the chart, then on the right, use the properties panel to configure the chart options.

### Data properties <a href="#data-properties" id="data-properties"></a>

The options in a chart's data properties panel affect how the data is organized and displayed.

#### Data source <a href="#data-source" id="data-source"></a>

A data source provides the connection between the component and the underlying data set. Data source options are:

* To change the chart's data source, click the current data source name.
* To view or edit the data source, click <img src="../../../../../.gitbook/assets/image (2286).png" alt="" data-size="line">. (You must have at least view permission to see this icon.)
* Click **+BLEND DATA** to see data from multiple data sources in the same chart. [Learn more about data blending](broken-reference).

#### Dimension  <a href="#dimensions-metrics" id="dimensions-metrics"></a>

Dimensions are data categories. Dimension values (the data contained by the dimension) are names, descriptions or other characteristics of a category.

Add dimensions to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add dimension** in the _Data_ tab.

#### Date range dimension <a href="#date-range-dimension" id="date-range-dimension"></a>

This option appears if your data source has a valid date dimension. For Google Ads and Analytics data sources, this option is automatically set to the _Date_ dimension.

The Date Range Dimension is used as the basis for limiting the date range of the chart. For example, this is the dimension used if you set a date range property for the chart, or if a viewer of the report uses a date range control to limit the time frame.

#### Drill down <a href="#drill-down" id="drill-down"></a>

This option appears on charts that support drill down.

Drilling down gives viewers a way to reveal additional levels of detail within a chart. When you turn on **Drill down,** each dimension you add becomes another level of detail you can drill into.[ Learn more about chart drill down.](broken-reference)

#### Metric

Metrics measure the things contained in dimensions and provide the numeric scale and data series for the chart.

Add metrics to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add metric** in the _Data_ tab.

**Metric options**

| Metric X    | The X (horizontal) axis metric (e.g. _Avg Grade_ in the right hand example above).                              |
| ----------- | --------------------------------------------------------------------------------------------------------------- |
| Metric Y    | The Y (vertical) axis metric (e.g. _Homework Hours_ in the right hand example above).                           |
| Bubble Size | Setting this causes the chart to display as a bubble chart. This metric determines the size of the data points. |

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

| Filter name    | Click an existing filter to edit it. Mouse over the filter name and click ![](<../../../../../.gitbook/assets/image (730).png>) to delete it. |
| -------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| + Add a filter | Creates a new filter for the chart.                                                                                                           |

#### Interactions <a href="#interactions" id="interactions"></a>

When interactions are enabled on a chart, that charts acts like a filter controls. You can filter the report by clicking or "brushing" your mouse across the chart. [Learn more about chart interaction filters.](broken-reference)

### Style properties <a href="#style-properties" id="style-properties"></a>

A chart's style properties control the overall presentation and appearance of the chart.

#### Scatter chart

This section controls the appearance of the scatter chart data.

| Show data labels  | Displays individual values for the data points in the series.                                                                                                                                     |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Bubble color      | Sets the dimension to use for coloring the data points in your chart. When set to None, the bubbles display in a single color. Selecting a dimension causes the chart to display multiple colors. |
| Number of bubbles | Determines the number of data points to display. If the number of dimension values exceeds this number, only the top N values are shown.                                                          |

#### Color by <a href="#color-by" id="color-by"></a>

This section controls how your data is colored. Learn more about [coloring your data](broken-reference)

| Dimension values | Colors each dimension value in the chart with the color specified in the dimension value color map. This option ensures that your data uses color consistently, regardless of the position of that data in the chart. |
| ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

#### Trendline <a href="#trendline" id="trendline"></a>

A trendline is a line superimposed on a chart revealing the overall direction of the data. Data Studio supports three types of trendlines: linear, polynomial, and exponential.

A **linear trendline** is the straight line that most closely approximates the data in the chart. (To be precise, it's the line that minimizes the sum of squared distances from every point to it.)

If your data is best explained by an exponential of the form _eax+b_, you can use an **exponential trendline** to show the direction of your data.

A **polynomial trendline** displays data directionality as a curved line. It can be useful for analyzing large, highly variable data series.

Options for setting the trendline color and weight appear when you select one of the above options.

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

#### Legend <a href="#legend" id="legend"></a>

These options determine the placement of the chart legend.

| None      | No legend appears                                                                                                                                 |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| Right     | Legend appears on the right.                                                                                                                      |
| Bottom    | Legend appears on the bottom.                                                                                                                     |
| Top       | Legend appears on the top.                                                                                                                        |
| Alignment | Sets the alignment of the legend relative to the selected position.                                                                               |
| Max lines | Set the number of lines to display the legend. If the number of strings requires more lines, additional items can be displayed by scrolling down. |

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

#### Chart Header <a href="#chart-header" id="chart-header"></a>

The chart header lets viewers perform various actions on the chart, such as exporting the data, drilling up or down, and viewing the chart in the Explorer tool. Chart header options are:

| Show on hover (default) | Three vertical dots appear when you mouse over the chart header. Click these to access the header options.           |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Always show             | The header options always appear.                                                                                    |
| Do not show             | The header options never appear. Note that report viewers can always access the options by right clicking the chart. |
| Color                   | Set the color of the chart header options.                                                                           |

### Related resources <a href="#related-resources" id="related-resources"></a>

* [Filter property](broken-reference)
