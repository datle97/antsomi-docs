# Quick start guide

This article explains **six key steps** that will help you get started quickly using **Insights**.

_Throughout this User Guide, Glossary provides more information on selected terms. Hover over the link to display a summary, or click the link to jump to the full definition. There is table at the end of this article summarizing the terms used here._&#x20;

_Insights are flexible tools: there are often multiple ways to achieve the same results. The workflow described here is just a basic example._

## ![](<../.gitbook/assets/image (1445).png>) Start with a report

[Reports](reports/create-reports/about-reports.md) let you visualize your data, gain insights, and share those insights with others.

### Instructions

When you sign in **Insights**, you'll see the default page is **Report** with the **My Reports** tab selected. All the reports to which you are owner appear in the screen. The plus buttons let you create a new blank report, or start with a pre-built report template.



#### Create a report

1. In the top left, click <img src="../.gitbook/assets/image (761).png" alt="" data-size="original">.

<figure><img src="../.gitbook/assets/image (3870).png" alt=""><figcaption></figcaption></figure>

Select a default data source for your report by how to select to a source data in the new mailbox and the select **Continue.**

_Notes: The report is created from the selected data source. To_ [_create a data source_](data-source/create-a-data-source.md)_, please read it._

In a moment, you'll see the report editor, with a blank canvas.

<figure><img src="../.gitbook/assets/image (3873).png" alt=""><figcaption></figcaption></figure>

## ![](<../.gitbook/assets/image (816).png>) Add charts and controls to the report

Use the menus and toolbar to add [components](reports/create-reports/build-stylize-and-add-data-to-reports/add-and-configure-components.md) to the report canvas. Use the properties panel on the right to configure the data and style options for the selected items.

1. On the toolbar, select a component (chart, control, or others)
2. Move and resize the chart, as desired.
3. Add or change the dimensions and metrics by clicking the fields in the properties panel, or dragging and dropping them from the Available Fields panel (to the right of the properties panel).

## ![](<../.gitbook/assets/image (2341).png>) View your report



See your report the way it looks to other viewers.

### Instructions

View mode lets you see all the data and use any interactive controls you've placed on the report to change that data. You can not change the structure of the report in view mode.

#### Switch between view and edit modes

1. In the upper right, clicks ![](<../.gitbook/assets/image (3874).png>). You are now in **view** **mode**.
2. To return to **edit mode**, click ![](<../.gitbook/assets/image (3875).png>).

## ![](<../.gitbook/assets/image (1227).png>) Share the report



Share reports with other viewers. Collaborate with other editors.

### Instructions

Editors need to sign into Insights to edit the report but viewers do not need to be signed in.

#### Share a report

1. In the upper right, click ![](<../.gitbook/assets/image (3876).png>)
2. Select Invite people from the drop-down list.
3. Specify the people and/or groups with whom you want to share your data source.

<figure><img src="../.gitbook/assets/image (3877).png" alt=""><figcaption></figcaption></figure>

_Sharing a report doesn't share its data source._

## ![](<../.gitbook/assets/image (837).png>) Share the data source

Let other people create their own reports based on your data source.

### Instructions

_There is no need to share a data source if you only want other people to view or edit your reports._

To share a data source, you must access it **directly from the DATA SOURCES home page** (not via the report). You must be signed into Insights to view or edit a data source.

#### Share a data source

1. Hover your mouse over **Data**, choose **Sources**.
2. Find the data source you want to share and click on it to go to the details page.
3. Go to **Settings** tab, then access **Data Freshness and Share**.

<figure><img src="../.gitbook/assets/image (3879).png" alt=""><figcaption></figcaption></figure>

4. Specify the people and/or groups with whom you want to share your data source

<figure><img src="../.gitbook/assets/image (3880).png" alt=""><figcaption></figcaption></figure>

_Use caution when sharing a data source with edit access. While sharing does not grant access to the underlying data, modifying a data source could cause it to be incompatible with existing charts that use that data source. Sharing a data source with view access lets people create reports without being able to change its structure._

## Key concepts

Here is a recap of the terms and concepts used in this article and throughout this Help Center.

<table><thead><tr><th width="257">Concept</th><th> What it does</th></tr></thead><tbody><tr><td>Report</td><td><p>An <strong>Insights</strong> file that contains a collection of <em>components</em> whose purpose is to present to viewers information and insights derived from your data.</p><p>Learn more <a href="reports/create-reports/about-reports.md">about report</a>.</p></td></tr><tr><td>Component</td><td><p>A widget you add to a report to display your data, such as <strong>charts</strong>, <strong>tables</strong>, and interactive <strong>date range controls</strong> and <strong>filter controls</strong>. Data components get their information from a <em>data source</em>.</p><p>You can also annotate your report with <strong>text</strong>, <strong>shape</strong>, <strong>image</strong>, and embedded content components.</p></td></tr><tr><td>Connector / Data source</td><td><p><br>Connecting to your data involves two components that work together:</p><ul><li><strong>Connectors</strong> connect <strong>Insights</strong> to your underlying data. Connecting to your data creates a <em>data source</em> in <strong>Insights</strong>.</li><li><strong>Data sources</strong> represent a particular instance of a connector: for example, a connection to a specific MySQL table, or Google Sheet. Data sources let you configure the fields and options provided by the connector used to create that connection instance. In addition, the data source gives you a secure way to share information and insights with report viewers who may not be able to directly access the underlying data.</li></ul><p>Learn more about <a href="reports/create-reports/build-stylize-and-add-data-to-reports/add-and-edit-data.md">connecting to your data</a>.</p></td></tr><tr><td>Field</td><td><p>A column of data.</p><p>There are 2 basic kinds of fields in Insights:</p><ul><li><strong>Dimensions</strong> are things you want to measure, or that serve as ways to categorize your data.</li><li><strong>Metrics</strong> are numbers that measure the things contained in dimensions.</li></ul><p>Learn more about <a href="reports/glossary/field.md">fields in reports</a>.</p></td></tr><tr><td>View mode / Edit mode</td><td><p></p><ul><li><p><strong>Edit mode</strong> allows you to edit the structure of a report and change, add, or remove data sources.</p><ul><li>People who can edit a report or data source are referred to as <em>editors</em>.</li></ul></li></ul><ul><li><p><strong>View mode</strong> allows you to see all the data you are authorized to see, and to use interactive viewer controls. View mode does not allow you to modify the report structure.</p><ul><li>People who can only view a report or data source are referred to as <em>viewers</em>.</li></ul></li></ul><p></p></td></tr><tr><td>Sharing and file access</td><td><p>When you share reports and data sources, you determine how other people can access the file:</p><ul><li><strong>Can edit</strong> access lets people modify the file (making them <em>editors</em>).</li><li><strong>Can view</strong> access lets people view the file, but they can't modify it (making them <em>viewers</em>).</li></ul><p>The advanced sharing options let you control other aspects of file access, such as the ability to download the data or print the report.</p><p>The link sharing options let you share your files more broadly around the internet.</p></td></tr></tbody></table>

