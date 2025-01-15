# Time range

When you using CDP 365, Time range usually appear throughout system features

## Time range

Time range helps you to set filters or set conditions to retrieve data in the desired time period

### Custom

With Custom Time range type, the retrieved data will be fixed according to the period time you choose&#x20;

To select Custom Time range type, proceed following steps:

1. Select Custom
2. Choose start date and end date
3. Click Apply

![](<../.gitbook/assets/image (2383).png>)

{% hint style="info" %}
Note: start and end dates may overlap

For example, you choose a start and end date that are both 14/02/2022. The results will be the data of 14/02/2022
{% endhint %}

### Today

With Time range type is Today, the retrieved data will be the data of the current date

![](<../.gitbook/assets/image (2553).png>)

#### Compare Today and Custom (with the same start and end dates)&#x20;

Date of first calculation: 17/02/2022

* Computation schedule: every 2 days
* Custom Time range: choose the same start and end date on 17/02/2022
* Today Time range: 17/02/2022

Results of recalculation date: 19/02/2022&#x20;

* Custom Time range: It will be the data of 17/02/2022
* Today Time range: It will be the data of 19/02/2022

Therefore, you can find the difference between the 2 types of Time range: Custom is a fixed date, Today is a flexible date. Today's date value is the date of the data recalculation

### Yesterday

With Yesterday Time range type, the retrieved data will be the data of the previous 1 day (calculated based on the current day)

![](<../.gitbook/assets/image (1964).png>)

### This week

With This week Time range type, the retrieved data will be the data of the days of the week (Calculated from the week of the current date)

There are two options for the start of the week, Monday to Today or Sunday to today. It depends on the first day of the week standard of each country that you need to install

{% hint style="info" %}
Note: This week is also a dynamic Time-range type. The value of Today will be the current date
{% endhint %}

![](<../.gitbook/assets/image (2427).png>)

### Last 7 days

With the Last 7 days Time range type, the retrieved data will be the data of the last 7 days (calculated from the current date)

{% hint style="info" %}
Note: Last 7 days Time range type does not include the data of the current date
{% endhint %}

![](<../.gitbook/assets/image (1427).png>)

### Last week

With the Last week Time range type, the retrieved data will be the data of the days of 1 previous week (calculated from the current week)

There are two options for the start of the week, Monday to Sunday or Sunday to Saturday. It depends on the first day of the week standard of each country that you need to install

![](<../.gitbook/assets/image (1706).png>)

### Last 14 days

With the Last 14 days Time range type, the retrieved data will be the data of the last 14 days (calculated from the current date)

{% hint style="info" %}
Note: Last 14 days Time range type does not include the data of the current date
{% endhint %}

![](<../.gitbook/assets/image (727).png>)

### This month

With This month Time range type, the retrieved data will be the data of the days of the month (calculated from the month of the current date)

{% hint style="info" %}
Note: This month Time range type includes the data of the current date
{% endhint %}

![](<../.gitbook/assets/image (2423).png>)

### Last 30 days

With the Last 30 days Time range type, the retrieved data will be the data of the last 30 days (calculated from the current date)

{% hint style="info" %}
Note: Last 30 days Time range type does not include the data of the current date
{% endhint %}

![](<../.gitbook/assets/image (1117).png>)

### Last month

With the Last month Time range type, the retrieved data will be the data of the previous 1 month (calculated from the month of the current month)

![](<../.gitbook/assets/image (2130).png>)

### This quarter

With This quarter Time range type, the retrieved data will be the data of this quarter (calculated from the quarter of the current date)

![](<../.gitbook/assets/image (1840).png>)

### Last quarter

With the Last quarter Time range type, the retrieved data will be the previous 1 quarter calculated from the quarter of the current date

![](<../.gitbook/assets/image (1874).png>)

### All-time

With the All time Time range type, the retrieved data will be the whole period time of data

![](<../.gitbook/assets/image (1263).png>)

### Up to today

With Up to today Time range type, the data is retrieved from the current date back to  the number of days (you have to enter the number) calculated form the current date&#x20;

Example: You set the Computation Schedule on 18/02/2022 with the condition is 9 day(s), up to today&#x20;

Thus, the collected data process starts on 10/02/2022

![](<../.gitbook/assets/image (1241).png>)

### Up to yesterday

With the Up to yesterday Time range type, the data is retrieved from the previous date of Today back to the number of days (You have to enter the number) calculated from the current day

Example: You set the Computation Schedule on 18/02/2022 with the condition is 10 day(s), up to yesterday&#x20;

Thus, the collected data process starts on 08/02/2022 to 17/02/2022

![](<../.gitbook/assets/image (2049).png>)
