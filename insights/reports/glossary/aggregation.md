---
description: The method used to summarize data.
---

# Aggregation

In general data science terms, an aggregation is "a function or field where the values of multiple rows are grouped together as input on certain criteria to form a single value of more significant meaning or measurement." (Source: [Wikipedia](https://en.wikipedia.org/wiki/Aggregate_function))

In **Insights**, fields can have the following aggregation methods:

* `Average`
* `Count`
* `Count Distinct`
* `Max`
* `Min`
* `Sum`
* `Auto`
* `None`

`Auto` is applied by **Insights** and cannot be changed.

`None` is applied to dimensions and unaggregated metrics. You can change this for metrics in the data source and report. If left as None in the data source, the default aggregation in reports is `Sum`.

### Related resources <a href="#related-resources" id="related-resources"></a>

* [About dimensions and metrics](broken-reference)
