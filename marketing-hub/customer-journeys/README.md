# Customer Journeys

[ Read more about the role of Customer Journeys in CDP operations](../../#data-activation-omnichannel-marketing)

## I - Introduction

Customer Journeys app helps you implement marketing scenarios and manage the performance of those campaigns.

<figure><img src="../../.gitbook/assets/image (4130).png" alt=""><figcaption></figcaption></figure>

&#x20;The app includes:

1. A left panel showing the list of available [channels](./#channels) you could use
2. A workspace include 3 tabs:
   * Journeys: Manage the marketing automation journeys

<figure><img src="../../.gitbook/assets/image (4131).png" alt=""><figcaption></figcaption></figure>

* Campaigns: Manages campaigns (channels) used to distribute marketing messages

<figure><img src="../../.gitbook/assets/image (4132).png" alt=""><figcaption></figcaption></figure>

* Variants: Manages the content of the marketing messages.&#x20;

<figure><img src="../../.gitbook/assets/image (4133).png" alt=""><figcaption></figcaption></figure>

For the Web Personalization channel, there is also Advertising Zones tab which controls the display zone of Inline templates on your websites.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdYe9zBFaThWnA_Fpwr39SGTdBiSENstoV3SEEHchfYeqjloDmMs8Xq99tKksQ1RxidiV_KPeYx-lvp1LhbqGgOZNEExYiDkqInZeQdGVLLwwp72nAG-g_1PUCe4h0N6jKeWYUCMqejtcu48FEa-8V7GDg?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

### Journey Level

* **Level 1: Journeys.** A journey is the setting of a marketing automation scenario, for example, a scenario aims to send emails to loyal customers, or a scenario aims to show a pop-up for whom view more than 3 items per hour
* **Level 2: Campaigns.** A campaign is attached to a marketing output channel, or called a destination in CDP 365. A journey could have multiple destinations, so it has multiple campaigns. For example, the journey of sending emails to loyal customers aims to break into two campaigns. The first campaign aims at whom spent more than $3,000 within 3 months, and the second campaign is for the rest customers
* **Level 3: Variants.** A variant is a template delivered marketing messages and it's a part of the campaign. A campaign could have 5 variants maximum.

### Channels

<table><thead><tr><th width="220">Channel</th><th>Description</th></tr></thead><tbody><tr><td>All channels</td><td>All channels that audiences can be reached</td></tr><tr><td>Web Personalization</td><td>Audiences can be reached by media templates display in a website</td></tr><tr><td>Web Notification</td><td>Audiences can be reached by Web Notification</td></tr><tr><td>App Notification</td><td>Audiences can be reached by App Notification</td></tr><tr><td>Email</td><td>Audiences can be reached by Email</td></tr><tr><td>SMS</td><td>Audiences can be reached by SMS</td></tr><tr><td>FB Messenger, Viber, Zalo, Whatsapp, Telegram, Line</td><td>Audiences can be reached by FB Messenger, Viber, Zalo, Whatsapp, Telegram, Line</td></tr><tr><td>File Transfer</td><td>Allow you to send data from CDP 365 to your system by files</td></tr><tr><td>Webhook</td><td>Allow you to send data from CDP 365 to your system through Webhook</td></tr><tr><td>Journey Orchestration</td><td>To create a Journey with the combination of many channels. This channel could not deliver Media Templates.</td></tr></tbody></table>

## II - Details

### How to create a new Customer Journey?

#### 1. Preparation&#x20;

A customer journey is a setting of a marketing automation scenario, so it requires:

* The data of the audiences to whom the journey reaches (attributes, events, or event attributes)
* The destination&#x20;
* The promotion pool (if the journey aims to send promotion codes)
* Variants or templates (email templates, media templates, etc.)

#### 2. Setup a customer journey&#x20;

To create a new Customer Journey, choose a channel you want on the left panel, and click button <img src="../../.gitbook/assets/image (151).png" alt="" data-size="line">. Then, follow the two steps below:

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfds3eJHddzYthxs5-0M79Cq7a_gE9kWQntAglXN1LmsrwMBr3DwyH-GiD7lMqgtPe7j2o1nKp1AKcwNNnk7Kcr_y4V3KzoO9v2yZ-m4bPD0RG3q49GVShmTKPi3xGKQZdaVTorck7m2taggyhQU0mFNSE?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

**Step 1**: Select a channel used to create the Journey

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcHsn-g004ulZujJBT39TpzplE4NN4VNXOQFpHVt1fwksRrlwvxZ_EwccL2rsCUDEJ60tMb-bYbT8VNYTvPI95rcJ3HMa7ALXgXKoQqf1S6r4Nu-3KhdGsyL91Yw90dsT-7sxSNbZ_j34X1bYDgw2PTjFty?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

There are 3 options to be chosen:

* **Blast campaign:** Create a simple Customer Journey. [Read here.](blast-campaign.md)
* **Create from scratch:** Create a new Customer Journey with full customization. If this option is selected, users will be moved to the second step.
* **Load existing Journey:** Create a new Customer Journey by copying an existing Journey. To do so, select the Journey you want to copy, then click on **Select** button.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfz3AgXkDIZJX8tciC1maSrW_xVB6JSIVuzRcMhsl0qXiFzEx-hQDEtEflUWQMebB2WVP57Yu2W2S5drVYCV8Ui7HI_ji1iNTHo9K5ghdwfBchd5SMrExPL5h2NLcxTMdzFLg35CnVdm-s83XgDcdVON-4U?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

**Step 2**: Setup a Customer Journey

Each rectangle block represents a node. A journey often comprises by 3 types of node:

* Trigger node
* Action nodes
* Destination nodes

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc3Q5EzcR4_FBs6If-_bu1E9TOAjv9hkAK2qfYfgaTpw0em_CkUODY9rTbAD-uPC-hT8k71aQ6APjiHgT5VxghjArRdFWpGpUDks02wrdjmpFZq9ZA3aM9RkqcgGdSD7AJbNJWuajxDw_5KUJY_dJGpJeA4?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

#### Trigger nodes

Trigger node contains conditions that trigger the journey. There are two trigger types

* Action-based trigger: the journey is triggered by events of audiences &#x20;
* Scheduled trigger: the journey is triggered by audience segments
* For example if demanding to send emails to loyal customers then use the scheduled trigger to start the journey. If demanding to show a pop-up for whom view more than 3 items per hour then use the action-based trigger to start the journey.

_Notice: a journey is triggered by one trigger node._&#x20;

#### Action nodes

Action nodes allow filtering of the audiences entering a journey that help the journey customize the marketing messages.

Action nodes have

<table><thead><tr><th width="188">Action node</th><th>Description </th></tr></thead><tbody><tr><td><a href="./#delay">Delay</a></td><td>The journey continues after a set of time</td></tr><tr><td><a href="./#if-then-branches">If/Then branches</a></td><td>The journey breaks into branches and an audience enters a branch only </td></tr><tr><td><a href="./#filter">Filter</a></td><td>Filter the audience being in the journey </td></tr><tr><td><a href="./#a-b-split">A/B split</a></td><td>Conduct A/B testing </td></tr><tr><td><a href="./#wait-for-event">Wait for event</a></td><td><p>The journey breaks into 2 branches </p><ul><li>Branch 1: the event waiting happens</li><li>Branch 2: the event waiting doesn't happen when the waiting time is out</li></ul></td></tr><tr><td><a href="./#update-info">Update info</a></td><td>Update attributes of existing customers or visitors in CDP 365</td></tr><tr><td>Update segment</td><td>Add or remove audiences from a segment </td></tr><tr><td>Parallel filter</td><td>The journey breaks into branches and an audience enters all branches</td></tr></tbody></table>

#### Destination nodes

* A destination node is a marketing output of the journey.&#x20;
* The destination is different from the channel. Channel is the communication means and destination is the vendor of that means.&#x20;
* For example, an Email channel could have Gmail destination, SendGrid destination, etc.



### Node Configuration

#### 1. Trigger node

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdjG0rKIISRCkxN-mZsEdVyNi7W56zuv0kv0WMpDiVE5dJUbYGvk3vXCMesdaiCxN_QteGYUPlfEewh98XW1V6_M1FAoyvLUIuHz-W3bYyfwRH1zBt3Nsgn5TlNsFtkG8OL9MGrgMVbH761SZDAFKzrFog?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcoTJnuefst-VXLejCHrb44000rVBPz2Bddu6anNlDdYA5GO5ZmAo8rIC6YujQ6rB5gUAsxfSsKZA3gentq-hSuyOHFO4xhLrX0t96cUg4zweLGe1E37xAcygNpOwJhtsJAsXiZ-vYu0gS4vreZlMEEEQ?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

A trigger node includes 4 groups of settings:

1. **Journey goal** - Decide if you want to calculate the Conversion coming from this Journey

You can add only 2 goals in a Journey. The list of goal includes the [conversion event](../../data-hub/event-sources/conversion-event.md) created in Data Hub.&#x20;

The rule to record the goal goes from First to Second, if the First goal was reached, the Second goal will be ignored.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfFYDaqhSUtCo22OK5iesyziXH7Zq9Is3gyHWo8Q6WyGnIH6Btr8qU0AzyWQo6ZuMRk9Smo7ScbTKDj6YHL5nBBa8SZ4rk4VleAG3daJwxpnyPSjfdh3_4deExTH92Tu_Hu4GcIVobMwwCiY9XJViNtxHGA?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

2. **Journey schedule** - The time to run and end a Journey

* Start date and Close date set the starting and ending date of the journey.&#x20;
* Trigger time sets the time when the journey stops or allows receiving the audience.&#x20;
* For example, a journey sends emails to loyal customers to encourage them to purchase in the last month of the year. And the journey pauses sending emails from 10 pm to 7 am every day during its lifetime. The setting should be <img src="../../.gitbook/assets/image (2250).png" alt="" data-size="line">

_Notice: If using the scheduled trigger, the setting would be_

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXceoETgNoJwTMAcYWUzO3FtVxbyz9psg-l9tQRQG4y_7HObJDWhu5EHAXhbGml41pTgdEjVPFx3izs6VfmipPm3YDVd3AGVxdWBaBoMaLQDWA2_vadtDscLxZGET89t8rkURUzSMmeqamzwLytvW5RwBBNQ?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

* Trigger journey is the interval of time the journey would repeat its process

3. Specific settings of each type of node

_**If using an Action-based trigger,**_ the journey would start when the audience satisfies the condition of the event&#x20;

* 'Select event' is the interaction of visitors or customers. 'Select event' includes 3 steps: select an event, select comparing method and input the value of the comparison&#x20;
* 'In any source of' is the domain where the event happened. After selecting an event, CDP 365 will propose a list of sources that have the event&#x20;
* 'Where' is a filter of the selected event. 'Where' could combine more than one event attribute by AND logic.

<figure><img src="../../.gitbook/assets/image (4134).png" alt=""><figcaption></figcaption></figure>



_**If using a Scheduled trigger,**_ the journey would send the marketing messages to audiences of the segments

* Included audiences is the audience segments the journey aims to. If the journey includes more than one segment, should pay attention to&#x20;
  * The audience can come from any of: means an audience can enter the journey if they belong to one segment
  * The audience must belong to all of: means an audience can enter the journey only when belonging to all the selected segment&#x20;
* Add specific customers is the specific audiences to which the journey reach
* Excluded audience is the audience segments the journey exclude&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXe1U9W3sVTLdNcocq9kCkKFdF5MZmGpEf6zhiuQ-3DpZBDXQmRXl88Svj5sX5VS706CGu25d0ky0Ihak__IUS1Svig75EFOXTp_yviNP2XBhO36HIJrsc6jWRAF3uwB3ZPWnXyoO_-jVhxuQ2uPhh34h4A?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

4. _**General settings -** The frequency an audience could be involved in this Journey_

* Unlimited frequency allows audiences to enter the journey unlimitedly
* Limited frequency, in contrast.&#x20;
* For example, a journey aims to show a pop-up for whom view more than 3 items per hour and a user views the pop-up once during the whole journey. The setting should be <img src="../../.gitbook/assets/image (1463).png" alt="" data-size="line">

#### 2. Action node

#### Delay

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdwijevhFbWhVfJJdGbWowiW2VfrxO0MzRoKQOdnlHgKrxi6dYsH5opIG_IPc5dmWy49GfT-_xFKJ28m83WdNig3CsZMq9gfFttXnyPJlpZ-217VNa_qATGmZKxkEoJ5G7ec7RNBxbGhp81199UdjsSTWWx?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

* Delay type has two options
  * Delay for the amount of time.
  * Delay until a date or time
* For example, a journey aims to show a product recommendation after 3 minutes customers add to the cart. The setting should be ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc4EZ4XGAmv3k7sAZpswfgEvoJF9MlSreL4JLoaG5_-IlpAOR8oHTbnZYO97y0EFrC2F-x5QvhyoqKYMMh5UGTiMcaD52QdGy9ixm_SzXKdcmC6g7mmlD5raxAwuFhq-xAS8Wr-Zebjqdg_i6eGHnXKtusv?key=McWN_Lv9ZK-QuQzVrY3nVw)

{% hint style="info" %}
Note: Maximum delay time is 365 days
{% endhint %}

#### If/Then branches

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdsoySY_Npq1JfjGmD7KaXfHmRtYbMl2sBEK5ej7JBhcZjhHXQLJrRLJkTx1mLmYgw3yNIbUWrWMj7ZopExqAkDFWldBM1NeD28afQr_rdJutr9OMCDHnhewCIuKDeKM0QSrqntBePPjzAaYC2OpD-0QuZT?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

* The node includes two steps of setting
  * Set the number of branches in If/then branches node
  * Set the filter condition in Yes nodes
* The node could have up to 20 branches including multiple Yes and a No
  * **Yes** includes filter conditions that split the audiences&#x20;
  * The audience will enter **No** if they don't satisfy the condition of Yes
* Filter type has three options
  * Filter by audience attribute uses the attributes of Visitors or Customers Business Object to filter
  * Filter by audience segment uses the segments to filter
  * Filter by trigger event attribute uses the event attributes of the trigger event to filter
* For example, a journey aims to show a pop-up for whom purchase more than 3 items, so the setting should be ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd8-hyKP_UJBWU7Y2q45yzn6LTQ_WmjOVjMp-xhKjU-RGtfWqR6k8NozvuGZE0spFMqclG3dUuRPxJlZdNHqkizQICVVb2aMDYQjX9ZUgwlSQ-N3vOrwsrtDlCXyArG6FnuADw_IYH9NG2efmKLn7ZW888?key=McWN_Lv9ZK-QuQzVrY3nVw)

#### Filter

The settings of the Filter node are as same to the If/Then branches node.

However, the audiences don't satisfy the filter, they would be **removed** from the journey.&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfUVMzmQNaJbRCmDc0TZQQZjL4D6ovDnjMZxa0TfkJJBiFEVBQuoibGpmcgciOhvIbf2vD8H55QZdf_aIZWoN885ausCkelKarqUAlbdgqXyeIUdBRKnI9wBsY9DldeHtjuTqzwwQSUuzggjIZKbj-rMKU?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

#### A/B Split

This node allows you to perform AB Testing method for your campaign. It divides the audiences into branches (groups) randomly.

* You can change the percentage by enter number in the box, clicking up/ down button or drag and drop slider bar.&#x20;
* To add a new group, click ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeWMUu4MsTIBSSVG-E_63qqXz-btrwlYPfEpqqtcvP64vFBQd7q4j2YsQrnXJMg4m6pKaVEeHi6psWzqh5zh31-ZHDcS6V8LNC5GhLdS_kRPpL_KlPjxw4RgxNmMOPgvpmWvQf7Neepz0_r7Fkovth72VYb?key=McWN_Lv9ZK-QuQzVrY3nVw).
* To add a Control Group branch, turn on the switch button <img src="../../.gitbook/assets/image (2612).png" alt="" data-size="line">. The audiences enter this branch will note receive any message, meaning you could not add Destination node in this branch.
* If you want to change Group's name, click on the node you want and change the name in _Branch name_ field. <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd-u-X03fUNPACV3AXjt3by6k597fx_xQoZHTwozNL9fgv9cmqMJCIOFMA9WvQgbxjjC5u67XHFLL2JyYgqgFR4vG9RTAXT_4iR47Mxb2grHvpBZ01h_-mNqeMYiOJIdG6HaEtH1I_vtXflgS5hGsmk85UQ?key=McWN_Lv9ZK-QuQzVrY3nVw" alt="" data-size="line">
* If you want to create a Segment of audience who entered this branch, you could use event _Entered Control Group_ and combine it with any condition you want.   <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcfugySjYnsSVcEDklJlV8nBzB3N0dUYWhijwdrgeySiAPVytXWAhHec0D6sCWzNhUp1sGqthScPxcDfrd3QFGhrmNzh5Vg6Q_KGNYktpqp8VaExkCIjb6XaEYa8QlAPC6vuIqyCR3k_HBvq9T8Tr_NrB_5?key=McWN_Lv9ZK-QuQzVrY3nVw" alt="" data-size="line">

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc0Nk_6C3EPr7_5QPE9YnCWgKlVfvYoGRSQck3piV1aERxeLJP5P6CTRGzsXGz6zVLJ8i1pART4IyEY6obHWBRAlX2RYlWWaLKlyJeYYX9WweFK-TPLCHLrWEvbNiPT1JY06RlKT6AW8l05pA_81NWS7JDq?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

#### Wait for event

For example, the journey sends a promotion code to the audiences who don't purchase after 5 minutes of adding to the cart.

The journey should be&#x20;

* Triggered by the 'add to cart' event
* Wait the 'checkout cart' event for 5 minutes

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdsIXBAqDc7q9Tp053B8RWLaXAGlLe1L815BJaPkzv3ppEkisl9Gh6gqMBXHeNocpDRjTBrBqgeUnrfvl3JUyMT-lqwBV3bFlQeC1GI2bTtP4YpuYDVk9c7kcF3n4-lrB3UOxf7auhXJFXRFYGRUOqgtOwq?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

#### Update info

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcmVxMv4w3HvjK9l9zs8yekcaLH_GdHWWf6aqIZ4pMGE5D3QoXAKtWE3WgiWbI_EMGuOM9qEVoB_RAKxGyQrrxLtnssGWkdP_wV4cQms2kBYc9umDBDkvLJX3XO9-NsEjbuFySILhThb7HKBcF45X7UOj9E?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

The settings includes&#x20;

* Business Objects could be Visitor or Customer
* Attribute is the attribute of Visitor or Customer&#x20;
* Data type is the format of the data
* Node action is the update methods including&#x20;

<table><thead><tr><th width="202">Node action</th><th>Description</th></tr></thead><tbody><tr><td>Reset value</td><td>Reset the value of the field</td></tr><tr><td>Change value</td><td>Change the value of the field</td></tr><tr><td>Push new element</td><td>Add an element to a field that is an array of data type</td></tr></tbody></table>

* New value is the value would be updated to the attribute. It has two methods to insert
  * Input from keyboard
  * Use a formula by selecting ![](https://lh4.googleusercontent.com/Zy2yhDZgBEeVNTn0APARZ8EYnpy8QswQ9Ab5POh3VqPCPyj0uGqaJ3gBZ0jzPEFu16P5LkOgfdb8cCgnCRhih8INLasf0Irj6AwfOVaxQbTMOPOWa14c-nEpJjpwrA8rJO2oHZpo2dFpr5UAlpXgcNRZ73SWGKUZ-Yh5TdF2vPMWwdoMHZ5P5JCmwR9rNg)

_**If the new value is generated by a formula**_

* Variable name: name of the variable
* Expected value: variable formula
* Ignore the null value, and use the default value instead: it does not accept the null value and replaces the null value with the default value declared at the Default value
* Allow update the null value: allow updating the null value

#### Update segment

The configuration of update segment includes

* Node action includes 'Add audiences to segments' and 'Remove audiences from segment'.&#x20;
* Segment type has 'Visitor segments' and 'Customer segments'. The setting is to add or remove the audiences into the existing segments of Visitors and Customers.&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdedWWNq-c2iCkl2wqqIO5l0voiLrbb6E33x_BQNnzx0s0ck-9PB5hh2EmMdvLuf63nVb59oMaxq2SsK4QsLjFoypE7Lwd-woqh56AYu9JaIercpVCGCuQzZ7tEq4xe8XnXMicrNgRmJtBmyWE2Fop_yzv0?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

#### Parallel filter

The settings of the parallel filter is as same the settings of the if/then branches.

However, the audiences must go through all the branches of the parallel filter.&#x20;

#### 3. Destination node

#### 3.1 Choose a method to design the campaign

After adding a destination nodes, there are many design method you could choose to compose your message. Depending on the chosen destination node, these options could be vary.

**Web Embedded**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXezISw8fz4MGeP5LCV6WEDTdCAwjgmUCSjhiFm8aeylBBsequy6jESFXBqcgsU2uYDVuh_v5s2PdX1oQdRMiA58otDDQKDakYMEmPiM1RSCHFlQ_VcJQYKeKtVuTDElumE2fV0ANosk8ofiokLNbXL-eH0d?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

* Design from template
* Load Existing Design
* Design from JSON

**Destinations which have built-in templates**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXePDi0GGHb07rI_D3quge_1JggfqCYJQa2bSnsWYpvK3ls2DXV0GUw95QeGLuT720cXrEviFbhcwTj9eAeAm4u7FbVB1NMpziEyg3iprAsE7EOGlvyLJlAH7DD_SzNcqk1ydvECcU86b5eWQFNK2NujXI9m?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

* Choose a template
* Load existing design

**Destinations which does not have built-in templates**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeDHZivSvvyShuU94dP5z2Qkvy7-9JeysmyPtEP66YSetfMwJCq_NUCzdyDuKF_xZPypu-RuuCYcVfl_of8vBTjDsgJ9vAZ10ABQN4ClI4Otzrb1cjnUR9w3Z7QDc4PJYmdzJ36yi-0OCFOF1DDUJaIzC_9?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

* Design from scratch
* Load existing design

**3.2 Configure your campaign**

A destination node includes two steps of settings:

<mark style="color:blue;">**Settings**</mark>**&#x20;-** Choose the destination and how you want to deliver the message to your audience. Depending on the chosen destination node, the configuration fields and requirements are vary.&#x20;

* Campaign name \*: The name of your campaign
* Delivery destination \*: The specific destination to be used to deliver your message
* Delivery algorithm \*: The algorithm delivering the campaign, randomization by default. If the journey has more than one campaign, each of the campaigns is delivered randomly to the audiences
  * **Web Embedded**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcC6HcAwmQbMMrc8Gxn1qDxcYc93faqEn0EWtkZyKR3UKsArH9TCwr0I2hlt_Jg9BrecWPGla7RqJ7nPddX2BDg5b8GjA5hRcZqdGNm64ilLYz6txrNBGZW8vXc9QP0nrbnwoSh_If8k63Xtgu5-hTRPFPo?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

* Display Ad Zone: The zone on the website where the media will be placed
* Content Placement: The method to place the media on the zone
* Zone's display priority: The priority of this template comparing to others
  * **Other channels**
* Delivery hours of the day are the time when the campaigns start sending out their variants.

***

<mark style="color:blue;">**Compose**</mark>**&#x20;-** Determine the content of your message. Based on the chosen channel, the configuration and requirements will be vary. But there are similar settings listed below:

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXduPqUw2NHNJB5st1cdXVGVrdnSnyFnYgvW303se8t31-qE3FVC0UZ4VQcjrQ34ARBCjgyDeSXsG57SbDADzT963yXeEL9uG6pq8ZEUqrSRiWHekKPAnnneWsWw3P8sXn-G_b9Eq3eCQO2qo20EEN6K7Nk?key=McWN_Lv9ZK-QuQzVrY3nVw" alt=""><figcaption></figcaption></figure>

* Variant priority: The displaying probability of variants in a campaign
* Variant name: The name of the variant

[See more about the Data table ](../../cdp-365-introduction/cdp-365s-interface.md#data-table)
