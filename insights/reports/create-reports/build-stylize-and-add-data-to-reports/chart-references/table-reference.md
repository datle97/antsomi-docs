---
description: How to use and configure tables.
---

# Table reference

Tables display your data in a grid of rows and columns. Each column represents a dimension or metric, while each row is one record of your data.

### Tables in Insight <a href="#about-chart" id="about-chart"></a>

Tables in Insight automatically summarize your data. Each row in the table displays the summary for each unique combination of the dimensions included in the table definition. Each metric in the table is summarized according to the aggregation type for that metric (sum, average, count, etc.). A Insights table can have up to 10 dimensions and 20 metrics.

**Example:**

This is the sales data sheet of a fictional clothing store.

<figure><img src="../../../../../.gitbook/assets/image (1264).png" alt=""><figcaption></figcaption></figure>

The table below shows the quantity sold and the material:

<figure><img src="../../../../../.gitbook/assets/image (2256).png" alt=""><figcaption></figcaption></figure>

_Example table 1_

In Example 1, Insights aggregated sales based on Sale date, Product ID, and Material.

_Example table 2_

In the example 2, the table consists of 8 rows, 1 row for each entry. Quantity sold are aggregated per item.

### Add a table to your report <a href="#add-a-table-to-your-report" id="add-a-table-to-your-report"></a>

To add a table to a report:

1. Edit the report.
2. At the top, click **Add a chart**.
3. Select a default table style.
   1. For example, you can add a standard table, a table where the metrics are displayed as bars, or a table with a heatmap applied.
4. Drag the chart to the desired location on the page and resize it to the desired dimensions.
5. Use the properties panel on the right to add metrics and dimensions and to style the table.

#### Adjust column size <a href="#adjust-column-size" id="adjust-column-size"></a>

To manually change the size of individual columns in the table, click a column divider and drag it. To resize multiple columns at once, hold the Shift key while dragging a column divider.

### Data properties <a href="#data-properties" id="data-properties"></a>

The options in a chart's data properties panel affect how the data is organized and displayed.

#### Data source <a href="#data-source" id="data-source"></a>

A data source provides the connection between the component and the underlying data set. Data source options are:

* To change the chart's data source, click the current data source name.
* To view or edit the data source, click ![](<../../../../../.gitbook/assets/image (2587).png>). (You must have at least view permission to see this icon.)
* Click **+BLEND DATA** to see data from multiple data sources in the same chart. [Learn more about data blending](broken-reference).

#### Dimension  <a href="#dimensions-metrics" id="dimensions-metrics"></a>

Dimensions are data categories. Dimension values (the data contained by the dimension) are names, descriptions or other characteristics of a category.

Add dimensions to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add dimension** in the _Data_ tab.

Tables can have up to 20 metrics.

#### Sort your data <a href="#sort-your-data" id="sort-your-data"></a>

Viewers of your reports can sort the data by clicking on a column header. Each click reverses the sort order: e.g., click once to sort in ascending (lowest to highest) order, click again to sort in descending (highest to lowest) order. In the example above, the table is sorted by _Qty Sold_ in descending order. Viewers can still sort the chart even if the editor has defined a default sort.

If a viewer changes the sort order of a chart, and that chart was sorted by a metric not displayed in the chart, refreshing the page restores the default sorting. When a secondary sort field is selected, the primary and secondary sort fields are numbered in the table 1 and 2, respectively. Sorting by any other field (by clicking the field name in the table header) removes the primary and secondary sorts.

#### Set the default sort <a href="#default-sort" id="default-sort"></a>

The **Sort** and **Secondary sort** options in the chart's _DATA_ properties panel control the default sorting behavior. You can select any metric in the chart's data source, or any dimension currently displayed in the chart, to use as the primary or secondary sorting field.

The **Secondary sort** option only appears when there is an appropriate combination of dimensions and metrics in the chart.

#### Rows per page <a href="#rows-per-page" id="rows-per-page"></a>

Use the **Rows per page** option to control how many table rows to display per table page. **Show pagination** must be enabled for this to take effect.

#### Show summary row <a href="#show-summary-row" id="show-summary-row"></a>

The **Show summary row** option toggles display of a row at the bottom of a table summarizing each metric column.

#### Default date range <a href="#default-date-range" id="default-date-range"></a>

The default date range property lets you set a timeframe for an individual char&#x74;_._

**Default date range options**

| Auto              | Use the default date range determined by the chart's data source.             |
| ----------------- | ----------------------------------------------------------------------------- |
| Custom            | Lets you use the calendar widget to select a custom date range for the chart. |
| Date compare type | Displays comparison data for the selected time period.                        |

#### Filter <a href="#filter" id="filter"></a>

The filter property restricts the data displayed in the component by including or excluding the values you specif&#x79;_._ L[earn more about the filter property.](broken-reference)

**Filter options**

| Filter name   | Click an existing filter to edit it. Mouse over the filter name and click ![](<../../../../../.gitbook/assets/image (1436).png>) to delete it. |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| +Add a filter | Creates a new filter for the chart.                                                                                                            |

#### Interactions <a href="#interactions" id="interactions"></a>

When interactions are enabled on a chart, that charts acts like a filter controls. You can filter the report by clicking or "brushing" your mouse across the chart.[ Learn more about chart interaction filters.](broken-reference)

### Style properties <a href="#style-properties" id="style-properties"></a>

A chart's style properties control the overall presentation and appearance of the chart.

#### Table Header <a href="#table-header" id="table-header"></a>

These options control the appearance of the table header and column labels.

| Show header        | Shows or hides the table header. Note that viewers can't sort tables with hidden headers. |
| ------------------ | ----------------------------------------------------------------------------------------- |
| Wrap text          | Wraps header text.                                                                        |
| Header font color  | Sets the font color of the table header.                                                  |
| Header font size   | Sets the font size of the table header.                                                   |
| Header font family | Sets the font family of the table header.                                                 |

**Table Colors**

These options control the colors of the table borders and cells.

| Header background color | Sets the color of the table header background.   |
| ----------------------- | ------------------------------------------------ |
| Cell border color       | Sets the color of the border between rows.       |
| Odd/Even row color      | Sets the color of odd or even rows in the table. |

#### Table Labels <a href="#table-labels" id="table-labels"></a>

These options control the appearance of the table data.

| Font color            | Sets the font color of the data.                                                                                     |
| --------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Font size             | Sets the font size of the data.                                                                                      |
| Font family           | Sets the font family of the data.                                                                                    |
| Heatmap text contrast | Sets the font color automatically when displaying a heatmap. Choose from 3 levels of contrast, low, medium, or high. |

#### Table Body <a href="#table-body" id="table-body"></a>

These options control the appearance of the table body.

| Row numbers | Adds row numbering as the leftmost column of the table. |
| ----------- | ------------------------------------------------------- |
| Wrap text   | Wraps long text in the table body.                      |

#### Table Footer <a href="#table-footer" id="table-footer"></a>

These options control the appearance of the table footer.

| **Show pagination**  | Pagination lets the viewer navigate through long tables. Show or hide the page controls with this option. |
| -------------------- | --------------------------------------------------------------------------------------------------------- |
| Compact pagination   | Reduces the vertical spacing of the pagination controls.                                                  |
| Footer border color  | Sets the footer border color.                                                                             |
| Footer border weight | Sets the thickness of the footer border.                                                                  |
| Footer border style  | Sets the line style of the footer border.                                                                 |

#### Missing data <a href="#missing-data" id="missing-data"></a>

This option controls how to display missing values. For example, when data is missing from the table, you can choose to show blanks, hyphens, or the words "no data."

#### Dimension and metric appearance <a href="#dimension-and-metric-appearance" id="dimension-and-metric-appearance"></a>

These options control the display of your dimension and metric columns. Each column in your table has a corresponding numbered section in the properties panel: from left to right, the first metric in the table is Column #1, the second metric is Column #2, and so on. You can set the following options for each column:

| Number display    | <ul><li><strong>Number</strong> - displays the metric value "as is."</li><li><strong>Heatmap</strong> - displays the metric value with a colored background, the intensity of which shows how that value compares to the other values in that column.</li></ul><p>Use the <strong>Heatmap text contrast</strong> option (in the Table Labels section above) to set the font color automatically to provide better readability of your data labels. Choose from 3 levels of contrast: Low, Medium, or High.</p><ul><li><strong>Bar</strong> - displays the metric value as a horizontal bar. You can change the bar color and include the numeric value, as well, if desired.</li></ul> |
| ----------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Alignment         | Aligns the data in the column left, right, or center.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Compact Numbers   | Rounds numbers and displays the unit indicator. E.g., 553,939 becomes 553.9K.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Decimal Precision | Sets the number of decimal places in metric values.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Show target       | Appears when the column type is set to Bar. Shows a target line for the value set in the target value field, similar to a bullet chart.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Show axis         | Displays an X-axis for the bar chart.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |

#### Chart Header <a href="#chart-header" id="chart-header"></a>

The chart header lets viewers perform various actions on the chart, such as exporting the data, drilling up or down, and viewing the chart in the Explorer tool. Chart header options are:

| Show on hover (default) | Three vertical dots appear when you mouse over the chart header. Click these to access the header options.           |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Always show             | The header options always appear.                                                                                    |
| Do not show             | The header options never appear. Note that report viewers can always access the options by right clicking the chart. |
| Color                   | Set the color of the chart header options.                                                                           |

### **Related resources** <a href="#related-resources" id="related-resources"></a>

* [Pivot table reference](broken-reference)
* [Filter your data](broken-reference)
