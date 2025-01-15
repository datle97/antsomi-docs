# Collections

## Navigate to Collections Menu

1. Hover your mouse over **Data**. Choose **Data Objects**.

<figure><img src="../../../.gitbook/assets/image (3680).png" alt=""><figcaption></figcaption></figure>

2. For this example, choose **Product** Data Object.

<figure><img src="../../../.gitbook/assets/image (3681).png" alt=""><figcaption></figcaption></figure>

3. Choose **Collections**

<figure><img src="../../../.gitbook/assets/image (3683).png" alt=""><figcaption></figcaption></figure>

## Create a Collection

You can create a Collection by following the steps:&#x20;

1. Click ![](<../../../.gitbook/assets/image (1649).png>) to create a Collection

<figure><img src="../../../.gitbook/assets/image (3684).png" alt=""><figcaption></figcaption></figure>

2. [Configure the Collection](collections.md#undefined)
3. Click ![](<../../../.gitbook/assets/image (3690).png>)to save and wait for the calculated result by the system&#x20;

<figure><img src="../../../.gitbook/assets/image (3691).png" alt=""><figcaption></figcaption></figure>

### Configure the Collection

#### Update method

<figure><img src="../../../.gitbook/assets/image (3686).png" alt=""><figcaption></figcaption></figure>

| Update Collection | Description                                                                                          |
| ----------------- | ---------------------------------------------------------------------------------------------------- |
| Static            | The final result is computed result after selecting ![](<../../../.gitbook/assets/image (3689).png>) |
| Dynamic           | The result will be recomputed periodically based on the schedule by date or time                     |

{% hint style="info" %}
The collection chooses the Dynamic Collection - scheduled update type will contain the Computation Schedule option. See more about the [Computation Schedule](broken-reference)
{% endhint %}

#### Include item that

<figure><img src="../../../.gitbook/assets/image (3687).png" alt=""><figcaption></figcaption></figure>

The item will be updated to Collection by selecting the method below:

| Item input method | Description                                                                                                                                                                |
| ----------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Add condition     | Collection will be created based on objects that already exist on your CDP 365 system portal. These objects are filtered based on your setting of the _**Have attribute**_ |
| Or bulk select    | The element will be imported into the collection by uploading a data file ​with format .csv, .xlsx, .xls. See more the[ Import](broken-reference) utility                  |

**Forecast**

You can see a sample of users in the audience by clicking **Forecast** on the right hand side of the screen.

<figure><img src="../../../.gitbook/assets/image (3688).png" alt=""><figcaption></figcaption></figure>

### Status of a **Collection**

You can change the status of a Collection by switching ![](<../../../.gitbook/assets/image (732).png>)or ![](<../../../.gitbook/assets/image (410).png>)

### Quick editing name of the Collection

You can edit the name of the segment quickly by following the steps:

1. &#x20;Hover the collection name and choose ![](<../../../.gitbook/assets/image (760).png>)
2. Edit name in the Collections popup
3. Click ![](<../../../.gitbook/assets/image (1884).png>)

<figure><img src="../../../.gitbook/assets/image (3692).png" alt=""><figcaption></figcaption></figure>

### Action with Collection

There are many actions you could do with one or multiple collections. To do so, click on the check box(es) of the collection(s) you want.

#### EDIT

<figure><img src="../../../.gitbook/assets/image (3693).png" alt=""><figcaption></figcaption></figure>

#### Enable

When enabling the collection will change the state of the collection to Enabled.

If within a specified time the segment is not used anywhere, the state is changed to disabled

#### Disable

Disabling the collection changes the state of the collection to Disabled. This will then block the input of the collection. Collection cannot be used in any function.&#x20;

If, within a specified time, the collection is not re-enabled, the collection will automatically change its state to archived.

#### Archive&#x20;

When archive collection will block all output and input of collection. Then the collection will not show up in any collection selector list.

If within a specified time period, the collection is not enabled, it will be deleted forever.

#### Recover

Restore archived segment.

During recovery, the segment's state can be changed to enabled or disabled.

**Make a copy**

Create a new collection with the setting of the chosen one. This only applies when choosing one items.&#x20;

#### LABEL

In order to better distinguish between collections having the same characteristics and the others, you could use **Label** feature. This is especially helpful in many cases such as labeling collections by the team who created it, by seasons of the year or by discount rate, etc.

If there exists available labels, choose on the labels you want and click **Apply**.

<figure><img src="../../../.gitbook/assets/image (3694).png" alt=""><figcaption></figcaption></figure>

To create a new label, click ![](<../../../.gitbook/assets/image (3696).png>) & input necessary information -> click **Create**

<figure><img src="../../../.gitbook/assets/image (3698).png" alt=""><figcaption></figcaption></figure>

## Computed result of collection

#### Quickly see the results in the collection list

<figure><img src="../../../.gitbook/assets/image (3700).png" alt=""><figcaption></figcaption></figure>

You can quickly check the status and number of calculated elements in the data table of the Collection

## Collection Computation Histories&#x20;

### View Collection Computation Histories

Click the icon![](<../../../.gitbook/assets/image (857).png>)on the collection display to view the Collection Computation Histories

<figure><img src="../../../.gitbook/assets/image (3701).png" alt=""><figcaption></figcaption></figure>

### Collection Computation Histories Data table

It presents a data table containing information about collection computation

* **Computation ID:** Every time attribute is computed, it will have an ID
* **Name:** name of the attribute
* **Update method:** type of update method (Static/Dynamic)
* **Computation trigger:** Trigger by the user or Scheduled Update
* **Computation status:** Status of the computation (Success, Computing, Unsuccess, Paused, Waiting)
* **Computation started on:** the date and time that the computation starts
* **Computation ended on:** the date and time that the computation ends
* **Computation duration (sec):** The duration of computation (in seconds)
* **Computation output:** Number of outputs that satisfy the condition after finishing the computation
* **Error info:** Error code that caused compute failed

<figure><img src="../../../.gitbook/assets/image (3702).png" alt=""><figcaption></figcaption></figure>

## Copy a Collection

When you want to create a collection that has similar condition settings to an existing collection, you can use the **Make a copy** feature. After creating a collection copy, you can modify the conditions to match the purpose and save it by selecting **Make a copy**.

### Steps to make a collection copy

1. Select the original collection
2. Select **Make a copy** in Action&#x20;

<figure><img src="../../../.gitbook/assets/image (3703).png" alt=""><figcaption></figcaption></figure>

3. Enter the name and click **Make a copy**

<figure><img src="../../../.gitbook/assets/image (3704).png" alt=""><figcaption></figcaption></figure>

4. Customize conditions&#x20;
5. Select **save** and compute

<figure><img src="../../../.gitbook/assets/image (3707).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Note: The copy is only Saved and calculated when you click ![](<../../../.gitbook/assets/image (1422).png>)
{% endhint %}

## Use cases of Collection

### [How to create a Collection](../../../use-cases/data-hub/business-objects/how-to-create-a-collection.md)
