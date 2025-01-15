---
description: How to use and configure tree map charts.
---

# Tree map reference

A treemap shows your data organized into dimension hierarchies. For example, you can use a treemap to show the average annual sales of each item in a product category > subcategory > product hierarchy.

### Treemaps in Insights <a href="#about-chart" id="about-chart"></a>

Data in a treemap is displayed in "branches" (also called "nodes"). Each branch can have zero or more sub-branches, and one parent branch (except for the root, which has no parents). Each branch is displayed as a rectangle, sized and colored according to the values in your data. Sizes and colors are valued relative to all other branches in the graph.

Treemaps are a good hypothesis-generation tool because they can help expose the relative importance of, and the relationship between, different entities.

### Treemap examples <a href="#treemap-examples" id="treemap-examples"></a>

The treemap below shows the sales of a fictional store. The label of the branch comes from 2 dimensions Material and Size.

<figure><img src="../../../../../.gitbook/assets/image (1035).png" alt=""><figcaption></figcaption></figure>

Here's how the underlying data for this chart is organized:

<figure><img src="../../../../../.gitbook/assets/image (1200).png" alt=""><figcaption></figcaption></figure>

### Configure the chart <a href="#configure" id="configure"></a>

Select the chart, then on the right, use the properties panel to configure the chart options.

### Data properties <a href="#data-properties" id="data-properties"></a>

The options in a chart's data properties panel affect how the data is organized and displayed.

#### Data source <a href="#data-source" id="data-source"></a>

A data source provides the connection between the component and the underlying data set. Data source options are:

* To change the chart's data source, click the current data source name.
* To view or edit the data source, click <img src="../../../../../.gitbook/assets/image (917).png" alt="" data-size="line">. (You must have at least view permission to see this icon.)
* Click **+BLEND DATA** to see data from multiple data sources in the same chart. [Learn more about data blending](https://support.google.com/datastudio/answer/9061420).

#### Levels to show <a href="#levels-to-show" id="levels-to-show"></a>

The **Levels to show** option determines the granularity of the chart. For example, the sample chart above has Levels to show set to 2, causing it to show two levels of detail (Material and Size).

<figure><img src="../../../../../.gitbook/assets/image (916).png" alt=""><figcaption></figcaption></figure>

Setting **Levels to show** to 1 causes the chart to display only one level of detail (Material):

<figure><img src="../../../../../.gitbook/assets/image (2212).png" alt=""><figcaption></figcaption></figure>

#### Drill down <a href="#drill-down" id="drill-down"></a>

This option appears on charts that support drill down.

Drilling down gives viewers a way to reveal additional levels of detail within a chart. When you turn on **Drill down,** each dimension you add becomes another level of detail you can drill into. [Learn more about chart drill down](broken-reference).

**What's the difference between drill down and levels to show?**

**Drill down** lets you focus on a specific level of detail, while **Levels to show** controls how many levels of detail appear in the treemap. For example, here's the result of drilling down into the chart above. Note that it now displays only one level of detail, but that level is now the Material level.

<figure><img src="../../../../../.gitbook/assets/image (1508).png" alt=""><figcaption></figcaption></figure>

#### Total rows <a href="#total-rows" id="total-rows"></a>

Treemaps can display from 5 to 5000 rows of data.

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

| Filter name   | Click an existing filter to edit it. Mouse over the filter name and click <img src="../../../../../.gitbook/assets/image (834).png" alt="" data-size="line"> to delete it. |
| ------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| +Add a filter | Creates a new filter for the chart.                                                                                                                                        |

#### Interactions <a href="#interactions" id="interactions"></a>

When interactions are enabled on a chart, that charts acts like a filter controls. You can filter the report by clicking or "brushing" your mouse across the chart. [Learn more about chart interaction filters.](broken-reference)

### Style properties <a href="#style-properties" id="style-properties"></a>

A chart's style properties control the overall presentation and appearance of the chart.

#### Treemap

| Max color value    | Set the color for the highest metric value.                                                                                            |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------- |
| Mid color value    | Set the color for the median metric value.                                                                                             |
| Min color value    | Set the color for the minimum metric value.                                                                                            |
| Show branch header | Show or hide the parent branches.                                                                                                      |
| Show scale         | Show or hide the chart scale, which appears above the treemap. To see the scale in action, hover over different branches in the chart. |

#### Text <a href="#text" id="text"></a>

Set the font color, font size, and font family for text in the chart.

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
