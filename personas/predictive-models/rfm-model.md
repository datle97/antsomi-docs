---
description: >-
  This document provides instructions on building an RFM model and exploring
  customer data transitions within the model.
---

# RFM Model

## **INTRODUCTION**

RFM segmentation categorizes customers based on their **purchasing behavior** using three elements:&#x20;

* Recency (**R**) measures **the time** since the last purchase.
* Frequency (**F**) tracks **the number** of purchases.
* Monetary (**M**) indicates **the value** of purchases.&#x20;

These elements help businesses understand customer engagement, financial health, marketing effectiveness, and brand perception.

## CREATE A NEW RFM MODEL

The RFM model creation enables you to&#x20;

1. [**Choose data inputs**](rfm-model.md#step-2-choose-the-data-inputs).
2. [**Customize element scoring**.](rfm-model.md#step-3-train-model)
3. [**Create segment customers** based on their RFM scores and Schedule the mode](rfm-model.md#step-4-create-segments-and-schedule-the-mode).

### Step 1: Select the RFM model

To build an RFM model, access the **Models** menu section in **Profiles**.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd0rwu0oxNgqO6X9iZPZiKfeqVUW-AwrTqKClF6drpoAVSW0KMzmmIY2aggBGhDwCuTIyUMsEzYuwmmyDWKFslGhgMu-7Q6Irr7XVOYa-oGTRXAqADYJY9UpY1STiRvmo0lZNS3a3PItcmI4eYVz9dhYRal?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

In the Models tab, click the <img src="../../.gitbook/assets/image (364).png" alt="" data-size="line"> button.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXduLkN4NpQbyDdbiqM0eNShVGN7TVQycUPdVf5sEgUaXgTtEd0UcwCQWZxiZY-MU1kxJ-pTN3Sp9u7SDgatny31Uh_CYPWhOLEOt6wO3Vf9PFkpfGnSeaW9T8mnqDsOFAJdaUug66t1XvqWMk0D-VEFjcw?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

Choose **RFM Model** from the list of available models and click **Continue**.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdY7mcd5xKuGBz1GggoeJbDd9JWDIfawbiJ6owR-p4entIcZnKz6bzlbUxHYUbg0D_KpfLHz4a1gE33WFR_-KR_iTxFxtZddYAhyvSIQDaUzpHHyY3oa7QCe0Z-PsJ-4wmkpT4s4H-ezAK_MafNimitY4qI?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

### Step 2: Choose the data inputs

To complete the creation process, you must set up **three sequential steps** one after another.

During Step 1, which is the **Prepare Data** stage, you will configure the Data Inputs, which include the general information of the model such as its **Name** and **Description**. Additionally, you will set up the Data Inputs, specifying the [**Data Source**](rfm-model.md#there-are-two-rfm-data-source-types) and its [**attributes**](rfm-model.md#the-attributes-of-data-source).

_**Notes**: Before advancing to Step 2, it is necessary to configure all the elements successfully._

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd9GqYHQFnFuH5de9ppIE52vogrD1y2u3PttnhBMjOEyiiE4HRtcRL87hAB352Qk-jf_dvmkU-cBXCJsudQ7OLsND204m5WsL3acnvgofECOGWKXa-9BzVjousKVr_zc3cz_ltSyaJcHDD3HVAe7A_xrK2C?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

#### There are two RFM Data Source types:

The setting you are referring to determines the source of data inputs for the RFM model. The data can stream from either **Event** (1) or **Data Object** (2).

1. **Event** refers to the purchase event or the transaction event.
2. **Data Object** represents structured data entities in your Purchase Business Object or your Transaction Business Object.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeznc_AM2ij0nsjdsQNSazhY2Th4W5dtpxknzxCk4--4XFUzaRWA5Dn9f_EZA3BKZf9EIrwtXre82GNjAvDSA1BfTbFsDyM3K53I93Z9TNg3n6bBGYtg_O28X3Tbx-Rmjle-8UVP11MEdzBjIgwG3aqrnrj?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

By choosing between Events or Data Objects as the data source, you specify where the RFM model will gather the necessary information to perform the segmentation and analysis of customer behavior.

_**Note**: If you choose **Event** as your Data Source, you must select the appropriate **event source** accordingly._

<figure><img src="../../.gitbook/assets/image (374).png" alt=""><figcaption><p>In any source of (Event Source)</p></figcaption></figure>

#### Where

If you wish to build an RFM model while focusing on **specific purchase behavior** within a particular category, the **WHERE** clause can assist you in **filtering and narrowing down the data accordingly**.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeMLFiKZSLX2V7gQcqtPuTuI4bcwBecQDIv6qS0vwc5TF0X6WBPMh-MYu7SbwRDaWq-ciSe-Zs2hzgR3US8KchvWJ3UcaxeiJ8sHhsmWhfJ8oNcZQE2-s-Gi64M-ddj05UckqW4WRymJzMNFd_gL5574DbX?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

#### The attributes of data source

When setting up an RFM model, you must select four attributes (1 to 4) and define the Time range (5).

1. **Customer Identify**: The attribute that defines the **subjects** who will **receive** the **RFM scores**.
2. **Date:** This attribute is used to calculate the time since the last purchase (**Recency** score).&#x20;
3. **Order**: This attribute provides the necessary data to calculate the customer's purchase frequency (**Frequency** score).&#x20;
4. **Revenue**: This attribute provides the data needed to calculate the customer's purchase value (**Monetary** score).
5. **Time Range**: This refers to the period during which the data attribute occurred.

<figure><img src="../../.gitbook/assets/image (376).png" alt=""><figcaption><p>Attributes and Time range</p></figcaption></figure>

### Step 3: Train Model

In this step, you will pay attention to 3 parts:

1. **Model matrix:** Establishing the structure of the RFM model.
2. [**Scoring**](rfm-model.md#recency-scoring)**:** Assigning scores to Recency, Frequency, and Monetary. [**Create RFM segments**](rfm-model.md#rfm-personas) (RFM Personas) - Categorizing cstomers based on their RFM scores.
3. **Adjust element scores:** Fine-tuning the scores of each element as needed.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcBUQAn-nKBjznTmrVQ90e1E_Rq92yieKaJx50577H_7Q8Y4wXUl0eWHqeO0ioPP7BhCPIXvMQE03DGq96grPzxuxmS1akossj_cICc609wcyFG2hnBbJYlC7jskMI70B1w_cMOMJ00GwAMaK61Gub6EbPC?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

#### **Recency Scoring**

* **Granularity** refers to arranging the Recency attribute according to different **time periods**, such as Day, Week, Month, or Year.
* The **bar chart** allows for easy adjustment of the scoring.
* The **scorecard** grades the scoring adjustments made in the bar chart by showing the number of customers (by percentage) in each category.
* The **pie chart** illustrates the percentage of customers in each category as depicted in the scorecard.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcfP9i9WU9mrLxsNQx_5W0mzjCvAGTqNHEo_AP9-lmwYL21TOlM2BirRMmE1uWpryW9GqSTnFDnAy44b6tQxJevGbw_ZKIqoPD_1-10WkXo7nsDevLVyLKTO-XGBXqcuTrQ7LaHeBHEzaijtxP4mzb7CVG3?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

_**Notes: Frequency Scoring and Monetary Scoring**_

_The other elements have similar charts and functions as the Recency Scoring._

#### **RFM Personas**

RFM Personas are automatically loaded based on the scores assigned to Recency, Frequency, and Monetary attributes.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeTaAaTa5cfAFbTELnDV7Rhrdbd-Gc7ztMA1jGl1TqblS3Oqdk7DrGOOCvVPBbWW0fgQljTC-0-85QGxzt0BVpjljnZMzKhWGbzJYM6XemKJnRYBWReQAXCJWZOnSnlhAakT2hZdUpSE04PftTKA00BCxC2?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

If you wish to edit the RFM Personas, you can hover a Persona and click the **EDIT** button.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXf0tuse3PxxBamSKSSFxxc2EgpbyuNY1w9PWcem6PCGFnQqXAhRycuA48q6iwHqi-APOAarJgP5L23LO7mDNBZjy1EBMQdR9gE29mLclSOo3LVz8BpGBN068iC-V3JAnPxkkz0nMJBIfO14dd5txKG-tuGV?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

The RFM Personas Configuration has 3 parts

1. **Personas**: A list of labels for RFM Personas.&#x20;
2. **Score**: A list of RFM scores for each Persona.&#x20;
3. **Customer Count**: The number of customers belonging to each RFM Persona.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdVka2Y1k3N_ksl_GNBioHo4n4gcYJxcEPWgty1VyhgJddypWvXtXzmLvHDNC1OKfsgfvKA3NUMbr4Hb9REf1AzTFpphgLT6LGcLfRodl4riheb6Nu2pUQDCGWCegiuMbWf0HXKtgR_Z2_GnQcGTxYjjLro?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

### Step 4: Create Segments and Schedule the mode

There are two parts in Step 3 - Schedule & Update that you should pay attention to

1.  **Data updated to Segments**

    * **Create New Segments**: Customers belonging to RFM Personas will be added to a new segment.
    * **Update Existing Segments**: Customers belonging to RFM Personas will be added to an existing segment.
    * **Delete**: Customers belonging to RFM Personas will not be added to any segment in CDP 365.

    _**Note**: During the next computation time, the customer data will be added to the segments that have been selected in this settings._
2. **Computation Schedule**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcKj4pSWV318zwzxiidnpb0GtoVGxCnFGvJ_bVhQiZjZPOZJ9gG6YIBBAl1Sm2RfqhLN7yh6Zx-gp6bbKoJpSs8Qr30S2H6SuQ0M4vDXXRC-t8lpekGup7PKd3fIEothTQ24dwzEL-mY1ec82rosnpsNjuB?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

### Step 5: Save your RFM Model

In Step 3, you can:

1. Click the **Back** button (1) to review your previous settings.
2. Click **Save** (2) to initiate the computation process of your model as per the scheduled time.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeOOVsd-sHdqmk_Bg0_n-t3GzSLbDJrpvatrEjrEp8KaeyMpQN_uW8R3-k0kSIDtBbYzOlQns3JoIetGA-xTGHaTZ1skfZfUhzAI3tVaa7a1MwjF9ojQpaDO-RybAX3UlvTv9JKPUA15ksGKlHiMaiFRUm2?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

## CHECK YOUR RFM MODEL

Once you have created your RFM Model, go to the Predictive Models tab, you will find the list of newly created RFM models in that location.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeEFSB0E9CfYKKmKQ0mi3vyd5jrAqHwRJYW8XUswH7R49fVef4tFehn4c5gnD3MH2AgHLd1YFdQJBNT5efTdDrPM-yDyFw8O7LDjsELbXJFS9eT2p2CZQlP518-t2Z8jPoOqmdMLJI2zirgPNbcMl3hLSKy?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

To **change the model status** or **make a copy of the model**, please select the desired model by **checking the box** next to it and then click the **Action** button.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd2uIFHBKtCIGA4U-V380FC7ms8j7ZZ8Erh_t3N_8UbZCBwRmbzCI48YzBmSVnOiJr4O22WcBjTMkYVLUYh1M5GlvwYbkjjrAAVcFp_pPe_BdzivwTwL5ParJQv8Pk16ma0aBPJfn71xG2l5lMZ7RnpfFBg?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

#### Check the RFM Model setting and its computation history

Once you select the desired model, you can access its settings (Configure tab), computation histories (Computation Histories), and version history.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfZUpAJEaOpQST1_tMXEKttNcO14UIyi2K1ulKOuE8bXP9ZMaDX5rGQmpTmNM3coxbv3bL3lhW7fDHU3N8SPab5-6q7GGK0eWyuLMz5Se4x_aeRsLX5BY9WmR3FF-T1DHPIswmj2-05sIk7AyUMnCd6WX_g?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

## EXPLORATION

The feature allows users to dive deeper, gaining more valuable insights after successfully creating a new RFM Model.&#x20;

* First and foremost, users have the ability to compare the five latest training versions (computation versions)
* Secondly, the clear movement of customers between RFM personas is also displayed
* Moreover, this feature empowers users to analyze vital metrics such as Recency, Frequency, and Monetary

Let's embark on an exciting exploration with the following steps:

### Open the Explore Popup

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeWp-GUtuDrCmUYSVJexJVGAc2cyKl6UcOfzd5Y5JITh8timPaDc7oqAV9mPcFOSkScMQAWg1XeYCBoFMs3VYmJs5F6O6yz02TXFwWPXJjyzi0mKMzNPhickD6iYo8nYkkMYja0tD_xQ6O_gdl7xS3CcQc?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

At the predictive model list, users hover over a predictive model and click ![](<../../.gitbook/assets/image (2617).png>) to open the explore popup.

### Take a moment to immerse yourself in the array of captivating features available on the user interface

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfZfyPQ_vtEHa7qWXJElGoaH932Advl_zYjQMZ-eFYXiNdybGvHHGN2gkQiCO49p2NWXywQtWL92Nstyfh_fxBK8FpFGX3H-hmjeM0TjxGHgD_p3rmQUG1BeAVG0pw3Q39xyIU70BxjJ0QKNerL3KTP9dWN?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

* (1): The interface consists of five tabs, each presenting unique insights through a variety of featured charts
* (2): Access the settings to create customized charts
* (3): To apply these settings in (2), users will utilize materials such as training versions, dimensions, and metrics
* (4): The final result will be displayed based on the applied settings

**Note:** We created sample tabs, making it incredibly user-friendly for anyone unsure about selecting appropriate dimensions and metrics for creating meaningful charts.

### Begin with the first tab - RFM Model

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXft_hZaDZgod9xRvpo0RkMYsm_hjzrQV8HJKYoQoRjOQCjwmFULaT13yUlprtYe_gOtVFbP8lERbrbgc4tRqoVpdyYqttRIBUdFzNDvZkzK6zasdPZKf232gVs-ftNcaCBJ_FYHAYxHh_ujABKU70vBgWo?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

In this tab, you can explore RFM personas, which represent the results obtained after creating a new RFM Model, presented in two visually engaging forms: treemap and bar chart. When you hover over these charts, you gain access to more detailed information.&#x20;

Please note that the Available Fields area supports only the five latest computation versions and provides support to compare for just two training versions.&#x20;

On the other hand, you have the flexibility to use distinct dimensions and metrics to create desired charts.

### Proceed to the second tab - User Transition

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXck8qRvRN7lgpcCRY8afZZDDQXV1TQgVv3Cw-YHATj0Kjhnr3MUl_oY6xk1DWBQ_Uxg6tbz7Irgi7LlNK1fmyQX349QFeCB-aLFgChRrJPwiEQraHtO7EG82KATWHYNkltOQueQUExnEeKjwM6lb8-iJTI?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

Unlike the first tab, the user transition tab showcases the movement of customers across RFM personas between two training versions. You can easily observe this movement by hovering over the lines in the diagram. Furthermore, for accessing more detailed data, you can utilize the data table.

### Next, delve into the Recency tab

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcfbTJWWpXj9yfxppP2RshdZTt1qxP44akGVWZMyqDmYAQwzabLJv5PcCw6xLoLim2K347ukYywOFYD9HqYkxUO___aD82DBc5D_9upcTIVKsmKIY7VeP3v37rMW-phv3jeod0GayFZlCwwxdBzcCxy1zo?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

The recency metric is visualized using both a tree map and a bar chart, making this tab quite similar to the RFM Model tab. However, there is a notable difference here: the **Recency label** dimension is employed to represent the five levels of the recency metric, ranging from very low to very high.&#x20;

Similarly, we utilize the **Frequency label** and **Monetary label** for the Frequency and Monetary tabs, respectively.

### Create new tabs

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXe-WC9XG0EZHbggi_7LYOo1a40WW9OQ0m5SZKmXm1hvanhR745oebXHcCbj9UH8E4VcY_GIqjpqQKCJR9k5KzTTXZ50G_mkfMmM4p9x1gV9F40O8tbgh_xVWt-VboDlexS-DeTgX-8hKeeVsusgDVkmJbHq?key=nsg4PmgvSxrd7fjFkMggfQ" alt=""><figcaption></figcaption></figure>

We allow users to create up to a maximum of 10 tabs, so you can completely customize your own set of tabs. Click ![](<../../.gitbook/assets/image (2621).png>), then choose one of the two options - **Free form** or **User Transition** - to create a new tab.
