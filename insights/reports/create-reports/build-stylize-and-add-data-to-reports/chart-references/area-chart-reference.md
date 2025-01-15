---
description: How to use and configure area charts.
---

# Area chart reference

An area chart is a variation on the line or time series chart. It uses shaded areas under the plotted lines on the graph to indicate the volume of data represented by the lines. Like a time series, area charts are useful for seeing how your data trends over time.

### Area charts in Insights <a href="#about-chart" id="about-chart"></a>

Area charts let you visualize a single dimension (the _breakdown dimension_) and a single metric, plotted over time.

#### Area chart example <a href="#time-series-example" id="time-series-example"></a>

The example below shows 2 area charts. Both charts show sales data from a fictional pet store. The chart on the left shows sales of items by category (contained in a _Device type_ dimension). This dimension has 3 values: Personal computer, Smart phone và Other.

The metric In both charts is Viewable (called _Viewable_ in the data source).

These examples show 2 different styles of area chart. The left one is stacked: the series values appear in layers, building one atop the other. The right is unstacked: each series starts at the same baseline.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfxSwlRm5f2s5f7Vbr2Oory3GJV_MK_rH297HRpzBJjzDeNamTW66_LcA9Db-Ece7zYOPURc-G6rJzQP9DS2gsi-Nh6RHN3hHWn57KGa-wTEq4vUbOAj8TqEm0R_7OfA0VuCTXd3UN3SoSA1BIhqGRDBSt_?key=c3wH37wA9h3h9ApPDZt-ng" alt=""><figcaption></figcaption></figure>

#### Time dimension <a href="#time-dimension" id="time-dimension"></a>

A time dimension provides a time-based X-axis for your chart. The data type of this dimension determines the granularity of the time series. For example, to visualize daily data, use the Date data type with full year, month, and day. To group the data by calendar quarter, change the data type to Year Quarter.

#### Drill down <a href="#drill-down" id="drill-down"></a>

This option appears on charts that support drill down.

Drilling down gives viewers a way to reveal additional levels of detail within a chart. When you turn on **Drill down,** each dimension you add becomes another level of detail you can drill into. [Learn more about chart drill down](broken-reference).

#### Breakdown dimension <a href="#breakdown-dimension" id="breakdown-dimension"></a>

The Breakdown Dimension displays the metric data broken down according to the selected dimension. For example, a chart showing annual sales data could be broken down by a Sales Region dimension to show sales by region, or by an Employee ID dimension to show sales by sales associate.

#### Metric

Metrics measure the things contained in dimensions and provide the numeric scale and data series for the chart.

Add metrics to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add metric** in the _Data_ tab.

You can display a single metric in an area chart.

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

Learn more about working with dates and time.&#x20;

#### Filter <a href="#filter" id="filter"></a>

The filter property restricts the data displayed in the component by including or excluding the values you specif&#x79;_._

**Filter options**

| Filter name   | Click an existing filter to edit it. Mouse over the filter name and click ![](<../../../../../.gitbook/assets/image (2556).png>) to delete it. |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| +Add a filter | Creates a new filter for the chart.                                                                                                            |

#### Interactions <a href="#interactions" id="interactions"></a>

When interactions are enabled on a chart, that charts acts like a filter controls. You can filter the report by clicking or "brushing" your mouse across the chart. [Learn more about chart interaction filters](broken-reference).

### Style properties <a href="#style-properties" id="style-properties"></a>

A chart's style properties control the overall presentation and appearance of the chart.

#### Area Chart

This section controls the overall appearance and layout of your chart.

| Show Stack        | Stacks the data series.                                                                                                                                                                                                                                                                                      |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 100% Stacking     | When checked, stacked charts show the contribution of each data series to 100% of the total value.                                                                                                                                                                                                           |
| Show Cumulative   | When checked, data series are summed over time. Otherwise, the data is shown with no additional aggregation.                                                                                                                                                                                                 |
| Show points       | Displays individual data points. Viewers can mouse over a data point to display its value.                                                                                                                                                                                                                   |
| Show data labels  | Displays individual values for the data points in the series.                                                                                                                                                                                                                                                |
| Compact Numbers   | <p>Turn on <strong>Show data labels</strong> to see this option:<br>Rounds numbers and displays the unit indicator. E.g., 553,939 becomes 553.9K.</p>                                                                                                                                                        |
| Decimal Precision | <p>Turn on <strong>Show data labels</strong> to see this option:<br>Sets the number of decimal places in metric values.</p>                                                                                                                                                                                  |
| Number of series  | Determines the number of secondary dimension series shown in the chart. If the number of series selected is less than the number of series in your data, only the top N series will be shown (where N equals the number of series you've selected). Remaining series will be grouped in an "other" category. |

#### Color by <a href="#color-by" id="color-by"></a>

This section controls how your data is colored. Learn more about [coloring your data](broken-reference).&#x20;

These options appear when you have a secondary (breakdown) dimension in your chart.

| Single Color     | <p>When checked, the data series are displayed in shades of a single color. Otherwise, the chart displays in a veritable rainbow of happy colors (depending on your <a href="broken-reference">report theme</a>).</p><p>You can change the series colors using the color pickers below.</p> |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Series order     | <p>Use the current theme to color the data according to its position in the chart. This option emphasizes the ranking of the data over the identity of the data.</p><p>You can set specific colors using each data series' color picker.</p>                                                |
| Dimension values | Colors each dimension value in the chart with the color specified in the dimension value color map. This option ensures that your data uses color consistently, regardless of the position of that data in the chart.                                                                       |

#### Missing data <a href="#missing-data" id="missing-data"></a>

This option appears when your time dimension is missing data. **Insights** offers 3 ways of dealing with this situation.

Note: this option has no effect on bar series. The Line to Zero option will affect a trendline, however.

| Line to Zero         | When you select this option, a line series will drop to zero for the missing dates. This is the default option.                      |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| Line Breaks          | When this option is selected, missing data appears as breaks in the data series.                                                     |
| Linear Interpolation | When this option is selected, Data Studio will continue the series by connecting the data points on either side of the missing data. |

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

| None      | No legend appears                                                                                                                         |
| --------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| Right     | Legend appears on the right.                                                                                                              |
| Bottom    | Legend appears on the bottom.                                                                                                             |
| Top       | Legend appears on the top.                                                                                                                |
| Alignment | Sets the alignment of the legend relative to the selected position.                                                                       |
| Max lines | Sets the number of lines used by the legend. If the number of series requires more lines, overflow items can be displayed by scroll down. |

#### Chart Header <a href="#chart-header" id="chart-header"></a>

The chart header lets viewers perform various actions on the chart, such as exporting the data, drilling up or down, and viewing the chart in the Explorer tool. Chart header options are:

| Show on hover (default) | Three vertical dots appear when you mouse over the chart header. Click these to access the header options.           |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Always show             | The header options always appear.                                                                                    |
| Do not show             | The header options never appear. Note that report viewers can always access the options by right clicking the chart. |
| Color                   | Set the color of the chart header options.                                                                           |



### Related resources <a href="#related-resources" id="related-resources"></a>

* [Filter property](broken-reference)
