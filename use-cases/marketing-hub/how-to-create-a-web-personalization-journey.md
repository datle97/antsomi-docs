# How to create a Web personalization journey?

## STEP 1: Go to Web personalization

* Hover your mouse over **Marketing** and go to the **Web Personalize** menu

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXehnv9h411dZ5p-4wZW_CfrPAU5GhRKSe8Y8XfFQTU2VPQJZHc5pBj3_gd6a6dJgqXh6dU4aZBGx6rHq67y0AF7ryPvLtwfgAsI6qQvkQSkxzDkSmd81_GM745YKFKaSVr6FpsVV_M7kWhHwQ8WtuD2ZQKw?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

Click![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeNf4zVadwiAHdiwf2LyTOyUUQ94Y66olP0rYmwe0_Nl6iNedhNG9steEko2c-bfLpyU9Yn6BgHofOFYBFp42DhkDiEm6RtehypuDpE7U38ErTPkvV03kE9vteP4e8YlSqdkDhEm2-0DrbEfA-rInuWeWx5?key=jqlrLHcQRq84j2mU-bHqrw) button to create a new journey

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfOq9jfOuIGgY3FQdePuRVQeEY2UvwKdoLTDpXKqqsYGOezaP7uYXihK_ZosqOOJcdrUDmy3ZXdgee4889oqBaBaGOiGN6j0wNqwu5gC6RBEvXjPKg48stqYsOcdCg9I1k0xI1MUuKu6t4uhR6jOPWdJ_Ep?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

* Choose an account you want to be the creator of the journey -> Click **Select**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdIX2mR2iRfIznKCIsza7qdp-fvl7zjPlsrqZCzwt5h-gvuwr37aEbCCrediwAWdzfw1gkmVFVIziv8iLn8WyF0ObyNn6rLTlsVU9TJBntGbhwyOm4s3ILA1-HiI3jl0FBY7b1otzxk67l2ZyNPPOWANxq8?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

## STEP 2: Configure the Journey

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfhXNdju-NCVlYNmSUXArxrll6tbjwIoc6ePpuzANLCUm7X1q_9zMTAruBKNebZ5ojlUkYwJ0XT6z4Ajp6xJar6sF-3e6hfexJmlQvvM340HOIZoKvnZ_VC1m56JpakRgOweZYS2DFQBT8A4oBkyKKYtrw2?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### Trigger node

For Web personalize, the trigger node is always **Action-based** type, meaning the Journey is triggered by the event of audiences.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXctmbVN63c6gDQfoL9wHZez3Dvh2GVBunAGl7OGmMJO6bl8ZDeEMwqXNIGL4Tn6ApqQ8o2MHC4_JSs8g5HNRPdHXIDs9Wno8WpXAO1uJe84Q7vbWNVa5RXg0RCBVYaMFeB2jfFNNu2RRg4xcqE0W7cZqHbz?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

#### Journey Schedule

It's the time running the journey.&#x20;

* Start date: The date and time a journey will start running
* Close date: The date and time a journey will stop running
* Trigger time: The time when the journey stops or allows receiving the audience.&#x20;

&#x20;     -> All time: The journey will always receive audience



&#x20;    \--> Specific days of the week: The journey will only receive audience in a set period of time

&#x20;    For example: The journey displaying a pop-up on a website only from 7:00 AM to 9:00 PM every day during its lifetime. The setting should be <img src="../../.gitbook/assets/image (2250).png" alt="" data-size="line">. If you adjust the time on Everyday, it will automatically apply for all days of the week.

#### Trigger when visitor

Set the conditions of the chosen event that an audience must satisfied.

* Select event: Choose the event you want&#x20;
* In any source of: Choose the domain where the event happened. After selecting an event, CDP 365 will propose a list of sources that have the event.
* Where: Filter the selected event. It could combine many conditions by AND logic

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXepDBRTP1jjXPa7i-FSP8gJ8e-m3Ue-mOVXTGlMwyJch4UnZs7WGwyHR1RK32f2zq7RgszdVL6WkhZydsUmApj9O-2wgYRzlufvux6Krgw2DhKtv-XtGZgRoI5J_o2zoNdM4T-J845VyzrgIX5jSL2KYal4?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

#### _**General settings**_&#x20;

Limit the times an audience enters the journey

* Unlimited frequency: Allow audiences to enter the journey unlimitedly
* Limited frequency: Limit the times an audiences entering the journey&#x20;

For example, a journey aims to show a pop-up for whom view **more than 3 items per hour** and a user could only views the pop-up once during the whole journey. The setting should be <img src="../../.gitbook/assets/image (1463).png" alt="" data-size="line">

### Action node

Allow filtering of the audiences entering a journey that help the journey customize the marketing messages.

As for Web personalization, there are 5 available node:

<table><thead><tr><th width="188">Action node</th><th>Description </th></tr></thead><tbody><tr><td><a href="https://docs.antsomi.com/cdp-365-user-guide-en/marketing-hub/customer-journeys#delay">Delay</a></td><td>The journey continues after a set of time</td></tr><tr><td><a href="https://docs.antsomi.com/cdp-365-user-guide-en/marketing-hub/customer-journeys#if-then-branches">If/Then branches</a></td><td>The journey breaks into branches and an audience enters a branch only </td></tr><tr><td><a href="https://docs.antsomi.com/cdp-365-user-guide-en/marketing-hub/customer-journeys#filter">Filter</a></td><td>Filter the audience being in the journey </td></tr><tr><td><a href="https://docs.antsomi.com/cdp-365-user-guide-en/marketing-hub/customer-journeys#a-b-split">A/B split</a></td><td>Conduct A/B testing </td></tr><tr><td><a href="https://docs.antsomi.com/cdp-365-user-guide-en/marketing-hub/customer-journeys#parallel-filter">Parallel filter</a></td><td>The journey breaks into branches and an audience enters all branches</td></tr></tbody></table>

To add Action node, there are 2 ways:

* Drag and drop the node you want

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXexJG2Fmb5kCxUIR9jhw0GaSUfJRXTkQn-rGvGRYSiCyXkuUrKDOLRc3OjKSnB_-MmYOhW_i9iJD5VNCbjs4sOb1cIdZZexqEiPx26C_5stHYw9ygNbDiX3RBIdNgO_ZD5AYzfTSj-h_d8SO8CFAVhx4qM1?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

* Click and choose the node you want

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcUc2FSrXJOZpDx8TqTnbAzfOBiVGGymy9DZF7R75Qb1mw6N2TOxypQrtNI1JD-hkEGGJuD18YYh2JHPa4AVcn0FLpWJ6HVczpIC-JzRbpa7Qm14ZcBWWJtJDKc0OWb7FwEA5jWtzkT8m1AA45egpDNeQc?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### Destination nodes

It's a marketing output of the journey. As for Web personalization, it's the media that will be displayed in a website (pop-up, banner, floating bar, etc).

1. Add destination node: the action is the same as [Action node](how-to-create-a-web-personalization-journey.md#action-node).
2. Choose the method to design the template

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcfi5dCyX15mC0phh0Hi8KGusZoSzA4j9qAFj-6_5OWDNPqBVzr0eEswYU3vN-I50HUmKYZmNcpwlNE8zFLXpWmWpx-Mw5X7t5rVVYOdCBY8AWHRtQoXPEXADqCEk0vvRWSuZRQnR_ZHqp2VEaAgwFTewiA?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

#### **a. Design From Template**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdisT2QSNbX0udDl58ESJ1i8E9W_vrNdosFQhvRAVZBvj_ZIQduKkyFrghDfNDJQgULiHA_SHkqjoRlnRZ5NMVZ_o_z2VTt7uo45eN2zj6eN1pmt0xuTIzP4UtnyfJsvP5PdXQ2iPD-eqZOlRXgb1pp4FT8?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

* Settings

Campaign Name

Delivery Destination

Delivery Algorithm

Display Ad Zone

Content Placement

Zone's display priority

* Compose

Variant Name

Select template

#### **b. Load existing design**

#### **c. Create from JSON**

## STEP 3: Save and activate the Journey

* Choose **Save** to save the setting of the Journey
* Choose **Activate** to start running the Journey

<figure><img src="../../.gitbook/assets/2024-09-09_16-37-43 (1).png" alt=""><figcaption></figcaption></figure>
