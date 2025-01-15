---
description: How to use and configure Geo charts.
---

# Geo chart reference

A Geo chart provides an easy way to visualize how a measurement varies across a geographic area.

### Geo charts in Insights <a href="#about-chart" id="about-chart"></a>

An **Insights** Geo chart requires you to provide 3 pieces of information:

* a geographic dimension, such as _Country_, _City_, _Region_, etc.
* a metric, such as _Sessions_, _Units Sold_, _Population_, etc.
* the map's zoom area.

#### Zoom area <a href="#zoom-area" id="zoom-area"></a>

The zoom area determines how much of the world the map displays. It also can restrict the data shown by the Geo chart. For example, selecting the _City_ dimension and setting the zoom area to Germany (DE), limits the Geo chart to showing cities in Germany. The map itself zooms in to focus on Germany.

_If there is not a 1:1 mapping between the selected geo field type and available zoom areas, you may be able to restrict the data using a filter, as shown in the examples below._

### Geo chart examples <a href="#geo-map-examples" id="geo-map-examples"></a>

#### Example 1: Limit the map display to a specific country (e.g., France). <a href="#example-1-limit-the-map-display-to-a-specific-country-e-g-france" id="example-1-limit-the-map-display-to-a-specific-country-e-g-france"></a>

Step 1: Set the dimension and visible area

* Dimension: _Country_
* Metric: _Number of Sessions per User_
* Zoom Area: Western Europe

Step 2: Filter the country dimension to only include France.

* Dimension: _Country_
* Match Type: **Equals**
* Expression: France

<figure><img src="../../../../../.gitbook/assets/image (519).png" alt=""><figcaption><p>Geo map example: sessions per user for France</p></figcaption></figure>

#### Example 2: Display US state map

Step 1: Set the dimension and visible area

* Dimension: _Region_
* Metric: _Number of Sessions per User_
* Visible Area: US

Step 2: Filter the country dimension to only include the United States

* Dimension: _Country_
* Match Type: **Equals**
* Expression: United States

<figure><img src="../../../../../.gitbook/assets/image (1376).png" alt=""><figcaption><p>Geo map example: sessions per user for US states</p></figcaption></figure>

### Configure the chart <a href="#configure" id="configure"></a>

Select the chart, then on the right, use the properties panel to configure the chart options.

### Data properties <a href="#data-properties" id="data-properties"></a>

The options in a chart's data properties panel affect how the data is organized and displayed.

#### Data source <a href="#data-source" id="data-source"></a>

A data source provides the connection between the component and the underlying data set. Data source options are:

* To change the chart's data source, click the current data source name.
* To view or edit the data source, click <img src="broken-reference" alt="" data-size="line">. (You must have at least view permission to see this icon.)
* Click **+BLEND DATA** to see data from multiple data sources in the same chart. [Learn more about data blending](broken-reference).

#### Dimension  <a href="#dimensions-metrics" id="dimensions-metrics"></a>

Dimensions are data categories. Dimension values (the data contained by the dimension) are names, descriptions or other characteristics of a category.

Add dimensions to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add dimension** in the _Data_ tab.

A single valid geo dimension is required.&#x20;

#### Drill down <a href="#drill-down" id="drill-down"></a>

This option appears on charts that support drill down.

Drilling down gives viewers a way to reveal additional levels of detail within a chart. When you turn on **Drill down,** each dimension you add becomes another level of detail you can drill into. [Learn more about chart drill down](broken-reference).

#### Date range dimension <a href="#date-range-dimension" id="date-range-dimension"></a>

This option appears if your data source has a valid date dimension.

The Date Range Dimension is used as the basis for limiting the date range of the chart. For example, this is the dimension used if you set a date range property for the chart, or if a viewer of the report uses a date range control to limit the time frame. &#x20;

#### Metric

Metrics measure the things contained in dimensions and provide the numeric scale and data series for the chart.

Add metrics to the chart by dragging fields from the _Available Fields_ panel on the right. You can also click **Add metric** in the _Data_ tab.

Any single available metric is required. Your data will be displayed on the map using a color progression to indicate relative value, with higher intensity color gradient representing higher values than lower intensity colors. You can change the color of the map using the STYLE tab.

#### Zoom area <a href="#sort" id="sort"></a>

This limits the map display to the selected area. The choices available depend on the scope of the geo field type used for a given chart. For example, when a City geo field is selected, options for Visible Area are limited to Country and Region. When a Sub Continent Code field is selected, options for Visible Area are limited to World and Continent.

| World        | <p>Displays the entire world map.Available with the following geo field types:</p><ul><li>Continent</li><li>Continent Code</li><li>Sub Continent</li><li>Sub Continent Code</li><li>Country</li><li>Country Code</li><li>Latitude, Longitude</li><li>City</li><li>City Code</li></ul> |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Continent    | <p>Displays the selected continent.Available with the following geo dimensions:</p><ul><li>Sub Continent</li><li>Sub Continent Code</li><li>Country</li><li>Country Code</li><li>Latitude, Longitude</li><li>City</li><li>City Code</li></ul>                                         |
| Subcontinent | <p>Displays the selected subcontinent.Available with the following geo dimensions:</p><ul><li>Country</li><li>Country Code</li><li>Latitude, Longitude</li><li>City</li><li>City Code</li></ul>                                                                                       |
| Country      | <p>Displays the selected country.Available with the following geo dimensions:</p><ul><li>City</li><li>City Code</li><li>Metro</li><li>Metro Code</li><li>Region</li><li>Region Code</li><li>Latitude, Longitude</li></ul>                                                             |
| Region       | <p>Displays the selected region.Available with the following geo dimensions:</p><ul><li>City</li><li>Metro Code (US only)</li></ul>                                                                                                                                                   |

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

| Filter name   | Click an existing filter to edit it. Mouse over the filter name and click <img src="broken-reference" alt="" data-size="line"> to delete it. |
| ------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| +Add a filter | Creates a new filter for the chart.                                                                                                          |

#### Interactions <a href="#interactions" id="interactions"></a>

When interactions are enabled on a chart, that charts acts like a filter controls. You can filter the report by clicking or "brushing" your mouse across the chart. [Learn more about chart interaction filters](broken-reference).

### Style properties <a href="#style-properties" id="style-properties"></a>

A chart's style properties control the overall presentation and appearance of the chart.

#### Geo chart

These properties control the appearance of the chart elements.

| Max color value | Sets the color for the highest value in the data range. Typically, this should be the darkest shade in the chart. |
| --------------- | ----------------------------------------------------------------------------------------------------------------- |
| Mid color value | Sets the color for the median value in the data range. Typically, this should be a medium shade.                  |
| Min color value | Sets the color for the lowest value in the data range. Typically, this should be the lightest shade in the chart. |
| Show Legend     | Shows or hides the metric legend.                                                                                 |

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

The chart header lets viewers perform various actions on the chart, such as exporting the data, drilling up or down. Chart header options are:

| Show on hover (default) | Three vertical dots appear when you mouse over the chart header. Click these to access the header options.           |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Always show             | The header options always appear.                                                                                    |
| Do not show             | The header options never appear. Note that report viewers can always access the options by right clicking the chart. |
| Color                   | Set the color of the chart header options.                                                                           |

### Geo chart limits <a href="#geo-map-data-tab-properties" id="geo-map-data-tab-properties"></a>

Geo charts include the first **5000** rows of data, unless otherwise mentioned for a field type. Chart data is sorted in descending order based on the selected metric.

### Geo functions <a href="#geo-functions" id="geo-functions"></a>

Insights provide a number of geo functions that can be used to work with and transform geographic information in your data sources.

### Related resources <a href="#related-resources" id="related-resources"></a>

* [Filter property](broken-reference)
