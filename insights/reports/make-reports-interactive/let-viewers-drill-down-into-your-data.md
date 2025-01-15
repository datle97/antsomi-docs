---
description: Turn on drill-down to explore data hierarchies.
---

# Let viewers drill down into your data

Drilling down gives viewers a way to reveal additional levels of detail within a chart.

For example, suppose you want to report on sessions by country, and sessions by city. Rather than include two charts in your report, you can include a single chart with drill-down enabled. When drill-down is enabled on a chart, you can

* **Drill down** from a higher level of detail to a lower one (e.g., from Country to City).
* **Drill up** from a lower level of detail to a higher one (e.g., from City to Country).

Adding drill-down charts to your reports can make them more interactive, reduce the number of separate charts required, and make it easier to find insights at various levels of detail in the data.

### Turn on drill-down for a chart <a href="#enable-drill-down-within-a-chart" id="enable-drill-down-within-a-chart"></a>

1. Edit your report.
2. Select a chart.
3. On the right, in the DATA properties panel under _Dimension_, turn on **Drill down**.
4. Add dimensions to the chart. Each dimension you add becomes another level of detail you can drill into.
5. Select the **Default drill down level**.

_**Legend**_**:**

1. Add dimensions.
2. Turn on drill down. (Note: you need to turn this on before you can add drill-down dimensions.)
3. Set the default drill-down level.

<figure><img src="../../../.gitbook/assets/image (2238).png" alt=""><figcaption></figcaption></figure>

### How drill-down works <a href="#how-drill-down-works" id="how-drill-down-works"></a>

To add drill-down capability to a chart, you'll define a dimension _hierarchy_. The hierarchy defines the levels of detail that chart can display when you drill down or up. Example hierarchies include:

* Date (Year > Month > Day)
* Geography (Country > Region > City)
* Product (Department > Category > SKU)
* Google Analytics events (Event Category > Event Action > Event Label)

The order in which you list the dimensions within the hierarchy matters. As a rule of thumb, you should define hierarchies to always go from the most general to the most specific. For example, defining a geographic hierarchy as Country > City > Region could produce undesirable results, because you're going from a general level to a more detailed level, then back to a more general level.

Drill down into all values

1. View your report
2. Choose a chart in which you've turned on drill-down
3. Click the up and down arrows to see details <img src="../../../.gitbook/assets/image (2569).png" alt="" data-size="line">&#x20;

**Example: drill down to see all cities**

The chart below displays sessions by country. The chart has a drill-down hierarchy defined for the _Country_ and _City_ dimensions. To drill down and see the sessions for all cities, click on up or down arrow to see details.

This displays all the cities, regardless of which country they are in.

<figure><img src="../../../.gitbook/assets/image (940).png" alt=""><figcaption></figcaption></figure>

### Turn off drill-down for a chart <a href="#disable-drill-down-within-a-chart" id="disable-drill-down-within-a-chart"></a>

To turn off drill-down:

1. Edit your report.
2. Select the chart.
3. On the right, in the DATA properties panel, turn off **Drill down**.

### Drill-down and pivot tables <a href="#drill-down-and-pivot-tables" id="drill-down-and-pivot-tables"></a>

You can see additional levels of detail in a pivot table by turning on expand-collapse. You can then show or hide the data from the dimension hierarchy in the pivot table by clicking + and – in the column header. [Learn more about pivot tables](broken-reference).

### Limits of drill-down <a href="#limits-of-drill-down" id="limits-of-drill-down"></a>

* Drill-down doesn't apply to dimensionless charts, such as scorecards and bullet charts.
* Geo charts don’t support all geographic field types within all zoom areas. See the [Geo chart reference](broken-reference) for more details.
