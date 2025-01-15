---
description: Turn your charts into interactive filters.
---

# Add chart interaction filters

Chart interaction filters turn your charts into filter controls. When interactions are enabled on a chart, you can filter the report by interacting with that chart in two ways:

* Clicking one or more dimension values in the chart.
* Dragging, or "brushing," your mouse across a time series, line chart, or area chart.

You can also [let viewers drill down into your data](broken-reference).

### How chart interaction filters work

Chart interaction filters work in the same way as filter controls. For example, a pie chart based on the _Country_ dimension lets you filter your report in the same way as a filter control based on the _Country_ dimension. Brushing a time series acts in the same way as a date range control.

Chart interaction filters can be restricted to groups, just like filter controls.

#### Try it out!

This embedded report has interactions enabled for the charts.

* To filter the charts, click a _Medium_ in the table or a _Country_ in the pie chart.
* To use the time series as a date range filter, click and drag your mouse across part of the chart.
* To to select multiple values, use Ctrl + click (Command + click on Mac).
* To reset a filter, click on some whitespace in the chart, or right-click then select **Reset Action**.

### To enable chart interactions

1. Edit your report.
2. Select a chart.
3. On the right, scroll to the bottom of the DATA properties panel.
4. In the **Interactions** section, select **Apply filter**.
5. Repeat these steps for each chart you want to use as a filter.

### To reset chart filters

You can reset a chart filter to the default in several ways:

* Deselect the selected dimensions by clicking them.
* Click somewhere on the border of chart you are filtering by.

### Limits of chart interactions

* Chart interaction filters aren't available in scorecards or bullet charts.
* You can't filter by the "Others" category.
* Chart interaction filters are subject to the same limits as filter controls in terms of [filtering across data sources.](broken-reference)
