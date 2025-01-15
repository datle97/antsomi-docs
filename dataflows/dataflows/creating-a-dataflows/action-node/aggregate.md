# Aggregate

Used to group by the current data of this branch according to the Dimensions (Group by) and Metrics (Aggregate) of the existing columns.

<figure><img src="../../../../.gitbook/assets/image (493).png" alt=""><figcaption></figcaption></figure>

## Group by

Used to setup column group by (dimension). Default pre-selects columns with datatypes of Text, Datetime, Geo, Hyperlink, Image

The number of data lines after this node will be equal to the number of distinct combinations of columns selected in this Group by.

Columns that have been selected in Group by will not appear in Aggregate and in other lines of Group by.

## Aggregate

Used to select which column is the metric and select the corresponding Aggregation. Default pre-selects columns with datatypes of Number, Percent and Currency with Aggregation of Sum

Clicking Add aggregate will display a list of unselected columns in Group by to select. Columns already selected in Aggregate can still be reselected.

## Available field

List of columns available in this branch. Allow drag and drop on the above 2 components according to the rules

**Note:**

* A column may not be selected in Group by or Aggregate
* If any column is not selected, it will be removed from the data of this branch
