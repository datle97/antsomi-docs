---
description: Understand how filter controls work in reports with multiple data sources.
---

# Use controls across data sources

In a report based on a single data source, a control affects all the charts and other controls in the report. In reports with multiple data sources, how the control works depends on the data sources involved.

As a general rule, controls can filter charts from different data sources as long as the data sources share the same internal structure (schema). In practice, this means that you can filter across data sources if:

a) the data sources were created using the same [connector](broken-reference), and

b) the data sources have a fixed schema, with a predefined set of fields.

For example, a control based on the Google Analytics _Country_ dimension applies to all components on the page that also use a Google Analytics data source, even if they connect to different views. This is because all Analytics data sources have the same default field set. (Note that optional features in Analytics, such as Enhanced Ecommerce, will produce additional fields that may not exist in all Analytics data sources, and therefore, not be compatible with controls based on properties or views without those features.)

Filtering across data sources generally won't work if the charts involved are based on data sources of different types, even if the fields have the same visible name. This is because filtering is based on the _internal_ field IDs, not the visible field names in the data source. (And, once a field has been created in the data source, you can't edit the internal ID.)

### Example

Say you have a report with 3 different data sources: one from Google Sheets, and two from Analytics. Even if all three data sources include a field with the visible name of "Country," only the Analytics data sources share the same internal structure. A control for the Analytics charts can use the _Country_ dimension from either data source, but it won't filter the Google Sheets chart. Conversely, a control based on the Sheets _Country_ dimension will filter the Sheets-based chart, but won't affect the Analytics charts.

The embedded report below illustrates the limits of cross data source filtering.

* Controls don't affect charts based on data sources with different schemas
* This report includes 3 data sources: one from Google Sheets (left) and 2 from Analytics (right).
* The Analytics-based control affects both of the Analytics-based charts because their data sources share the same schema.
* The Sheets-based control only affects the Sheets-based chart, because its schema doesn't match the Analytics data source schema.
* (The internal names of the dimensions are different between Sheets and Analytics.)
