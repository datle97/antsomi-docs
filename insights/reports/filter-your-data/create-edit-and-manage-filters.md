# Create, edit, and manage filters

## Create a new filter&#x20;

### Step 1: Select the chart&#x20;

Select the chart that you want to refine its data.

Go to the Data tab and find the Filter setting.

Click ![](<../../../.gitbook/assets/image (1467).png>) to set the filter condition.

<figure><img src="../../../.gitbook/assets/image (1787).png" alt=""><figcaption><p>Bar Chart Filter</p></figcaption></figure>

### Step 2: Set the filter condition

If you want to create a new filter, click the button \[1].

A setting block \[2]  on which you set the filter condition will show .

<figure><img src="../../../.gitbook/assets/image (2542).png" alt=""><figcaption><p>Create a filter</p></figcaption></figure>

### Step 3: Include or Exclude the filter value

<figure><img src="../../../.gitbook/assets/image (1137).png" alt=""><figcaption><p>Include or Exclude</p></figcaption></figure>

### Edit a filter

1. Edit your report.
2. Select the chart or control that has the filter.&#x20;
3. Select the **DATA** tab in the _Properties_ panel.
4. Click <img src="../../../.gitbook/assets/image (2599).png" alt="" data-size="line">.

### Reuse an existing filter <a href="#reuse" id="reuse"></a>

Once you've added a filter to a report, you can use it in other components or even other reports. Adding an existing filter to a component _reuses_ that filter. Reusing a filter does not create a copy of the filter. It's actually the same filter, so if you later edit it in one place, that changes the filter everywhere in the report.

If you reuse a filter for a chart or control with an incompatible data source, the chart or control will display an error. You can fix this by editing the filter to use dimensions or metrics that are common to both data sources.

[Learn more about filters and data sources.](broken-reference)

### Copy components and reports with filters

When you make a copy of a page or component within a report, its filters are reused by the copy.

If you copy a filtered component into a different report, Insights makes a new copy of the filter. It has no relationship to the original filter. Note that if you copy and paste the component a second time, you will get another copy of the filter. The 2 copies are not related.

If you make a copy of a report and change the data source, any filters in the report get the new data source.
