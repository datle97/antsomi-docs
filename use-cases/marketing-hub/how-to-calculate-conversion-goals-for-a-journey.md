# How to calculate conversion goals for a journey?

**Use case:** The marketing team is launching a new campaign that offers voucher sales of up to 50% for new customers. Specifically, they will set up a popup to appear on the home page, providing a promotional code when a customer visits the home page for the first time.&#x20;

Additionally, the marketing team wants to calculate the number of new customers who complete an order (using a promotion code) to assess the campaign's effectiveness.

To calculate conversion goals for a journey, follow these steps:

## Step 1: Create a new conversion event

At Convertion Event, click on **Create** to enter the interface for creating a new conversion event

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXegpxn2kBdNciPUglfFjq8BI0Ij4BuvVBVh1Sy-o7sKqdllhhN-szjDwBC-mXihzKREC2jMqqXqk1yFpbSV_BKT4kTnkep6DsQt6WG98pODM63QjUHmfxrDbSIWGE2BNbJ3UVKm92Wqo5qLA_Zxf6fTgZxL?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

Next, enter your desired conversion name in **Customer conversion name** field. It's advisable to use a clear and straightforward name for ease in subsequent steps.

**Description** field is optional, and the system will automatically generate the internal name for your conversion event. Additionally, you have the option to include an icon or image for your event.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdgUiSH18VmMR8XX8GWhI4jGbc1tzJWvM0x2jHUoHBN6duMsbYfxl25Hv_SxjhFXK_f8DEemQIdmPzivzvo7Ke7f5V3WJph7OFHtvO0JaScRg5W0gO9FV7kCp7JtYrXkyE_wn-xnUHjHfynO2MjeywWMzo?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

At **Conversion event** section, because the campaign desires to measure the number of transaction on the website. Thus, **Purchase** event is chosen. Besides, you can also filter this event by removing unnecessary sources or refining by attribute.

To better understand the concept of a **Contribution event**, let's address the question: "Which event leads to the conversion event?".&#x20;

Returning to our use case, the marketing team specifies that a conversion should only be recognized when new customers utilize a promotion code for their orders. Consequently, we've introduced the **Promotion code used** event to categorize orders that do not use a promotion code.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeBm_fFyqibNSXqDktJjvMI2S-77luVSCh5M_T_qHV_uYkHS1fq8RvWSixydJSA4H1EfyAxC2KfDB633vfL7rLmKBG3PL2eAiqAyYzbFanYTwCdNnZc8T9NvA98o9wAdApmlG-eTMfiIpGrJDErJt8ws2GU?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

**Note:** To minimize delays in data processing regarding the **Promotion code used** event, you should select the **Specific** option and configure the time when the conversion event is calculated. To know more details about these fields, [click here.](https://docs.antsomi.com/cdp-365-user-guide-en/data-hub/event-sources/conversion-event)

## Step 2: Create a new column for Journey Performance Table

Access the AM Journey Performance editing interface, then click on **Add source** and choose the **Conversions** source.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeiSoDbxQ76wPuTrJ6i66NW1Io7uNBw51AF1u_ePzXCSQ0gpxHH439j9p7w16nIaAYQYTo22H9eSRCQU5ga3hBsSEQLevwZttQJkGcRGNnffKrAC9DPh9ziK1fQt4kjpmfuqJdgP9cFTbd95FL2_gqhogI?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

Then, to add a new column for Journey Performance table, click on **Event Measure Field**.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcSctq-rWwQ5aDV8bhPfJkHBKhmNXwiQnFwOpYyW83xIIreBdBC8WbrzIUhtltw8LAiPrsEFvGZgJoIaZ8i486oo6Djne0HH3Bsz0MdXybzKIgTHffPrzff84wNjz8BMLeDk3wqK8W6xj2w8zNEtR_yQBEo?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

The system displays popup **Add field**:

* (1): Enter a new field name
* (2): Provide additional information for the new field
* (3): Select a conversion event which user desires to calculate (In this case, it is the Conversion - Offer voucher campaign.)
* (4): To calculate value of conversion event, user selects attribute **Goal Value**
* (5): To calculate total value of conversion event, user selects **Sum** for Measure type field

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdo9ToFwzmKNrbhlYQ2sD2G-WJUkm8H-chmvgmKVGMB7dEBBmafP5HerzKXolFnwW-yx-i9A6uSHuk3WmR8DdPqJ0Nrn9l62v1hZHqqjmTzbd9ofeaO5HUlhe6yBP0jTR03UZmNcJXH_9kCBDkGCjVFg10?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

* (6): CDP 365 allows users to set up a maximum of 2 goals. In this scenario, the new column calculates the total of the first goal. Therefore, users should specify conditions to calculate only for the first goal.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeqRtrSvGYDWkgyGWDKU5tRFp866755Z-aIyztSz2QAHTlOyovxAk5-3DSzhBDIROAzn5sUn1dwPvQPzu5ULrG5Fu7IBiad86SphIxPjJlfOQ1kmtdl4bM7TI9lA-jXlaru6IBmmeAyGcbWd24pN2XMzo0?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

## Step 3: Set up a new Journey

Within Journey goals, choose **Specific conversions to measure** and add the desired conversion event for the journey (Conversion - Offer voucher campaign). Furthermore, users have the option to configure up to 2 goals.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfUAUmHoYLlewYqs0Yg6vRlZ3liYFRIGyBfdZGohP3-cIlbfoGtP3fqg8moq4XdmZELpuNtsjaH9EyTbNjDZ55BalVNqy6tY7Oxvb1gjlx_f8_OsH6cEk-KvimwtJu03bzVWgrCmL2b2eJ2oLZPpLRJb0ct?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

## Step 4: Monitor the number of goals achieved

Once the journey is active, users can monitor the number of achieved conversion goals using the **Goal 1st** column.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXehg0VfSLFZcbbd0bMf6xNxZiIUPkxsGqI3J99DSP0UmXCsbZBrHVnHHLCVeiaPdPq3FNjUtd7pqWljMT7SCFH7ZbJscxVaokUyGosQEp2NJ2saK9j29AFs7jKGVAuWX_DO9kL5Ay1FHKXBKdk9norXhOE?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>
