# How to send messages using OneWay SMS destination?

## STEP 1 - Create One Way destination

### 1. Open Channel Integration

Choose SMS Destination >> Create a new Destination

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfpJd_jBLnOvBu3trtrKEVHdmj0-JDDYCxvv7unAKMc1cilrpwqtykVYewxvwzGiQlhL-kvpv42dw7nzqvOm38HfSqmBGhJnbExUrE9rhtmI42Fz7G6giedjRnB5RYblU_J5R5MuXMgvo5v6W9zVlOJkn2o?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### &#x20;2. Click  ![](<../../.gitbook/assets/image (1435).png>) to create a new Destination

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeAfzOZOyCB0s9b_rLzvWNY2AXTYsS7uZLk4jLrzogFLpOON5UiU5Dg1jWR76lAksXQwkQAkcNobxmo1z7O4H2gGTutwFuApJ1Y9I_7fu1QeHP868w6hdKT8v60-E-j3OLTbNGnK1tEBBS3wmiLh8yNj8ov?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### 3. Choose _SMS_ category

<figure><img src="../../.gitbook/assets/2024-09-09_14-33-41.png" alt=""><figcaption></figcaption></figure>

### 4. Fill the necessary information

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd4JtXJXFmysqwfbw_gruZfpXbhAwIcU4PF0BccU6IlGzqHdMJ7cPWt06MHtI3Kl5qvUTJ4zbbTGmqWojkwHA_jPE04YxCU9GAbLWeJJcjqx-sonIiGYp3lYTxheHe5SgRyaOAbQtxYcUnBTMMd6V5mkMpK?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

_**General information**_

* Destination Name
* Description
* Destination Catalog: Choose My One Way SMS
* Method: Choose Send

_**Configure fields**_

* User Name: Your user name on One Way
* Password: Your password on One Way
* Phone: The receiver's phone number. You can make the receiver's phone number dynamic by clicking  <img src="../../.gitbook/assets/image (1600).png" alt="" data-size="line"> icon. A pop-up will be shown below:

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXe0j7LEC-zEOedDWEhot2JVgq6fQU0_HISNk96ZhpNW2YchDRsaTr60y7PrD9mORn0i7oYBJM8E-_jFDHoxdqSwaWOky2mWF-nywS3U56oKNKuSzEbFGUewh72okBdYzefqIbrgzylWA5r-dZtsnOndfgvy?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

* Base URL: The URL of your account on One Way

#### General Setting

_**Frequency Capping**_

Frequency Capping settings allows users to limit the times an audiences receiving a marketing message.

<table><thead><tr><th width="262">Option</th><th>Description</th></tr></thead><tbody><tr><td>Ignore duplicate messages for the scheduled journey</td><td>One audience just receive one message in an iteration of journey schedule </td></tr><tr><td>Limit frequency for the journey (3 months duration)</td><td><p>Limit allocation frequency to 1 audience in a journey for 3 months </p><p>(Ex: 2 times/person)</p></td></tr><tr><td>Limit frequency for destination</td><td><p>Limit allocation frequency to 1 audience per unit of time (hour, day, etc.) </p><p>(Ex: 3 times/month, 1 times/day)</p></td></tr></tbody></table>

_**Delivered rate**_

Delivered rate setting allows users to limit the number of messages sent per second for a specific Destination.&#x20;

<table><thead><tr><th width="333">Option</th><th>Description</th></tr></thead><tbody><tr><td>As fast as possible</td><td>The maximum number of marketing messages sent per second will depend on the system possibility.</td></tr><tr><td>Limit send rate {x} time(s) per second</td><td><p>The number of marketing messages sent per second will be set by user. </p><p>(Ex: You are creating a destination for G Suite Email, the value you set is 100. That means only 100 emails will be sent per second.)</p></td></tr></tbody></table>

### 5. Click Save to save the Destination



## STEP 2: Create a Customer Journey

### 1. Hover your mouse over Marketing

* Choose **Orchestration**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdLdlIWkgHl826_NOi9VWyDIotUttOyZhYuTmQ774UpykafjlQGAQu92Kl0i9xWDfzcPFUbn88blFfk4bH_d4n6pt0s7FCcjMflNry-ItGBHo08GB597rzKSVicxPvBUWGBaCWECxtjBCtxEdCYYoVJYHav?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

Or Marketing >> SMS

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcOLoFWEDud9Qk67NgHHaITRftJ8NCMCLpMNLpfCaNSlYjHm854q2mISpgpj_L_5axxLVug-3-yfubsHXUlypDzhh4eCWf7MqxnNMMXKRSp8B5B87Lil2rVghgM_8mGAY3-g2NSWhBFyowgY7nLFMFJNFU?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### 2. Click + button to create a new Customer Journey.&#x20;

### Then configure the Trigger Node

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdt-dCYXPBXHU0nzEoOwPCXuvHWtESXw4FRPVQ52yvEa5TPvli80Lfm32c2bgavZLZgcjnJye45ypjKKeGCTEeHDhIFZy5WsLuUKkBbh5fdhriR6RZ9LyJ9bE_SjYoV9cKTROJtdAl4Tc1dT4t-RQX4cC6f?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

**Journey schedule**

_Trigger Journey_

* Once: The journey will run only 1 time
* By hour/day/week/month: The Journey will run hourly/ daily/ weekly/ monthly

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfnFaGjbbZtyzvzIBHtFrEmU3yCHrlYKSKqrr1Bq7yq9SPGE_OnN1GUo6dnYTwqDp2z1XvA79pXbUm8Q-uiVpCnATHV5vN6f5WsabEahlYrSmh-_lfnQB68o4l5ubJhco34ZYVRUSjqEvBqbSzMLan8pJY2?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

_Trigger time -_ The time Journey will start running

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfrXtRxzEUkqCbImr9hUI_In8UuhMlB9BCu-L-50LTk_K2wuhVC675JlG0Dj6sAOztV5PmlE6MynBymqitG0ylYKwsotqiC7SMClkxFgsT4w0i7XzcuvGNazxiIrDllpXMQnb8JZ-axEhdLs3puEUS3RVBo?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

* At a specific date & time: Choose the date and time the journey will start
* Right after the journey activated: The journey will run after you click **Activate**

**Include/ Exclude Audiences**

* Choose the audiences who are able/not able to go to the Journey
* Click ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe7qtnJ_skUvCFC1zGezn3rThbIYXp7cLtkWJVzou-iO5QnwqkxWRDmKlE8w8HkcJfa7Pwx-JjBeYIwPYo0z2DldLSrkOb5RFd-dlM_qjh-9Kp5YbFAsun9N9kj0Q9o_F3o336cH43AH2evGhb3XpXcBNs?key=jqlrLHcQRq84j2mU-bHqrw)or ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdSeJuse1J544mjbLWR3dnGc1_niyb4hj3Mh4o-Z1HtMn99h3RoEW-8lsakkPFNsxYd5yf23fnOXFssfpNhp1w9RONHQzbOGnssmuNClwcoEMEwXGVJmMUhUC6ibGHhGjuHVa0EpCnTUtdW8M6p5Padxhov?key=jqlrLHcQRq84j2mU-bHqrw) to add audiences

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdB9CUQNm-v-psvMtJDA1b-VIU_2GP90J6Tq3njyxLAu0bmJNxvbe_iaahoxflr-sGSMEDNsrbpO79brEdnCYh_QAdj8XP4wyywGLckpC4_bPzihMA-lf9lavU45q4oWx7oeQZwYRadJluNGZrZkQbvRmJ7?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

**General Settings**

Limit the time an audience would receive a ticket

* Unlimited frequency: The audience will receive as many ticket as the journey run
* Limited frequency: The audience will receive {x} ticket per day/week/month/lifetime

### 3. Add Action node (optional)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfvAhtJaOUS-bPotnf4qw3Z2b-x3SHeBhyEuFmZR7LYiVATTMpyv4mFgNPw58y_eWNAdFveCkMj_OGUOIo7NCh8NxJP4_2Y755_5u7en0nU3N52vF5OgLifZKEBmRht5Y-95_DqwgPa74VvqlijSIgXJjWJ?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### 4. Add and configure Destination node

Click + to add Destination node -> Choose **My One Way SMS**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdgXKiiWzOS4bREtb8NjUbSzZOUVs3GHI03M3afmxLwG7_5JrCkaYPaAVSvioGfYzbZegaL-n7tWTTgQNrUXunJ3EGThEirEyylMwRXjV_FFnYZcfUMjuf4AIovPO6i8xAhyLnHTmBNVUiO6Lp6puOqyvAK?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

Choose **Design from scratch**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeH5OHcqU4WNG25-VowiZrkFfm7PGrrsMDoD5yI0_aavOXwAEJRU7jBDOLxKNTVVK3xGAioQyodvNVVa9GcMHtXms7TPsGWHFKmHHyF_wrZ-oFbHTrf9hUvBM82vLZMuCjjYObLgsCcs97aKG0TyT_Hney6?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

Design the campaign:

1. _**Settings**_

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXe6a8n90SzaRcB4vH7xmCbgPWr4u_0HegPPj2g3OEKrjkpNFH0bDouvqJkVQbsuv8Dmlh1J57jW-5uoI4-KM_oHjNULtL5sctRUuN3o4WI8eS0U3iwUBPpQ8QxaEgGUsyqEwFaJdjIRPkX-sQi3kOi_nCwn?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

* Campaign Name
* Delivery Destination: Choose the destination you created in [STEP 1](how-to-send-messages-using-oneway-sms-destination.md#step-1-create-one-way-destination)
* Delivery Algorithm
* Delivery Hours of the Day: Choose the time you want to send the messages

2. _**Compose**_

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd8_8hEmGgOxl7Zy-8idhlckBQQDo_2SqtHEtj7dFKS6BqWvciEuHW-oi2utC2CcsXuv-BD7d98-6_KsuEM1wMx4VL2KD0ewS0fIvOzMDVhbuVsAOievOjmYzQDDIrPTCuhrQKh397AJ5M2nRE51-hBvGNY?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

* Variant Name: The name of the message template
* Content: The content of the message. You could make your content dynamic by clicking ![](<../../.gitbook/assets/image (933).png>) icon

<figure><img src="../../.gitbook/assets/image (2202).png" alt=""><figcaption></figcaption></figure>

### 5. Save and Activate the Journey

* Click **Save** to save the Journey

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcYWwLXhI4SX8B8P5UBlmYux-6Fo9eM-vMxm74b-Gsthk0ZXZQaDSpuKJ0JCGI-2ifoDUGv7pjh8WvRywH_k0EDLFOBevxSRcg0hsZRdhoM0MVNcl3kkzpM3f6k5viiimhBSBnWpV4IUYT_l-efMq9P0Ayw?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

* Click **Activate** to start running the Journey

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdGxHlIbrG3_DzUxcTirYJUIlNeDuSzotYmNQEUer9e5x3SoMG6z1VNTI61hD-Fc8NOAyoablzY5ZannXX92Q-rXbt8sLJPbEvnvI03HRDE8wthfZL7OljMiyr1ZXSLqptCeY3Ifff-e_VOsTiiBxtFL0U?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

