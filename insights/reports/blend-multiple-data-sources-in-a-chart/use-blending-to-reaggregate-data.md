---
description: Learn how to work with previously aggregated data.
---

# Use blending to reaggregate data

Reaggregation is a common need in data visualization. This article will help you understand the concept of reaggregation and how to achieve it in Insights using data blending.

One example of reaggregation is calculating the **average of averages**. For example, say you have a table of stock price changes:

| **Sector** | **Ticker** | **Price Change** |
| ---------- | ---------- | ---------------- |
| Tech       | GOOG       | +6               |
| Tech       | AAPL       | +5               |
| Tech       | MSFT       | -3               |
| Tech       | NFLX       | -1               |
| Energy     | E1         | +2               |
| Energy     | E2         | +10              |
| Energy     | E3         | -3               |
| Finance    | F1         | -6               |

The average price change for this data is a simple aggregation.

| **Average of Price Change** |
| --------------------------- |
| **1.25**                    |

To calculate the average price change for every sector, you'd group this table by the _Sector_ dimension.

| **Sector** | **Average of Price Change** |
| ---------- | --------------------------- |
| Tech       | **1.75**                    |
| Energy     | **3**                       |
| Finance    | **-6**                      |

To reaggregate this data, you'd apply another aggregation function, for example, applying average again:

| **Average of Average of Price Change** |
| -------------------------------------- |
| **-0.42**                              |

### **Reaggregation in Insights**

To reaggregate metrics in Insights, use [data blending](broken-reference). Blending lets you work around the fact that previously aggregated fields are set to the AUTO field type. You can't change this field type, nor can you apply another aggregation function to such fields.

For example, to find the average change of stock prices per sector in Insights, you'd create a blend configuration that joins the same data source with itself. Use _Sector_ as the join key, and include the _Average Price Change_ metric in both the left and right data sources, as shown below:

<figure><img src="../../../.gitbook/assets/image (1235).png" alt=""><figcaption><p>Data blending example </p></figcaption></figure>

​![1](https://lh6.ggpht.com/Y1gFfIuXsqvwPm6JZlQbsQvHAWwGUhdfVDrylouYaHbNR9W0X1ti8yKW6LNhoKi5SMIGypNL=w50-h50)_Sector_![2](https://lh5.ggpht.com/s-ZxOC9CQan_v8BIDttLvZFvBjpep--6rAptcvXxsyeBeX6cZnXm8e4BveGGSDOWOOtIK6oO=w50-h50)_Average Price Chang&#x65;_&#x54;his blended data source lets you apply new aggregations on the previously aggregated _Price Change_ field.

**Blending disaggregates data**

Blending data creates a new table from the columns that you select in the blend configuration. Metrics in the new table are treated as unaggregated numbers.Because _Price Change_ is no longer an aggregated metric, you can now apply a new aggregation function on it. The table below shows the results of creating a new metric AVG(_Price Change_) with the previously aggregated numbers:

<figure><img src="../../../.gitbook/assets/image (1082).png" alt=""><figcaption><p>Average price change</p></figcaption></figure>

![Average price change](https://lh3.googleusercontent.com/cq8_5JENQQTmGirfQnbMrjkcf5pM3R6uWUE75yaqhS0cvn2p8GWHdThDcPS9Sp0Dnfc=w1400)

![1](https://lh6.ggpht.com/Y1gFfIuXsqvwPm6JZlQbsQvHAWwGUhdfVDrylouYaHbNR9W0X1ti8yKW6LNhoKi5SMIGypNL=w50-h50) _Price Change_

This new metric reaggregates the numbers **1.75, 3** and **-6** and displays their average: **-0.42** .

### Create a ratio column using blending

Another use for blending is to create ratio metrics with already aggregated numbers. Say you want to create a ratio column that divides one metric by another.

In this example, we'll use two fields; _Clicks_ and _Impressions_, coming from two different data sources.

| **Website**  | **Clicks** |
| ------------ | ---------- |
| google.com   | 300        |
| facebook.com | 400        |
| twitter.com  | 200        |

| **Website**  | **Impressions** |
| ------------ | --------------- |
| google.com   | 2000            |
| facebook.com | 2500            |
| twitter.com  | 2000            |

You can create a ratio column with a calculated field _Clicks/Impressions_ by blending these two data sources.

| **Website**     | **Clicks** | **Impressions** | **Clicks / Impressions** |
| --------------- | ---------- | --------------- | ------------------------ |
| google.com      | 300        | 2000            | 0.15                     |
| facebook.com    | 400        | 2500            | 0.16                     |
| twitter.com     | 200        | 2000            | 0.1                      |
| **Grand Total** | 900        | 6500            | **0.41**                 |

All the rows of _Clicks/Impressions_ have correct information except the summary row which shows the sum of the ratio column **`SUM(`**_**`Clicks / Impressions`**_**`)`**. This happens because _Clicks/Impressions_ is calculated for each row \[0.15, 0.16, 0.1] and then the `SUM` function is applied to it. \[0.15 + 0.16 + 0.1 = 0.41].

The correct result is **900/6500 = 0.14 .**&#x59;ou can do this by calculating the ratio column values using the formula **`SUM(`**_**`Clicks`**_**`) / SUM(`**_**`Impressions`**_**`)`.**

| **Website**     | **Clicks** | **Impressions** | **SUM(Clicks) / SUM(Impressions)** |
| --------------- | ---------- | --------------- | ---------------------------------- |
| google.com      | 300        | 2000            | 0.15                               |
| facebook.com    | 400        | 2500            | 0.16                               |
| twitter.com     | 200        | 2000            | 0.1                                |
| **Grand Total** | 900        | 6500            | **0.14**                           |

In this case, the summary row shows **`SUM( SUM(`**_**`Clicks`**_**`) / SUM(`**_**`Impressions`**_**`) )`. `SUM(`**_**`Clicks`**_**`)`** \[900] is divided by **`SUM(`**_**`Impressions`**_**`)`**\[6500] to give **0.14.** The **`SUM`** function is then applied to it again. The result is still **0.14**.
