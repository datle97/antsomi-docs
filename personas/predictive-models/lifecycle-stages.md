# Lifecycle Stages

## **INTRODUCTION**

'Lifecycle stages' predictive model targets customers by analyzing event data and purchasing behavior. Through this model, customers are classified into smaller groups, providing significant benefits for segmentation and planning marketing strategies.&#x20;

Customers are divided into two main groups: **Non-buyers** (people who have not yet made a purchase) and **Buyers** (people who have made a purchase).

<figure><img src="../../.gitbook/assets/2024-03-03_11-50-27 (1).png" alt=""><figcaption></figcaption></figure>

In regards to the **Non-buyer group**, the 'Lifecycle stage' model will analyze the level of interaction based on event data such as page views, product views, logins, etc., before allocating the customer to three smaller groups: active prospects, cold prospects, and inactive prospects.

* **Active prospect**: customers with a high level of interaction
* **Cold prospect**: customers with a medium level of interaction
* **Inactive prospect**: customers with a low level of interaction

<figure><img src="../../.gitbook/assets/2024-03-03_12-07-33.png" alt=""><figcaption></figcaption></figure>

***

In terms of **Buyer group**, the predictive model will group these customers into four segments: lapsed buyer, first time buyer, instant first time buyer, repeat buyer, regained buyer according to three metrics that includes **recency**, **transaction order** and **retention**.

<details>

<summary>Recency</summary>

Definition: Recency refers to the duration between the last purchase and the time of calculation by the model. This metric is utilized by the model to recognize the 'lapsed buyer' group.

**Lapsed buyer**: Individuals who have refrained from making a purchase for an extended period.

</details>

<details>

<summary>Transaction order</summary>

Definition: Transaction order represents the count of a customer's orders.

**First time buyer**: customers who make a purchase for the first time.

**Instant first time buyer**: customers  who make a purchase for the first time and agree to provide personal information such as phone number and email.

</details>

<details>

<summary>Retention</summary>

Definition: Retention refers to the duration between a customer's last two orders.

**Repeat buyer**: customers for whom the duration between their last two orders is short.

**Regained buyer**:  customers for whom the duration between their last two orders is long.

</details>

## CREATE A NEW LIFECYCLE STAGES MODEL

### 1. Select Lifecycle stages model

In Predictive model menu, click ![](<../../.gitbook/assets/image (2935).png>)

Afterward, select **Lifecycle Stages** and click **Continue** to generate a new model

<figure><img src="../../.gitbook/assets/2024-09-17_12-02-31 (1).png" alt=""><figcaption></figcaption></figure>

### 2. Prepare data for model's computation

**Lifecycle stages** model will utilize data according to the configurations set in Step 1 to compute results.

* **Data transaction**: select a data object where stores information related to transaction history
* **Where**: this feature allows users to modify the selected data object in the Data transaction by filtering according to its attributes.
* **Customer identity**: choose an attribute used to uniquely identify customers. The model will employ this attribute to calculate the number of customers.
* **Transaction date**: select an attribute that stores the time when a customer makes a purchase.
* **Revenue**: select an attribute that contains transaction values.
* **Time range**: define the duration for which the model will gather data for its calculations. We provide two options: all-time and custom.
* **Engagement event**: select events that you use to evaluate the customer engagement level. We also allow you to configure a duration for event data.
* **Customer register**: select an attribute that determines the time when your system creates a new customer based on the personal information provided by a customer.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfviUkaQZy4v4rOfSQvqK1P9rvZHuV2sFtYS-92O_6V9iiSS3hSU_GxTx7XELVlAI6DRpAMVnasG4n075jnTSjpZznx7wLcw3Y-CV_VY_vXF9qZjEEVTRshJvJweBhHZLQD8YpR8dz-8nyZu2S_69eLztAJ?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

Following, click **Next** to proceed to step 2.

### 3. View result

The **Lifecycle stages** model will automatically compute and display the final result in Step 2. Additionally, we also provide an expert mode that allows experts to modify the model in more detail.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcweDYRZpfEdIGHMUBNocV2fcz2ox26KuJLGAU-UgfeSsSICTjz0uTd9oylLp5q_0b_LgJlgBVODYYPRCX5oFAgFrXhjGBWRlYebaiiryv69zlxz-uk-N5iyeuvhn9z4hdiraz89Iz-NiV2QJA2ku_nFY1B?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

### 4. Apply to build segments

Select groups that you need to create segments. After that, you can use these segments for marketing campaigns.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXekLH9YASMkr7Hz8irriMeHXzutDKBZ0k2KAd-qHr_iK-maX8FFmcvTPxvIX99Cz-DoZcHiaBU-VLJOek914XKckYO5aNMXoCD-Otx0RzgVRi2nWMb07edMkfp3FeZ-e4Rr_9NEmPh4BcZxFUl4rGFyMfbX?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

### 5. Record customer data via Audience movement event

When this event is activated, the model will record customers who transition from one group to another. Data is leveraged for segmentation purposes.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdQbLeaAXCk7LesLfcyIBkSy7oRcsq8D6rNIA0nYQ-eXPekJl1qr0VyIWeyn4TcNUyswPG7nhgSXytf0sF5RdftdOb2Bf96g8c7UBjExBGKOyPIsJ4MGR3UieFffYxCI6BXb13HPugtY0V3U56CpL4AniNx?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>
