---
description: Use filter properties to fine tune your data stories.
---

# About filters

Filter properties (or just filters, for short) refine or reduce the data shown to report viewers. This lets you focus on the data that best communicates the story you want to tell, making your reports more relevant to your audience.

You can apply a filter to a chart, control, page, or the entire report using the DATA properties tab. Filter properties are sometimes referred to as editor filters, because report viewers can't change them. They can only be set by report editors.

### How filters work

There are 2 types of filters:

* **Include filters** retrieve only the records that match the conditions.
* **Exclude filters** retrieve only the records that DON'T match the conditions.

Note that filters do not transform your data in any way. They simply reduce the amount of data displayed in the report.

[Filter conditions](broken-reference) consist of one or more _clauses_. Multiple clauses can be joined with "OR" logic (true if any conditions are met), "AND" logic (true if all conditions are met), or both.

You can apply filters to dimensions or metrics, or both.

#### What you can filter <a href="#what-you-can-filter" id="what-you-can-filter"></a>

You can apply filters to the following components:

* **Charts**. For example, you can display a pie chart of new versus returning users in your biggest markets with a filter including _Country_ **Matches anyUY77777777777HJNM** "`United States,Canada,Mexico,Japan`"
* **Filter controls**. For example, you can let your viewers select from a list of best-selling products on _Quantity Sold_ Greater than (>) `100`.
* **Pages**. Page-level filters apply to every chart on that page. For example, you can dedicate page 1 of your Google Analytics report to mobile app traffic, and page 2 to desktop traffic by filtering on the _Device Category_ dimension.
* **Reports**. Every chart in the report is subject to the filter. For example, you can create a report that focuses on your best customers by setting the report-level filter property to _Lifetime Value_ Greater than or equal to 10,000.

### Filters and data sources <a href="#filters-and-data-sources" id="filters-and-data-sources"></a>

Just like charts, filter properties are associated with a data source. If you create the filter by adding it to a component, that data source is the one in use by the component. If you create the filter using the filter manager, you can select any of the data sources currently added to the report.

Reusing a filter on a component that uses a different data source can render the filter invalid. That's because the dimensions and/or metrics used by the filter may not exist in the new data source.

The same thing can happen if you copy a chart or control to a report that uses a different data source, or if simply change the data source in use by a filter by editing it in the filter manager.

Invalid filters display an error on the chart or control, and a warning icon on the filter. You can fix this by editing the filter and selecting new dimensions or metrics, or by deleting the filter.

### Filter inheritance <a href="#filter-inheritance" id="filter-inheritance"></a>

Filters can be _inherited_, meaning filters on higher level components apply to the components beneath them. The order of inheritance is:

**Report level > page level > chart/control level**

In order for a lower-level (_child_) component to inherit filters from a higher-level (_parent_) component, the dimensions and metrics used in the parent's filters must exist in the child component's data source. If they don't, then inheritance is turned off for the child component.

You can turn off inheritance explicitly by using the toggle in the _Filter_ section of the DATA properties panel for a selected component. For example, you can tell a chart not to inherit a page level filter property, or a page not to inherit the report level one.

### Multiple filters on a component <a href="#multiple-filters-on-a-component" id="multiple-filters-on-a-component"></a>

A component can have multiple filters. When this is the case, each filter is treated like an AND clause. This means that only the data rows that meet all of the conditions in the filter will be affected.

### Limitations of filters <a href="#limitations-of-filters" id="limitations-of-filters"></a>

* Report-level filters only apply to components using the default data source. If you include charts that use a different data source, you'll need to create a chart-level filter for that chart.
* A single component can have a maximum of 100 filters clauses.
* A single filter can have a maximum of 10 OR clauses. If you need more OR clauses, consider using the Matches any option instead.
* Metrics and dimensions cannot be mixed in an OR clause. This is due to how dimensions and metrics are aggregated.
* If you change a field in a data source from a metric to dimension or vice versa, any filters using that field are disabled.

### Related resources <a href="#related-resources" id="related-resources"></a>

* [Filter controls](broken-reference)
