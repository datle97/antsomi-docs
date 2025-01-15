---
description: >-
  If you're seeking a solution to eliminate duplicated product recommendations
  within the same category, this document can provide valuable assistance.
---

# How to recommend products using the Parent-Child Algorithm

## Why does it happen?

When utilizing algorithms to recommend products **based on customer interactions** such as viewing products or adding them to the cart, the recommendations include products **without considering** specific attributes like **size or color** that the customers may have interacted with.

This situation can result in an experience that seems generic and potentially frustrating for your customers.

<figure><img src="../../.gitbook/assets/image (2756).png" alt=""><figcaption><p>Duplication of the recommended products</p></figcaption></figure>

## How to solve it?

CDP 365 offers a feature that enables you to provide **product recommendations based on either Parent or Child data**.

This feature limits the recommended products to **either parent or child items exclusively**, and it removes any instances of duplicated parent and child products.

To differentiate between Parent and Child data, please navigate to the [Parent and Child data ](how-to-recommend-products-using-the-parent-child-algorithm.md#parent-and-child-data)section.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd-uSRheMWKJFC4VRaxj8DkdNp_eJ5UX0OQ6aw26RBfuu--Ywzy37FvMU8jx-ssGZAOONt8G4Dim83yxt1AFYY4kMey1DhImEv8K1sYHH8-f9uqdYd1Y73CfNx7U9r21PJQsAWLAxlPo5tDsRHNY3vZoTHw?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### Parent and Child data

Within CDP 365, we have labeled the **child products** using the **existing** values of the **Parent Item ID** attribute. If the Parent Item ID attribute has **non-existing values**, then those values correspond to the **parent products**.

Therefore, kindly proceed to your **Product** Business Object and access the attribute to view its associated data.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeBwgX88OE4wf4DfNtWbceaBNDHTETOKZ-tzi3Z4QHiH8-JGQUD2PXUcOWZuwco-fe8LUxWCXqZwtRd06Rv2-AS_6PWxpMDGPtXy8To3T-Hl5Re4UiJuC3_TPO22BluLsdvwIYIf16K-37-adeDtSbI-Ac?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

Once you identify whether a product is categorized as a child or parent, you can then **determine which product level** to recommend to your audience.

* **Step 1**: Go to the settings of the **Product Business Object**.&#x20;
* **Step 2**: Activate the **Parent-Child relationship** feature, enabling you to recommend products based on different product levels.&#x20;
* **Step 3**: Choose and configure the specific levels that you want to enable in the template settings.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeoJ64PS9hYJuM1VdZgW_PuFKznIhH4yeFzcBQIXQ0eXR9Gqswptw8qb6SilNGf22yA_PZjtFXbo_QbFE1v3v0fPnjUn67tG3cLrpCsTFi2mJqB2Iuqkob5EHNreQ-fFuMAaQp3lnuryNJEc-zn1CiDvIKY?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

You have the choice of three levels:

1. **Parent**
2. **Child**
3. **Parent and Child**

Depending on your selection, the relevant product level will become available for you to choose in the template settings.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcstz_yv685wceToUq_GJja4HX7f856efxLhV7-D8RMPsBYwYxGVbBFTEpmOAELBltpgNsG9TnEWgkL0gh2Uzt0HTEugto6walt_GcIJOd_14lXBlA8AbvnGpSZU3g5nayYI2MrJwt-VIivEnxLqjQoopQ?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### In your template

In your template, you can now **opt for the specific product level** to which you want to recommend products.

Here's how to do it:

* **Step 1**: Access the general **Settings** and proceed to the **Basic** tab.&#x20;
* **Step 2**: Within the **Content Sources** section.&#x20;
* **Step 3**: Choose the **Product source**&#x20;
* **Step 4**: Confirm your selection to complete the process.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfxgs-Fi787lk1-wi3IaVtlbMQJjo7nGGlMrG6kQO1sSnlz7u2AcP77SHOm8vffAWfEz3Bf1m5yubG8tExWHHsHVETBVki9mNGMm02c7-K95B3cLV4Cqqr3qg30IOeb0FpAn0N4KtMXakVWX86ephdDDxU?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>
