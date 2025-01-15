# Create a Data Source

From Data Sources main page, click <img src="../../.gitbook/assets/image (466).png" alt="" data-size="line"> to create a new Data Source

<figure><img src="../../.gitbook/assets/image (1501).png" alt=""><figcaption></figcaption></figure>

A page will show up to select the connector of this data source as below:

<figure><img src="../../.gitbook/assets/image (2251).png" alt=""><figcaption><p>Select a data source</p></figcaption></figure>

1. Input name for Data Source
2. Input keywords to look for the desire connector.
3. Click **Select** to select the connector.&#x20;

After selecting the desire Connect, an authentication step will be processed. For each type of Connector selected, different authentication information needs to be input. [Learn more](data-source-connectors/)

After finishing authentication step, a data sheet/source of the Connector should be selected to used as the data source for Dataflow.

<figure><img src="../../.gitbook/assets/image (785).png" alt=""><figcaption></figcaption></figure>

4. Click **Select Connector** to get back to selecting Connector page previously.
5. Select a data sheet/source to use as the data source. Depending on the selected connector, the process to select the data source at this step would be different. [Learn more](data-source-connectors/)
6. Click **Cancel** to cancel the data source creation and get back to the main page of the Data Source.
7. Click **Connect** to connect selected data sheet/source to use this data sheet/source A popup will be shown as following to select the field in the selected data sheet/source:

#### Set up the fields

<figure><img src="../../.gitbook/assets/Screenshot 2023-03-26 170624.png" alt=""><figcaption><p>Field selection</p></figcaption></figure>

8. Search the desire field.
9. Click <img src="../../.gitbook/assets/image (2549).png" alt="" data-size="line">to select/unselect a field.
10. Turn on if user only want to show the selected field.
11. Name of the field in the connector's data sheet/source.
12. Name of the field would be shown in CDP 365 Data Source.
13. Data Type of the field
14. There are two option of Treat as:

* **Attribute:** This field would be used as the attribute.
* **Measure:** This field would be used as a measurable field in data source. The aggregation for this calculation is at step (15)

15. If the Treat as at step (14) is **Measure**, there are some options of aggregation can be selected as following:

![](<../../.gitbook/assets/Screenshot 2023-03-26 171056.png>)&#x20;

16. Input the description for a field.
17. Click **Apply** to use the selected field of the data sheet/source and finish creating a new Data source. The detail of created data source will be displayed as below.

<figure><img src="../../.gitbook/assets/image (673).png" alt=""><figcaption></figcaption></figure>

To View/Edit a data source, please see in [this link](view-edit-a-data-source.md).

18. Click **Cancel** or <img src="../../.gitbook/assets/image (1792).png" alt="" data-size="line">to cancel the field selection and close the popup.
