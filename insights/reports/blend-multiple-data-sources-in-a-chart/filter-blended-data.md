---
description: Focus on specific data in charts based on blended data sources.
---

# Filter blended data

Insights provides two ways to filter the data shown in charts:

* [_Filter properties_](https://support.google.com/datastudio/answer/6291066), which allow report editors to filter by dimension or metric values, and
* [_Filter controls_](https://support.google.com/datastudio/answer/6312144), which report viewers can use to filter the data by selected dimension values.

For the most part, filtering charts based on blended data sources works in the same was as filtering charts based unblended data sources, but there are a few differences of which you should be aware.

### Filter a blended chart directly <a href="#filter-a-blended-chart-directly" id="filter-a-blended-chart-directly"></a>

Filter properties applied directly to charts based on blended data sources act on the blended data, as opposed to the underlying (pre-blended) data.

#### Apply an already existing filter

You can apply an existing filter to a chart based on a blended data source as long as that filter uses the same blended data source as the chart. **You can't apply a filter based on an unblended data source to a blended chart**.

### Filter individual data sources in the blend <a href="#filter-individual-data-sources-in-the-blend" id="filter-individual-data-sources-in-the-blend"></a>

You can restrict the data from a specific data source used in a chart by editing the blended data source and applying a filter in the _Blend Data_ panel. This filters the data before it is joined with the other data sources in the blend.

#### To filter a data source in a blend

1. [Edit](https://support.google.com/datastudio/answer/9061277?hl=en\&ref_topic=9061419#edit-blended-data-sources) the blended data source.
2. Choose one of the component data sources.
3. At the bottom of the data source panel, click **ADD A FILTER**.

#### Apply an already existing filter

You can apply an existing filter to a data source in the blend as long as that filter was created using the same data source. **You can't apply a filter based on a different data source**.

### Filter controls and inherited filters <a href="#filter-controls-and-inherited-filters" id="filter-controls-and-inherited-filters"></a>

Inherited filters and charts based on blended data sources must share have compatible schemas (field structure), otherwise the filter won't be applied. If a filter is compatible with pre-blended data, then filter controls, as well as inherited report, page, or group level dimension filters act on the data before it has been blended. Otherwise, the filter acts on the data after it has been blended. Inherited metric filters act on the pre-blended data, if possible.

#### Under the hood: inherited filters and blended data

When a chart based on a blended data source in your report is subject to an inherited filter, Data Studio processes the data in 5 steps:

**(Pre-blend)**

> * **Step 1:** The data is grouped and aggregated based on the dimensions specified in the _Blend Data_ panel.
> * **Step 2:** Inherited dimension filters and compatible metric filters are applied to the data sources included in the _Blend Data_ panel.

**(Blend)**

> * **Step 3:** The data is blended using the specified join keys.

**(Post-blend)**

> * **Step 4:** The data is grouped and aggregated based on the dimensions in the chart.
> * **Step 5:** Metric filters, if compatible with blended data, are applied to the chart.

### Related resources <a href="#related-resources" id="related-resources"></a>

* [About filter properties](broken-reference)
* [Let viewers filter the data with filter controls](broken-reference)
