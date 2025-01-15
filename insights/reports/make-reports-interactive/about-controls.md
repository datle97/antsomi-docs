---
description: Let viewers apply filters and set parameter values.
---

# About controls

Controls let viewers interact with the data displayed in a Insights report in the following ways:

* Viewers can filter the data by specific dimension values.
* Viewers set the time frame of the report.

To learn how to filter the data before viewers see it, use a [filter property.](broken-reference)

### Add a control to a report <a href="#add-a-control-to-a-report" id="add-a-control-to-a-report"></a>

1. Edit your report.
2. In the toolbar, select <img src="../../../.gitbook/assets/image (569).png" alt="" data-size="line">
3. Select the control type, then position on the page.
4. On the right, use the options in the properties panel to configure the control.
   1. To filter the report by selected dimension values, use a dimension for the **Control field**.

### How controls work <a href="#how-controls-work" id="how-controls-work"></a>

Controls let viewers filter or change the data displayed in the report's components.

#### Controls as filters

When a control is based on a dimension (you add a dimension from the available fields list as the **Control field**), the control acts as a filter on the data.

For example, a list control based on the _Country_ dimension let the viewer filter the data by country. An advanced filter based on a _Product SKU_ dimension lets the viewer filter by all or partial part numbers.

**More about filters**

Controls filter all components on the page based on the same data source as the control itself.&#x20;

Controls can filter other controls. For example, say you have one filter on the Country dimension, and a second filter on the Campaign dimension. Filtering on Country = France causes the Campaign filter to only show campaigns that ran in France. Similarly, filtering on campaign "ABC" restricts the Country filter to only those countries where that campaign ran.

Controls can only filter by a single dimension. To create a control that filters by more than one dimension, you have several options:

* Create multiple filter controls, one for each dimension you want to filter by.
* Concatenate the dimension data you want to filter by in a calculated field in the data source.
* Concatenate the dimension data you want to filter by in the underlying data, if possible.

_**Data Source**_

_Provides the dimensions you can use in the control._

_**Date range dimension**_

_This option appears if your data source has a valid date dimension._

_The Date Range Dimension is used as the basis for limiting the date range of the chart. For example, this is the dimension used if you set a date range property for the chart, or if a viewer of the report uses a date range control to limit the time frame._

_**Dimension**_

_Provides the list of values that appear in the control._

_**Control field**_

_The dimension to filter by or the parameter whose value is set by this control._

_**Default selection**_

_Specify default values, separated by commas. Be sure to enter the values exactly as they appear in your data._

_**Metric**_

_This option displays a reference metric in the control. You can use this to sort the list, however, the viewer can't filter based on a metric value. To hide the metric, uncheck the **Show values** option._

_**Decimal precision**_

_Specify the number of digits in the metric value to show._

_**Order**_

_This option controls the sort order and number of values listed in the control. You can sort the values list in either ascending or descending order by the dimension values, or by the reference metric._

_**Show top #**_

_This option limits the number of items displayed in the control. If the number of items available exceeds this limit, remaining items are grouped into "All others."_

_**Default Date Range**_

_This option limits the values displayed in the control to the range you specify._

_**Filter**_

_Restrict the data displayed in the control by including or excluding the values you specify._

#### Input box DATA options

_**Data Source**_

_Provides the dimensions and parameters you can use in the control._

_**Dimension**_

_Provides the list of values that appear in the control._

_**Control field**_

_The dimension to filter by or the parameter whose value is set by this control._

#### Input box STYLE options

_**Drop-down**_

_Displays the control in a drop-down box._

_**Fixed-size**_

_Displays the control as a fixed-size box._

_**Input box auto width**_

_When checked, the entry field's width automatically sizes to fit the available space. To set the entry field's width manually, uncheck this option and enter the desired width in characters._

_**Label position**_

_Sets the appearance of the control's label._

_**Search type**_

_Available for controls as filters. Determines the default search operator:_

* _**Is**. The value exactly matches the search term. (Case sensitive.)_
* _**Contains** (Default). The value contains the search term._
* _**Starts With**. The value begins with the search term._
* _**In**. The value matches one or more of the search terms (enter search terms separated by commas)._

_**Label position**_

_Sets the appearance of the control's label._

_**Search type**_

_Determines the default search operator:_

* _**Equals** (default). The value exactly matches the search term. (Case sensitive.)_
* _**Contains**. The value contains the search term._
* _**Starts With**. The value begins with the search term._
* _**In**. The value matches one or more of the search terms (enter search terms separated by commas)._

_You can filter by numeric dimensions values using the following operators:_

* _**Between.** The value is between the starting and ending numbers._
* _**>=** The value is greater than or equal to the number._
* _**>** The value is greater than the number._
* _**<=** The value is less than or equal to the number._
* _**<** The value is less than the number._
* _**In.** The value matches one or more of the search terms (enter search terms separated by commas)_

### Change the control type <a href="#change-the-control-type" id="change-the-control-type"></a>

You can switch an existing control on the report from one type to another:

1. Edit your report.
2. Select the control.
3. On the right, at the top of the properties panel, click on current control name.
4. Select the new control type.

You may need to edit the control's settings to use the new type.

### Make a control appear on every page <a href="#make-a-control-appear-on-every-page" id="make-a-control-appear-on-every-page"></a>

You can make a control appear in the same location on every page of your report. Filters or parameters set on one page will carry over to all the pages in the report.

1. Edit your report.
2. Select the control.
3. Right click, select Make report-level.

Can't find the control on other pages? It may be underneath other components on the page. Learn more about [report-level component position.](broken-reference)
