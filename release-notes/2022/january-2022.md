# January 2022

These are the features and improvements released during the month of January 2022

## Releases

* [Add BO Promotion Code](https://app.gitbook.com/s/mECwNqMNUmu6OXHSYgDv/release-notes/2022/january-2022-release-note#add-bo-promotion-code)
* [SQL Workspace](https://app.gitbook.com/s/mECwNqMNUmu6OXHSYgDv/release-notes/2022/january-2022-release-note#sql-workspace)

### Add BO Promotion Code

BO Promotion code is opened to expand user’s demand.&#x20;

Example: The need to add attributes for promotion codes to use in campaigns

<figure><img src="../../.gitbook/assets/image (2324).png" alt=""><figcaption></figcaption></figure>



BO Promotion code includes 4 tabs: Data Table, Attribute, Groups, Settings.\
Note: no Collection tab.

**Data table**:&#x20;

* Data table supports action: Filter, Search, Modify column, Search go to (Promotion Code), Export. Not support selection action yet.

<figure><img src="../../.gitbook/assets/image (1094).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (2018).png" alt=""><figcaption></figcaption></figure>

* When searching go to, filter will be applied at the Data table by promotion code

<figure><img src="../../.gitbook/assets/image (800).png" alt=""><figcaption></figcaption></figure>

* When clicking on Pool ID in the Data table, All promotion pools will be displayed with a filter by pool id.

<figure><img src="../../.gitbook/assets/image (1639).png" alt=""><figcaption></figcaption></figure>

**Attributes:**

Attribute supports action:&#x20;

* Filter&#x20;
* Search&#x20;
* Modify column&#x20;
* Search go to (Attribute name)&#x20;
* Selection action:&#x20;
  * Make a copy&#x20;
  * Change assign group Create attribute

**Group**

Support action similar to other BOs

**Setting**

SDK: status disabled, not allow to change

**Relative feature**

Add Promotion code attribute for Add Personalization

<figure><img src="../../.gitbook/assets/image (1423).png" alt=""><figcaption></figcaption></figure>

### SQL Workspace

**Add “Analysis” parent menu**, including 3 submenus:

* SQL Workspace
* Data Explorer
* Schedule Query

<figure><img src="../../.gitbook/assets/image (483).png" alt=""><figcaption></figcaption></figure>

**Left panel:**

<figure><img src="../../.gitbook/assets/image (1690).png" alt=""><figcaption></figcaption></figure>



1. List of Business Objects tables&#x20;
2. List of Event tables corresponding to Source&#x20;
3. List of Analytic tables created by (6)&#x20;
4. Clicking on table will open table detail Tab&#x20;
5. Hover on table will show Ellipsis, clicking on Ellipsis will show 3 actions: Open, Query, Delete (Only show when it is an analytic table)
6. Add analytic table button. Clicking on will open create analytic table popup

**Table details:** List of columns are attributes of BO/Event

<figure><img src="../../.gitbook/assets/image (1362).png" alt=""><figcaption></figcaption></figure>

**Create analytic table:**

<figure><img src="../../.gitbook/assets/image (2366).png" alt=""><figcaption></figcaption></figure>

* **Add field**: Add columns to analytic table

**Query Editor:** Input query

<figure><img src="../../.gitbook/assets/image (739).png" alt=""><figcaption></figcaption></figure>

**Query result**: After user input query and clicking on Run button

<figure><img src="../../.gitbook/assets/image (2282).png" alt=""><figcaption></figcaption></figure>

**Save Queries**: Listing Saved queries

<figure><img src="../../.gitbook/assets/image (2302).png" alt=""><figcaption></figcaption></figure>

**Explore Data:** The same Explorer project, Available fields and Data are columns of Query Result (Only enable Expore data button when successfully run query)

<figure><img src="../../.gitbook/assets/image (2023).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (1589).png" alt=""><figcaption></figcaption></figure>

**Save result**: Save data from Query result to Analytic table (Only enable Expore data button when successfully run query)

<figure><img src="../../.gitbook/assets/image (1637).png" alt=""><figcaption></figcaption></figure>

* Select Analytic table to Save result
* Mapping columns of Query result with selected Analytic table
* Write mode: Methods of processing and storing data

**Schedule**: Set up a schedule to execute the query and save results into the Analytics table (Only enable Expore data button when successfully run query)

<figure><img src="../../.gitbook/assets/image (2395).png" alt=""><figcaption></figcaption></figure>

* (1) Schedule name&#x20;
* (2) Select Analytic table to Save result after execute query&#x20;
* (3) Mapping columns of Query result with selected Analytic table&#x20;
* (4) Write mode: Methods of processing and storing data&#x20;
* (5) Set up a schedule to execute the query and save results into the Analytics table&#x20;
* (6) Send email/notification after the schedule runs completely

<figure><img src="../../.gitbook/assets/image (1067).png" alt=""><figcaption></figcaption></figure>

**Schedule query**: List of created Schedule Query

<figure><img src="../../.gitbook/assets/image (887).png" alt=""><figcaption></figcaption></figure>

**Run history:**

<figure><img src="../../.gitbook/assets/image (1739).png" alt=""><figcaption></figcaption></figure>

## Updates

* [The promotion pool allows to adjust the allocation restriction type after creating a new one](https://app.gitbook.com/s/mECwNqMNUmu6OXHSYgDv/release-notes/2022/january-2022-release-note#the-promotion-pool-allows-to-adjust-the-allocation-restriction-type-after-creating-a-new-one)

**The promotion pool allows to adjust the allocation restriction type after creating a new one**

&#x20;

<figure><img src="../../.gitbook/assets/image (2567).png" alt=""><figcaption></figcaption></figure>
