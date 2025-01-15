# How to create Customer Journey?

&#x20;1\. Log into the **CDP 365** system.

&#x20;2\. Hover your mouse over **Marketing** -> **Web Personalize**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeY7byLHpc2D3h2Jrh-4B3zSw-Ab6Gwbn1BCDl_BxEaADoWhPUpNdhqBIQPeYm5iaH3YZYOT-l5CiQqFM1tjo-zO7-3gqrEjf1JlmkYURF3ypN0VG3VKAGPoWbkMiaBSfb7HBsqNK9G7GUmlyjcZQ_1_ep5?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

&#x20;3\. Click **+** button

<figure><img src="../../.gitbook/assets/image (3555).png" alt=""><figcaption></figcaption></figure>

&#x20;4\. Select account and click **Select** button

5\. Add **triggers** node

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfQNLkXS0_5OEy4xNcNAmE7j5c3dUxKQ3_xcCI7s8I9D3q9EwfSO7v4CMnfWOPglFj1GsodJMhEznOwXCNP9oDMhiHZCEcoAVjAv6NdBNhYeDMVS87QeNUleTJm6sLfZvmXs3wJA12LetJW9iZ4QHJED9ur?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

&#x20;   5.1. Add **triggers** node - **Action-based Triggers**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdwNiWw-11xITK7lC5fy3Uv2WkzR8uKZqAorNGFxqeOVWBdV9DNcEknjDVCVxVTjdX7v6YbnJ48H4J5P5TdVsv7f8LcycN1utD-PjHN2NtLZYoqL_6rEkkDYcKir3J-yhQJ_MXhDiWbgPvt7XdptQ6a1z4?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

&#x20;     Description:&#x20;

&#x20;        1\. **Schedule**: User needs to declare the start and end time (date & time) of the story. Set trigger frequency, interval between triggers, story start date and story stop date.&#x20;

&#x20;        2\. **Trigger when visitor**: In the Action-based node, the user sets up the trigger story condition based on the visitor's event, specifically: select the trigger event, select the sources to use, and add the advanced condition of that event.&#x20;

&#x20;        3\. **General settings**: Allows the user to set more rules for when the story is run&#x20;

&#x20;             \- Let's say a story triggers when a visitor adds product to cart, and has a frequency capping of 2 times per week; A user A makes 3 add product to cart in 1 week. Then, only the first 2 times when adding product to cart, person A becomes a valid targeted audience and is included in the story to execute the next actions, but the third time, the story will skip A.&#x20;

&#x20;             \- If you do not want to limit the number of times to trigger the story to 1 user, the user selects the option Unlimited frequency&#x20;

&#x20;             \- When the user chooses the Limited Frequency option, it is necessary to declare the number of triggers in the range \[1-100], and select the time interval between the times of applying this setting, specifically \[day, week, month, year]

&#x20;   5.2. Or add **Triggers** node - **Scheduled Trigger**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXf-Kpvxydi5mWmD8aVb_KiYk_FbxOcGZPeMbm-qlnAPMYJAOULYM1bcm3WjoGq2rYPzDQpnxvRvKvHdOWnmuUoApLwThXLaWQdDyW2D8NWd9kULWjuRbXcev5BQoRD3RVEdKZAmPtphFKa5iptOTiybo54?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

&#x20;     Description:

&#x20;        1\. **Schedule**: User needs to declare the start and end time (date & time) of the story. Set trigger frequency, interval between triggers, story start date and story stop date.&#x20;

&#x20;        2\. **Included audiences**: The user can expand the list of target audiences based on the remaining options of the same selected audience-type group.

&#x20;        3\. General settings: Similar to **Action-based Triggers**

&#x20;6\. Add **Actions** or **Destinations**

&#x20;   6.1. Drag & drop node in workspace

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcDbviSceN0rHphivpncIHujbNkINzaM7zBH3y92I7PybOcr_OUW4tL6kc3Vt92D3CAnHN4EzH3Pfn4CiYnXBdEPM8H32deaSvW92-j_xejiN0d63sGuH331P6kRrnWujLnG0lIAcn_L6qAVz5W4kqUjRqA?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

&#x20;   6.2. Add nodes directly

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcsVGkjxaJdCzmz3nNYIeaz2GwJh77z2BlkuXO-IUWxRdNz2Z15_EYssmekyTpRliLKVyRZh3vFies9pkNWmkSkXhWVqbq4AxhFS_OrDuqNwbjCidBgq80O1dtvtfp-ZhRlMS73rCXAI0GHT1VET8t_lr3y?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

&#x20;7\. Fill destinations info

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdO5b1eJsZ9GocXPcsJ9OfKyby7Dq9E1X-MDZ-aKAzLzi1zfEk-kpPcnkkm-VZTAXbW4T1Z78mnbM1MKciunysHt7FtrD1-wQPDKbRvvFc26OGNx7TFtR1q-vFU_5fVSZXizmX1SPZXOJc2O8gxiIZczXBC?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

&#x20;   7.1. In step compose choose template and click button select this template

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeZMxChRd_EOpoqBjTf9wfZTQhATZQF8_967Tp9a-eF8tNoKy-4FkLjQtN_LDvx5lyzbYqRd_26LMQjNSNWPy9LfZvJWdc8dTEIF20Db1JOybvz67ztI-Dm4wzIWQeAuWNeU0WrlpUK94V1EXXuzzzKf-PD?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

&#x20;8\. Click button **Save**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXe--Oc-L0cR77H1wViYkZbzihdWJNT2grTroUZ8GGPGcN5_otc5L5JAOPMma-wx8H109DlGg9qIs6cCx8MVbUsvETxy7ZMs8fEoiK2L9Fj9Qgv8RX9pIxh-TmiT1dM8NS1pmCuzQLr4YxlH_EmD541w5VI?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

&#x20;9\. Click button **Activate** to run campaign

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfNqzwvUMV5ILkFdvYKvkOW1VbwoTlo3zpH-OQzeXGyiIrUUtlep60OxlrjMEzQOuNsq2BpFgV_U0_eo9RpqOpAL2M6CUoxmThcJymHs68Av3NCt19g6qY-Vq6wEf-zKSet440-ToAySIo7-d8MxG8EMDWa?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

&#x20;**In addition to the above actions and destinations, there are also the following categories**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfo8-kkqd0RLIDI72rK4TeZGJ1zGtxC3C2Rd8r_RGRBqLA7_2OXMbGThJHQUJvNe3IBC72NnbpXBFWN05rSBkx_bGgYVohkVTD4VmDENx0ey3cR5UeJqYpVf5kOSDGRM8dKQmBn5P418-vyQuiSAYR_tVXR?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="100">No</th><th width="222">Action</th><th>Description</th></tr></thead><tbody><tr><td>1</td><td>Delay</td><td>After an audience enters the delayed node, this audience will be kept at this node until a specific time is released and moved to the next node.</td></tr><tr><td>2</td><td>If/then branches</td><td><p>Node If/then branch allows users to create conditional branches.</p><ul><li>Includes 1 main node, and control nodes</li><li>Branch No is executed when an audience does not meet all of the above Else if conditions</li></ul></td></tr><tr><td>3</td><td>Filter</td><td>The filter node will check the condition when an audience enters this node, if the audience meets the conditions, they will move to the next node, otherwise the audience will be removed from the story.</td></tr><tr><td>4</td><td>A/B Split</td><td><strong>Allows distribution of this n</strong>ode's input audience into branches by percentage.</td></tr><tr><td>5</td><td>Wait for event</td><td>Used to wait for the audience to execute an expected event before deciding which branch of the journey paths the audience will move on.</td></tr><tr><td>6</td><td>Update segment</td><td><p>Allows the journey to interact with a static segment through one of the following two behaviors: </p><p>  - Ask the segment to remove a specific audience from the segment's members list </p><p>  - Ask the segment to add a specific audience to that segment's members list</p><p>  - Example1: User sets up an action-based journey A automatically shows the popup "Register now - receive gifts" on the sales website, when a new user is identified to view the website. </p><p>At this time, if journey A records a user who has completed the registration operation → the Update segment node of the journey will automatically add this user to the “Registered users” segment set.</p></td></tr><tr><td>7</td><td>Update Info</td><td>Update info for customer or visitor</td></tr></tbody></table>

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc3gAKIwzHBINHyiZwjzj3E2Yv4RpLlA5sE0dgDXq9gEbMkLrYs2qNOKCms_hwxWuOgNscjCeNviXXpHIv0UcQhN9QcSil64MrL6-xDwbjzFrazNbBWeIwAketj_1gUqSzxsAWxyfIeGc69DQkqgzSayNM?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="100">No</th><th width="271">Destination</th><th>Description</th></tr></thead><tbody><tr><td>1</td><td>SendGrid</td><td>Sending email via SendGrid</td></tr><tr><td>2</td><td>Amazon SES</td><td>Sending email via Amazon SES</td></tr><tr><td>3</td><td>SMS Yondu</td><td>Sending SMS via Yondu</td></tr><tr><td>4</td><td>CMS API Davi</td><td>Push message for app</td></tr><tr><td>5</td><td>Viber Yondu</td><td>Sending viber message via Yondu</td></tr><tr><td>6</td><td>Salesforce Email</td><td>Sending email via Salesforce</td></tr></tbody></table>

