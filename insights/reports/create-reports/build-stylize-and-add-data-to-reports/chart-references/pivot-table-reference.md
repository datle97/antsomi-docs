# Pivot table reference

Pivot tables let you narrow down a large data set or analyze relationships between data points. Pivot tables reorganize your dimensions and metrics to help you quickly summarize your data and see relationships that might otherwise be hard to spot.

### **Pivot tables in Insights** <a href="#about-chart" id="about-chart"></a>

Pivot tables in Insights take the rows in a standard table and pivot them so they become columns. This lets you group and summarize the data in ways a standard table can't provide.

**Example:**

The following is a standard table listing the Sale quantity are aggregated by Last modified, Product ID, Material and Size:

<figure><img src="../../../../../.gitbook/assets/image (1222).png" alt=""><figcaption></figcaption></figure>

A pivot table, however, quickly shows the relationship of this data:

<figure><img src="../../../../../.gitbook/assets/image (627).png" alt=""><figcaption></figcaption></figure>

#### Show totals

Pivot tables support totals and subtotals for both rows and columns:

<figure><img src="../../../../../.gitbook/assets/image (1621).png" alt=""><figcaption></figcaption></figure>

#### Expand-collapse <a href="#expand-collapse" id="expand-collapse"></a>

Expand-collapse lets report viewers show or hide different levels of information in the pivot table by clicking + and **–** in the column header. Viewers can then explore the data at the level of detail that interests them most. Expand-collapse also provides a way for a single pivot table to show both summary and detailed information, reducing the number of charts needed in your reports.

<figure><img src="../../../../../.gitbook/assets/image (1122).png" alt=""><figcaption></figcaption></figure>

* To change the chart's data source, click the current data source name.
* To view or edit the data source, click <img src="broken-reference" alt="" data-size="line">. (You must have at least view permission to see this icon.)
* Click **+BLEND DATA** to see data from multiple data sources in the same chart.[ Learn more about data blending](broken-reference).

#### Dimension  <a href="#dimensions-metrics" id="dimensions-metrics"></a>

Dimensions are data categories. Dimension values (the data contained by the dimension) are names, descriptions or other characteristics of a category.

Add dimensions to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add dimension** in the _Data_ tab.

**Row Dimension**

The row dimensions provide the breakdown of rows in the pivot table. Reorder the dimensions listed to change the order of the rows in your table.

**Expand-collapse**

Turn on expand-collapse to treat the row dimensions as an expandable hierarchy. The order in which you list the dimensions within the hierarchy matters. As a rule of thumb, you should define hierarchies to always go from the most general to the most specific. For example, defining a geographic hierarchy as Country > City > Region could produce undesirable results, because you're going from a general level to a more detailed level, then back to a more general level.

**Default expand level**

Set the level of detail to show by default. For example, in a geographic hierarchy consisting of Continent > Sub Continent > Country, setting the default expand level to Country would show Continent and Sub Continent details.

**Column Dimension**

The column dimensions provide the columns in the pivot table. Reorder the dimensions listed to change the order of the columns in your table.

#### Date range dimension <a href="#date-range-dimension" id="date-range-dimension"></a>

This option appears if your data source has a valid date dimension. For Google Ads and Analytics data sources, this option is automatically set to the _Date_ dimension.

The Date Range Dimension is used as the basis for limiting the date range of the chart. For example, this is the dimension used if you set a date range property for the chart, or if a viewer of the report uses a date range control to limit the time frame.

#### Metric

Metrics measure the things contained in dimensions and provide the numeric scale and data series for the chart.

Add metrics to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add metric** in the _Data_ tab.

#### Totals

Display totals for each row and column. If you have only 1 dimension in a row or column, the option is to display a grand total. If you have 2 or more dimensions, the options include subtotals and grand totals.

#### Sorting

The sorting options let you control the order of the data displayed in the pivot table. In addition, you can limit the number of rows and columns displayed.

#### Default date range <a href="#default-date-range" id="default-date-range"></a>

The default date range property lets you set a timeframe for an individual char&#x74;_._

**Default date range options**

| Auto   | Use the default date range determined by the chart's data source.             |
| ------ | ----------------------------------------------------------------------------- |
| Custom | Lets you use the calendar widget to select a custom date range for the chart. |

**Filter**

The filter property restricts the data displayed in the component by including or excluding the values you specif&#x79;_._ [Learn more about the filter property.](https://app.gitbook.com/o/-LzunofLVjpTa_-p1PQt/s/13P8l3kHXpB6Md6CLuQh/insights/reports/filter-your-data/about-filters)​**Filter options**

| Filter name   | Click an existing filter to edit it. Mouse over the filter name and click![](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F13P8l3kHXpB6Md6CLuQh%2Fuploads%2FiQND6UrkuoGtMb4STF8V%2Fimage.png?alt=media\&token=6f9f95e5-8105-4af7-abb7-1d83243779dd)to delete it. |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| +Add a filter | Creates a new filter for the chart.                                                                                                                                                                                                                                                     |

#### Interactions <a href="#interactions" id="interactions"></a>

When interactions are enabled on a chart, that charts acts like a filter controls. You can filter the report by clicking or "brushing" your mouse across the chart.[ Learn more about chart interaction filters.](broken-reference)

### Style properties <a href="#style-properties" id="style-properties"></a>

A chart's style properties control the overall presentation and appearance of the chart.

#### Table Header

These options control the appearance of the data labels.

| Header font color  | Changes the font color of the table header.  |
| ------------------ | -------------------------------------------- |
| Header font size   | Changes the font size of the table header.   |
| Header font family | Changes the font family of the table header. |

#### Table Colors <a href="#table-colors" id="table-colors"></a>

These options control the colors of the table borders and cells.

| Header background color | Sets the color of the table header background.   |
| ----------------------- | ------------------------------------------------ |
| Cell border color       | Sets the color of the border between rows.       |
| Highlight color         | Sets the color of the highlight bars.            |
| Odd/Even row color      | Sets the color of odd or even rows in the table. |

#### Table Labels <a href="#table-labels" id="table-labels"></a>

These options control the appearance of the table data.

| Font color            | Sets the font color of the data.                                                                                     |
| --------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Font size             | Sets the font size of the data.                                                                                      |
| Font family           | Sets the font family of the data.                                                                                    |
| Heatmap text contrast | Sets the font color automatically when displaying a heatmap. Choose from 3 levels of contrast, low, medium, or high. |

#### Missing data <a href="#missing-data" id="missing-data"></a>

This option controls how to display missing values. For example, when data is missing from the table, you can choose to show blanks, hyphens, or the words "no data."

#### Metric

This section controls the appearance of the metrics.

| _Drop-down menu_  | <ul><li><strong>Number</strong> - displays the metric value "as is."</li><li><strong>Heatmap</strong> - displays the metric value with a colored background, the intensity of which shows how that value compares to the other values in that column. Use the <strong>Heatmap text contrast</strong> option (in the Table Labels section above) to set the font color automatically to provide better readability of your data labels. Choose from 3 levels of contrast: Low, Medium, or High.</li><li><strong>Bar</strong> - displays the metric value as a horizontal bar. You can change the bar color and include the numeric value, as well, if desired.</li></ul> |
| ----------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Compact Numbers   | Rounds numbers and displays the unit indicator. E.g., 553,939 becomes 553.9K.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| Decimal Precision | Sets the number of decimal places in metric values.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Show target       | Appears when the column type is set to Bar. Shows a target line for the value set in the **target value** field, similar to a bullet chart.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| Show axis         | Displays an X-axis for the bar chart.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |

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

The chart header lets viewers perform various actions on the chart such as exporting the data or viewing the chart in the Explorer tool. Chart header options are:

| Show on hover (default) | Three vertical dots appear when you mouse over the chart header. Click these to access the header options.           |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Always show             | The header options always appear.                                                                                    |
| Do not show             | The header options never appear. Note that report viewers can always access the options by right clicking the chart. |
| Color                   | Set the color of the chart header options.                                                                           |

### Limits of pivot tables <a href="#limits-of-pivot-tables" id="limits-of-pivot-tables"></a>

* Pivot tables can process up to 50,000 rows of data, however, depending on the data set and dimensions and metrics involved in the table, performance may degrade. You can apply a filter to the pivot table to reduce the amount of data being processed.
* You may have up to 3 pivot tables per page in a report.
* Pivot tables can have up to 2 column dimensions.
* Pivot tables can have up to 10 metrics.
* Pivot tables do not paginate, as do standard tables.
* You can't apply metric filters to pivot tables; doing so displays an error message.

### Related resources <a href="#related-resources" id="related-resources"></a>

* [Table reference](broken-reference)
* [Filter property](broken-reference)
