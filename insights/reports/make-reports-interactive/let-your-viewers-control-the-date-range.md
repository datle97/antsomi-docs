---
description: Add a date range control to a report.
---

# Let your viewers control the date range

The date range control is a customizable calendar widget that enables your viewers to change the time frame of a report.

### Add a date range control to a report <a href="#add_a_date_range_control_to_a_report" id="add_a_date_range_control_to_a_report"></a>

1. Edit the report.
2. Select the **Date Range** tool from the toolbar <img src="../../../.gitbook/assets/image (2042).png" alt="" data-size="line">.&#x20;
3. Draw the date range in a nice spot.
4. In the _Date Range Properties_ panel, **DATA** tab, select the default date range.
5. Use the **STYLE** tab options to change the look of the widget as it appears on the report.

### How date range controls work <a href="#how_date_range_controls_work" id="how_date_range_controls_work"></a>

A date range control enables the report viewer to adjust the date range of the charts in a report. This lets the viewer restrict the data shown in those charts to a specified time frame. Date range controls appear to the user as a calendar widget on the report. Viewers can define a custom date range using the calendar, or using a drop-down of predefined ranges. The predefined options include ranges such as "Yesterday," "Last 7 days (including today)," and "Last quarter."

#### Date range controls and data sources

To add a date range control to a report, at least one of the data sources attached to the report must have a date dimension. Date range controls only affect charts built on data sources that have a date dimension.

#### Date range control scope

By default, a date range control governs all the charts on the page (assuming those charts come from a data source with valid date data). You can limit the scope of the date range control by doing either of the following:

1\) Assigning a date range property to an individual chart overrides the date range control. The chart's date property will stay in effect.

2\) Grouping a date range control with a chart limits the effect of the date range control to that chart. Any non-grouped charts will not be affected by the date range control.

### Make a date range control appear on every page <a href="#make-report-level" id="make-report-level"></a>

By default, every component you place on a report is a page-level object: it only appears on the original page on which you place it. You can make a date range control appear on every page of your multi-page report by making it report-level. To do this:

1. Edit the report.
2. Select the date range control (or other component).
3. Right click, select Make report level

Your date range control will now appear in the same location on every page of your report.
