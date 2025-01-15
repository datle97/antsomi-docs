---
description: >-
  In order to use webhook to engage your audience, please follow the
  instructions below:
---

# How to set up a Webhook Journey

Webhook destination will later be used in Customer Journeys, where you can configure the content and the targeted audience.

## Create Webhook Destination

Webhook destination will later be used in Customer Journeys, where you could configure the content and the targeted audience.&#x20;

Please follow these step:

### 1. Hover your mouse over Setting >> Channel Integration >> Webhook, then click Create button

<figure><img src="../../.gitbook/assets/2024-09-06_10-54-53.gif" alt=""><figcaption></figcaption></figure>

### 2. Choose destination in Destination Catalog

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdYoc782P7i9O_rND1Iz24b_Whz-dLHhGFhrct7j4CeoDzFgjRiHwYtDxGRcMFEbYXEdmcEttvZ7GLQaLJNrtKmhg7UR6Y2VmKmfRCLGPQ-428I27Cl6LF-J_UPVAhbBCqhmJs4oL7RKZgfOFQAeAv4hvkT?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### 3. Input the necessary information of the destination

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcQsq-AbrcfiHmljN-nqU33VAfvEoEPZyM8FGXianl5VeJAYgqCQzS448cXAFSj_TtyCGnWtgYUB2cdCiPZjB16zexUXCye0mIU-v6dmQq6GIodT8arPLEjhMvTGdsjhxY8kiGul9HE2E2d1fWZlJHyDvA?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

**General Information**

<table><thead><tr><th width="225">Field's name</th><th>Description</th></tr></thead><tbody><tr><td>Destination Name</td><td>Name your destination as you want</td></tr><tr><td>Description</td><td>Describe this destination. Usually, it would be the objective of this destination</td></tr><tr><td>Destination Catalog</td><td>Choose a catalog</td></tr><tr><td>Method</td><td>It is "Push" automatically</td></tr></tbody></table>

**Configure fields**

Depending on the selected category, a list of corresponding configuration fields will be displayed.

_**Frequency Capping**_

Frequency Capping settings allows users to limit the times an audiences receiving a marketing message.

<table><thead><tr><th width="262">Option</th><th>Description</th></tr></thead><tbody><tr><td>Ignore duplicate messages for the scheduled journey</td><td>One audience just receive one message in an iteration of journey schedule </td></tr><tr><td>Limit frequency for the journey (3 months duration)</td><td><p>Limit allocation frequency to 1 audience in a journey for 3 months </p><p>(Ex: 2 times/person)</p></td></tr><tr><td>Limit frequency for destination</td><td><p>Limit allocation frequency to 1 audience per unit of time (hour, day, etc.) </p><p>(Ex: 3 times/month, 1 times/day)</p></td></tr></tbody></table>

## Create a Journey using App Notification channel

### 1. Hover your mouse over Marketing >> Orchestration >> Create button >> Create from Scratch

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdkTs8eLdoannjUi2cbUyKy2y_KCOwVIOzKfqm-ZiIG5IgZNozKsUHF8D2z5Me5u630CdJi_topx5Orl0tMhqWMjX42_yWQ9vnbpDWUKbnodozkn_OU4Po5brqIhAm_K8zLptQhtjNA_EkHFN0kNEmxUZI5?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

NOTE: If you want to trigger Journey by Action-based node, choose Journey Orchestration channel instead.

### 2. Configure the trigger node

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfR7PP91B1YVruiyzxnVdIm0qIM_djjwr45eXYdQ5AneJW_GZxc4PK1XYe1vFhLPRENWGhiyy-xrT4hxn1L7U3dUeKo-I0zgnF_fdUbcl7M5YnjnNimb9D5498nYB48stSRPAByZRhLA39WZlHG_i6QsAw?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### 3. Add Webhook destination&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXefGHTZxKn_THCbdH8nxzKLptydQGYJaFcy0_GEM5_slSoUeHQRIh2obgHS_ec9QYkeg-x5DUwffzMpjhFdII5G6lXHUwort5a-nEW1bEDVqbM1RBDSXJw-uIwVUnywL6iuN8Vbjc3yZxTlFLTJLsYGTAy9?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

Choose Design from Scratch

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcyGeNwZyBbUEFzVwAHrVhLEuTRr-fZ2Yv51Fr5pcVL-xzYUdsXSSarcrqZj1f4FGUGWxX9mzHvGNxA9HDbzl2-V4ORZ_TntienSCFLSP3rEmqvsv45kaMeWc7hJ90MiQGQGh8n5oWB6lZg2-PgFAgol6ze?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### 4. Configure and input the content of the app notification

**STEP 1 - Settings**

* Campaign Name: Input the name of your campaign
* Delivery Destination: Choose the destination you have just created above
* Delivery Algorithm: Randomization
* Delivery Hours of the Day: Choose the time this notification will reach your audience

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcqgB6NetiJjKLB_p2EHj_-f7DiYp0_uURR_V-uquNvwsjQj85A3nhYTH6MOvCeb-buM2BTLt0s8G8kIfa9dmBPQqzXf7eAAVKcEvxET39WUWtMtTHAI5L0ziW7gZY2fYWtN35InWuE6GruT6AA35QUszw?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

**STEP 2 - Compose**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc9suhD6TUg32r88V8-6of7wAv4qd_-n5nSpQA3O0d0BVhyKPIhmM-x2VVzcQX3cLl9MBPDewaw85SD32yumDGE47SMpVZ-EomDO8lZdMArRtrS1-xu3UKQZMO94IhShB3lLqZu30Sb0Blt0BBfVfM5tuI?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### 5. Save and Activate the Journey

* Click _Save change_ to save the Journey

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXenmgZxrVRMmUdHT5hwCnZ2EiRcVBomNuRK1sVoNA7J4qSXMjuFhv6S2fxkCQQ6VLiB64zjuCM6BW3cQdcYXSsimhav7OJyK6xFRUWEV5T2o1x1dTQAz2C18NzN1S2SuQ6EL-7rM3R-j97eIAidAeYw6ZLQ?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

* Click **Activate** to start running the Journey
