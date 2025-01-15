# Data Objects

## INTRODUCE

A data object is a location where you can store your data. If you have a variety of data sources, you'll need to create and organize these sources within data objects to utilize them on CDP 365.&#x20;

## CREATE A NEW DATA OBJECT

In **Data Objects** menu, click **+** to generate a new data object.

<figure><img src="../../../.gitbook/assets/image (3766).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (3767).png" alt=""><figcaption></figcaption></figure>

Afterward, entering some basic information:

* **Object name**: provide a name for your data object
* **Object code**: the system will generate an object code based on the 'Object name.' You can modify the object code as needed. Please note that each data object is identified by a unique object code.
* **Description**: optionally, provide additional information.
* **BO owner**: display the account name of the individual who created the data object.

<figure><img src="../../../.gitbook/assets/image (3768).png" alt=""><figcaption></figcaption></figure>

### 1. General settings

We offer two methods for updating data in a data object: 'interactive through API' and 'SDK'.&#x20;

* **Interactive through API**: this method allows you to update the data of a data object via APIs.
* **SDK**: this method enables you to use event data to update a data object.
* **Update data from event constantly**: typically, with event data, we impose a limit on the time interval between two data updates. However, if you select the option 'Constantly update data from events,' the event data will be immediately updated in the data object.&#x20;

### 2. Share access

'Share access' feature allows you to configure accounts that can view and use your data objects. To add accounts with whom you want to share your data object, enter their email addresses at \[1].

**People with access**: displays the accounts you have added. For each account, you can also modify their permissions. There are two types of permissions:&#x20;

* **Viewer**: allows only viewing of the data object and prohibits any modifications.
* **Editor**: permits modifications to the data object, such as uploading data, removing data, changing configurations, adjusting permissions, etc.

In addition, we also provide the following two functions.

* **Remove access**: removal of added accounts from the data object.
* **Transfer ownership**: if you wish to change the owner of a data object, you can use this option. Please note that the 'Transfer ownership' option is displayed in the configuration of a data object only if you are the creator of it.

<table><thead><tr><th width="499">Permission</th><th width="132" align="center">Viewer</th><th align="center">Editor</th></tr></thead><tbody><tr><td>Search/ filter/ modify column/ explore/ export data table</td><td align="center">x</td><td align="center">x</td></tr><tr><td>Upload data table</td><td align="center">-</td><td align="center">x</td></tr><tr><td>Action toward data row (remove data row)</td><td align="center">-</td><td align="center">x</td></tr><tr><td>Search/ filter/ modify column/ export attribute</td><td align="center">x</td><td align="center">x</td></tr><tr><td>View attribute computation histories</td><td align="center">x</td><td align="center">x</td></tr><tr><td>View configuration of existing attribute</td><td align="center">x</td><td align="center">x</td></tr><tr><td>Create new attribute</td><td align="center">-</td><td align="center">x</td></tr><tr><td>Upload attribute</td><td align="center">-</td><td align="center">x</td></tr><tr><td>Modify configuration of existing attribute</td><td align="center">-</td><td align="center">x</td></tr><tr><td>Action toward attribute (change status, make a copy, change assign group, rebuild)</td><td align="center">-</td><td align="center">x</td></tr><tr><td>Search/ filter/ modify column/ export collection</td><td align="center">x</td><td align="center">x</td></tr><tr><td>View configuration of existing collection</td><td align="center">x</td><td align="center">x</td></tr><tr><td>View collection computation histories</td><td align="center">x</td><td align="center">x</td></tr><tr><td>Restore collection version history</td><td align="center">-</td><td align="center">x</td></tr><tr><td>Create new collection</td><td align="center">-</td><td align="center">x</td></tr><tr><td>Modify configuration of existing collection</td><td align="center">-</td><td align="center">x</td></tr><tr><td>Action toward collection (change status, make a copy)</td><td align="center">-</td><td align="center">x</td></tr><tr><td>Search/ filter/ modify column/ export group</td><td align="center">x</td><td align="center">x</td></tr><tr><td>View group infomation</td><td align="center">x</td><td align="center">x</td></tr><tr><td>Modify group</td><td align="center">-</td><td align="center">x</td></tr><tr><td>Create new group</td><td align="center">-</td><td align="center">x</td></tr><tr><td>Action toward group (remove)</td><td align="center">-</td><td align="center">x</td></tr><tr><td>View configuration of data object</td><td align="center">x</td><td align="center">x</td></tr><tr><td>Modify configuration of data object</td><td align="center">-</td><td align="center">x</td></tr><tr><td>Use data object for segmentation</td><td align="center">x</td><td align="center">x</td></tr><tr><td>Use data object at 'Customer' &#x26; 'Visitor' menu (apply only for 'Customer' and 'Visitor' data object)</td><td align="center">x</td><td align="center">x</td></tr><tr><td>Use data object to create data view</td><td align="center">x</td><td align="center">x</td></tr></tbody></table>

<figure><img src="../../../.gitbook/assets/image (3769).png" alt=""><figcaption></figcaption></figure>

**General access**: we offer two options, including Restricted and Public.

* **Restricted**: share your data object only with accounts added to 'People with access'.
* **Public**: allows you to share your data object with all accounts.

<figure><img src="../../../.gitbook/assets/image (3770).png" alt=""><figcaption></figcaption></figure>

## ACTIONS WITH DATA OBJECT

<table><thead><tr><th width="187">Action</th><th>Description</th><th data-hidden></th></tr></thead><tbody><tr><td>Enable</td><td>Activating a data object will switch its status to 'Enabled.' If the data object remains unused for a designated period, its status will automatically switch to 'Disabled.'</td><td></td></tr><tr><td>Disable</td><td><ul><li>Disabling a data object will transition its status to 'Disabled,' preventing further input to the data object and rendering it unusable in any function.</li><li>If the data object remains disabled for a specified period, it will automatically switch to 'Archived' status.</li></ul></td><td></td></tr><tr><td>Archive</td><td><ul><li>Archiving a data object will cease all input and output operations associated with the data object. Consequently, the data object will no longer appear in any data object selector lists.</li><li>If the data object remains archived for a specified duration without being re-enabled, it will be permanently deleted.</li></ul></td><td></td></tr><tr><td>Recover</td><td>Restore archived data objects. During recovery, the status of the data object can be changed to either enabled or disabled.</td><td></td></tr></tbody></table>

<figure><img src="../../../.gitbook/assets/image (3771).png" alt=""><figcaption></figcaption></figure>

## ELEMENTS OF A DATA OBJECT

<table><thead><tr><th width="182">Tab</th><th>Description</th></tr></thead><tbody><tr><td><a href="data-table.md">Data table</a></td><td><ul><li>Give detailed data of a data object. </li><li>The columns are attributes and the rows are attribute values.</li></ul></td></tr><tr><td><a href="attributes/">Attributes</a></td><td><ul><li>Fully inform these data objects. </li><li>For example, a Customer data object has attributes such as name, date of birth, number of success orders, number of complaints, etc.</li></ul></td></tr><tr><td><a href="collections.md">Collections</a></td><td><ul><li>Manage collections of data extracted from a data object by complex conditions of attributes.</li></ul></td></tr><tr><td><a href="groups.md">Groups</a></td><td><ul><li>Categorize attributes of a data object into groups which make management productive. </li></ul></td></tr><tr><td><a href="setting.md">Setting</a></td><td><ul><li>Give the settings information of data objects.</li></ul></td></tr></tbody></table>

<figure><img src="../../../.gitbook/assets/image (3772).png" alt=""><figcaption></figcaption></figure>
