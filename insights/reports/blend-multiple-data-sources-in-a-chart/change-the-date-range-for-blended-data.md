# Change the date range for blended data

You can control the date range of charts with blended data in three ways:

* Set the date range for individual data sources in the blend.
* Set the date range for a chart based on a blended data source.
* Use a date range control.

### Set the date range for individual data sources in the blend

Use the date range options for one or more of the data sources in the blend. This selects the data from this data source before it is joined with the other data sources in the blend.

#### To change the date range for a data source in a blend <a href="#to-change-the-date-range-for-a-data-source-in-a-blend" id="to-change-the-date-range-for-a-data-source-in-a-blend"></a>

1. [Edit](https://support.google.com/datastudio/answer/9061422?hl=en\&ref_topic=9061419#edit-blended-data-sources) the blended data source.
2. Choose one of the component data sources.
3. Configure the _Date range_ options
   1. Dimension — the date dimension which controls the time frame of the data source.
   2. Auto — use the chart's time frame.
   3. Custom — override the chart's time frame. This will also override a time frame set by the date range control.

TIP: Setting the date range in the blended data source to Auto provides the most flexibility, since you can control the date range using the chart's property panel, or using a date range control :TIP

### Set the date range for a chart based on a blended data source <a href="#set-the-date-range-for-the-blended-chart" id="set-the-date-range-for-the-blended-chart"></a>

You can apply a date range to charts based on blended data sources in the same way as charts based on a single data source. Date ranges applied to the chart act on the data after it's been blended. Custom date settings in the blended data source override the chart's settings.

### Use a date range control <a href="#use-a-date-range-control" id="use-a-date-range-control"></a>

Date range controls let report viewers select a time frame for the report. If you've set custom date ranges for either the blended data source or the blended chart, those settings override the date range control.

### Related resources <a href="#related-resources" id="related-resources"></a>

* [Set report date ranges,](broken-reference)
* [Add a date range control to a report](broken-reference)
