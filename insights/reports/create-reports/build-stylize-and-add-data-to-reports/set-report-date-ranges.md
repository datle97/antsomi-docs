---
description: Configure the timeframe and comparison periods in your reports.
---

# Set report date ranges

To visualize date-based data, you'll configure one or more of the following settings:

* The dimension that governs the timeframe of the report (the _date range dimension_).
* The dimension that determines how date-based data in a chart is handled (the _time dimension_).
* The _default date range_ for components that can display or interact with date-based data.
* How to compare the current period to a previous period, if desired (the _comparison date range_).

## Date range dimension

The date range dimension tells **Insights** which of the available dimensions controls the selected component's timeframe.&#x20;

#### &#x20;Set the date range dimension

You may need to set this manually if **Insights** cannot find a valid date dimension, or if your data source contains a different dimension you want to use.

1. Select a chart or control.
2. Select the _DATA_ tab.
3. In the _Data Source_ section, click the **Date Range Dimension**, then use the dimension picker to select a valid date dimension.

## Default date range

The default date range for your charts and controls depends on their data source. You can change the amount of data shown by setting the **Default Date Range** property. You can set this property for your entire report, specific page, or for one or more charts and controls on a page.&#x20;

#### Set the default date range

To change the default date range for **one or more charts or controls**, select them.

**Next:**

1. In the _Properties_ panel on the right, select the _DATA_ tab.
2. Scroll down to find the _Default Date Range_ property.
3. Select **Custom.**
4. Click the currently selected range to display the date range options.

**Previous period**--compares the currently selected period for the chart to the previous matching period. For example, if the current period is **Last 28 days**, the comparison is to the previous 28 day period prior to the last 28 days.

**Previous year**--compares the current selected period to the same period last year. For example, if the current period is **This week to date (Sun-Sat)**, the chart displays comparison data for the matching dates last year.

_Use the **Include today** check box to include any data collected so far for the current day (if applicable)._

_**Insights** defaults to starting the weekly rolling window on Sunday. You can change this to start on Monday by selecting **This week (Mon-Sun)** or **Last week (Mon-Sun)** in the date options list._

### Advanced date ranges

Advanced date ranges let you configure custom date periods for both the current date range and the comparison date range. For example, you can create date ranges such as "last 90 days from yesterday," or "last 52 weeks from last week" or compare the "current 30 days to the last 30 days, aligned by day of the week."&#x20;

#### **Configure an advanced date range**

_In edit mode:_

* Open the calendar widget in the date range properties for the selected chart, the current page, or the report.

_In view mode:_

* Open the date range control.

1. Then, in the upper right corner of the calendar, click ![Down Arrow](https://storage.googleapis.com/support-kms-prod/76B4941B08D1516AC7336D5A3C2E7914920D).
2. Scroll to the bottom of the list of preset date options.
3. Click **Advanced**.
4. Set the **Start** date:
   * Select **Today** to make the start date a rolling date.
   * Select **Fixed** to make the start date a specific calendar date.
5. Select **Minus** to make the start date a date in the past, or select **Plus** to make the start date a date in the future.
6. Enter the **number** of date units.
7. Specify what **date units** to use.
8. Repeat steps 4 - 7 for the end date.
9. Click **APPLY**.

**Examples**

_Last 90 days from yesterday._

| **Start Date** | **End Date** |
| -------------- | ------------ |
| Today          | Today        |
| Minus          | Minus        |
| 90             | 1            |
| Days           | Days         |

_Last 30 days from today._

| **Start Date** | **End Date** |
| -------------- | ------------ |
| Today          | Today        |
| Minus          | Minus        |
| 29             | 0            |
| Days           | Days         |

_Next 2 quarters from this quarter._

| **Start Date** | **End Date** |
| -------------- | ------------ |
| Today          | Today        |
| Minus          | Plus         |
| 0              | 2            |
| Quarters       | Quarters     |

_You can see other examples by selecting a preset date range, then viewing how it is configured as custom rolling date range. For example, configure your chart to use the "Last week (starts Monday)" preset range. Then open the advanced settings dialog to see how to it is set up as a custom rolling date range._

## Visualize dates in charts

Any chart in **Insights** can display date dimensions. However the time series and area chart are optimized to display date-based information, because they include a _time dimension_. The time dimension specifies how you want to aggregate the data according to the date unit.

For example, if you use a time dimension that has a type of Date, your chart shows aggregated data by year, month, and day. If you choose a time dimension with a type of Year Month, your data is aggregated by those units (year and month). In addition, the time series and area charts automatically sort by date, whereas other charts allow sorting by any dimension or metric.

### Comparison date range

Some charts can compare the current date range to another range in the past. For example, in a time series, the comparison data appears as a line of a different color from the current data. In a table, the comparison data is shown as the delta from the current data, with an increase or decrease indicator.

_While viewers can use the_ [_date range control_](broken-reference) _to set the current time frame for a chart, only report editors can set the comparison date range._

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdGm5mvHU95Rq2VkOZ1rwBNceEYofVhA_wglAFV2S0yliTH2DkiFCkpm3P_51KmX2ybCttizzMmmhotGjk0zYdWlxtKyEArnzwsFy-3O_6ON89APcIpnwBJbBRe2jO_Jc8xSqg_RyyuAlJE_LfxdYmTB8AJ?key=c3wH37wA9h3h9ApPDZt-ng" alt=""><figcaption></figcaption></figure>

### Set up a comparison date range

1. Select a time series, table, area chart, or scorecard.
2. On the right, in the DATA tab of the properties panel, scroll down to the _Default Date Range_ section.
3. Under _Comparison date range,_ choose the comparison period.
4. Click **APPLY**.

**Examples**

**Previous period / previous year**&#x20;

Assume today's date is January 1, 2019, and the currently selected period for the chart is **Last 7 days**:

| **Comparison period**                             | **Current dates**                      | **Comparison dates**                   |
| ------------------------------------------------- | -------------------------------------- | -------------------------------------- |
| Previous period                                   | December 25, 2018 to December 31, 2018 | December 18, 2018 to December 24, 2018 |
| Previous year                                     | December 25, 2018 to December 31, 2018 | December 25, 2017 to December 31, 2017 |
| <p>Fixed</p><p>June 1st, 2018 to June 7, 2018</p> | December 25, 2018 to December 31, 2018 | June 1, 2018 to June 7, 2018           |

Now, assume today's date is January 2, 2019:

| **Comparison period**                             | **Current dates**                    | **Comparison dates**                   |
| ------------------------------------------------- | ------------------------------------ | -------------------------------------- |
| Previous period                                   | December 26, 2018 to January 1, 2019 | December 19, 2018 to December 25, 2018 |
| Previous year                                     | December 26, 2018 to January 1, 2019 | December 26, 2017 to January 1, 2018   |
| <p>Fixed</p><p>June 1st, 2018 to June 7, 2018</p> | December 26, 2018 to January 1, 2019 | June 1, 2018 to June 7, 2018           |

**Advanced date comparison**

Compare the last 30 days from yesterday to the 30 days prior to that, aligned by day of the week (e.g., compare Monday to Monday).

| Current date range             | Comparison date range |
| ------------------------------ | --------------------- |
| Last 30 days (excluding today) |                       |

Compare year to date to two years ago.

| Current date range          | Comparison date range |
| --------------------------- | --------------------- |
| This year (excluding today) |                       |
