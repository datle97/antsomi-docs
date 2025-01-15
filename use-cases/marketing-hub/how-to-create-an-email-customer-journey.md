# How to create an Email Customer Journey?

## Use case:

A number of customers enter the website, viewed products, and added products to their cart but ended the session without purchasing. I want to send an email to remind customers about their carts and encourage customers to complete their transaction

## Steps:&#x20;

1. Hover your mouse over **Marketing**, select **Orchestration**\
   In **Orchestration**, click![](<../../.gitbook/assets/image (1582).png>)to create a journey

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeV6UL8bGzo3lSX2zrtFXk66K9v0nl-wCvp7H8jyqbv2LX2Ed2l7IShD6O5zN7AMhSVgiY4eiATCCxpTusY7jLQG8ohECt_G3S9NWRxUf7TW5uPnRoEJtizlhrjzg-G1aoOQlA4I3AzwDW0dSfLsG0ybOo?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

2\. In the **Orchestration** workspace:

**2.1.** Enter the journey name: Remind Customers about their cart

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcMdERy3N4wmLyZIyz1FjKD1fESuLniy3g_8-b0H1DPmyNms_ZRSzgW1JhBAZr-dyWszmj7Ks8jpbTpXf7GUd4OqDCBD8xkPZ8Aw9znhYKnNkg7A4zlGgfGzH0YHs-ii69aqcbW45xZuDnhqYH_i5cJFRtu?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

**2.2.** Add a trigger and configure the trigger node

* Trigger node: Action-based Trigger
*   Configure the trigger node:

    * Journey schedule:
      * Start date: 07/10/2022 at 03:00 PM
      * Close date: 14/10/2022 at 03:00 PM
      * Trigger time: All time
    * Trigger when visitor:&#x20;
      * Select event: Add to cart
      * In any source of: Websites, App iOS, App Android, App Flyer, Magento TS ENG&#x20;
    * General settings: Unlimited frequency
    * Custom Input: Client - Antsomi



    <figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd3MVpjhv21nGzW4zM90pnYjT-6y3Xniwa6A8T6JgFBzAgGYvRgILo9c-PHSlu1DzJe2qA6DGAVgcpymNlL2sAFBVzn0RZzBTjjVeZATFk4O6xl5BYv_CTrW4vDWZXqS2PI882AViO-wzTuHTiiqUU8Ajkn?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

**2.3.** Add and configure the Action node

* Action node: Wait for event
*   Configure Action node:

    * Trigger when visitor:
      * Select event: Purchase
      * In any source of: Websites, App iOS, App Android, App Flyer, Magento TS ENG
    * Waiting for: 2 hours



    <figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdoFPM3lJca-683Hk58Tt2l1E7ZVfVEzuBy5WmzWaR7leZq0RS29gEHSt9JvXbnubpuiIDmh5bMA5fTRp96tyPtBpwzXP7S2HT0q5L_kOIIc5wffdFN-q1C59n-jXv3iDxlKGKm_vWjPEnRlRz3cAyn-64?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

**2.4.** Add and configure the Destination node at the Waiting timeout branch

* Destination node: Amazon SES
* The design method: Design from Email template
* Configure Destination node:
  * Setting:
    * Campaign Name: Remind Customers about their cart&#x20;
    * Delivery Destination: Amazon SES to Visitors
    * Delivery Algorithm: Randomization
  *   Compose:

      * Variant Name: Remind Customers about their cart&#x20;
      * Subject: You missed something
      * Select template: from Gallary



      <figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc1K1BKRE2yldzrsgUYaqrt1k1tjQkRu_Cqz2qIGer6H6gpM9sHlzUC9mzEy49MUvIeRqVGTRhZQMy6ITZRuG3jvv-JCgxxf6dv8mP1f5Yz0IfrFYc_NfKSKpjKVLll7BXxX6VC9XRzW55TDaPLKqHFUjeq?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

3\. Click **Save** to save the journey

4\. Click **Activate** to run the journey



{% embed url="https://drive.google.com/file/d/1hcWi2gidMM-OVTlAw93e5a_fnxrf6TE2/view?usp=sharing" %}
