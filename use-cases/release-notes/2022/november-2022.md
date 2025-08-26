# November 2022



These are the features and improvements released during the month of Oct 2022

## Releases

* [Media template & Email template - Notify when there is an invalid element in the template](november-2022.md#media-template-and-email-template-notify-when-there-is-an-invalid-element-in-the-template)
* [Data Hub - Event source - Open auto-suggestion setting for Event attribute](november-2022.md#data-hub-event-source-open-auto-suggestion-setting-for-event-attribute)&#x20;
* [All - Displays the DateTime fields according to the portal's time zone on the object list and object details page](november-2022.md#all-displays-the-datetime-fields-according-to-the-portals-time-zone-on-the-object-list-and-object-de)
* [Customer Journey - Add “add personalization” feature to the “Viber yondu” destination](november-2022.md#customer-journey-add-add-personalization-feature-to-viber-yondu-destination)
* [Insight - Report - Pages & Navigation bar](november-2022.md#insight-report-pages-and-navigation-bar)
* [Personas - Segment - Add the “Next computed on” column and rename the “Computation status” column to the “Last computation status” column](november-2022.md#personas-segment-add-the-next-computed-on-column-and-rename-computation-status-column-to-last-comput)&#x20;
* [Media template & Email template - Add feature set index for Slide show block and Column block](november-2022.md#media-template-and-email-template-add-feature-set-index-for-slide-show-block-and-column-block)
* [Data Hub - Business Object - Change the label "Import Histories" to “Upload Histories”](november-2022.md#data-hub-business-object-change-the-label-import-histories-to-upload-histories)
* [Data Hub - Event source - Add the “Associate with UTM” checkbox in the Setting tab](november-2022.md#data-hub-event-source-add-associate-with-utm-checkbox-in-setting-tab)
* [Dataflow - Datasource - Add Google Analytics V4 Datasource](november-2022.md#insight-and-dataflow-datasource-add-google-analytics-v4-datasource)
* [IAM - Limitation & Default Notify của Portal](november-2022.md#iam-limitation-and-default-notify-cua-portal)
* [Customer Journey - Send time limit for send/push channels](november-2022.md#customer-journey-send-time-limit-for-send-push-channels)&#x20;
* [Personas & Data Hub - Add "Enable, Disable, Archive, Recover" action and automatically switch status Disable/ Archive/ Permanently delete for Business Object, BO Attributes & Collections/Segment](november-2022.md#personas-and-data-hub-add-enable-disable-archive-recover-action-and-automatically-switch-status-disa)
* [Media template - Add the Get top algorithm to the Product-based group](november-2022.md#media-template-add-the-get-top-algorithm-to-the-product-based-group)
* [Media template & Email template - Add the Notify algorithm to the Product-Based group ](november-2022.md#media-template-and-email-template-add-the-notify-algorithm-to-the-product-based-group)
* [Media template - Improvements to the Display condition feature](november-2022.md#media-template-improvements-to-the-display-condition-feature)
* [All - Operator matches any - Add comma as thousands separator](november-2022.md#all-operator-matches-any-add-comma-as-thousands-separator)
* [Marketing Hub - Destination - Add "eSMS" & "ZaloOA" destination](november-2022.md#marketing-hub-destination-add-esms-and-zalooa-destination)&#x20;
* [Customer Journey - Add BO Promotion Code into Add personalization in Customer Journey settings](november-2022.md#customer-journey-add-bo-promotion-code-into-add-personalization-in-customer-journey-settings)
* [MediaTemplate - Create Table Block For MediaTemplate](november-2022.md#mediatemplate-create-table-block-for-mediatemplate)
* [Media template - Add toggle allows turning on and off thumbnail capture](november-2022.md#media-template-add-toggle-allows-turning-on-and-off-thumbnail-capture)
* [Media template - Add Limited submit option to Optin fields block](november-2022.md#media-template-add-limited-submit-option-to-optin-fields-block)
* [Data Hub - Event source - Add table and chart to event detail viewing ](november-2022.md#data-hub-event-source-add-table-and-chart-to-event-detail-viewing)
* [Dataflow - Add the "Zalo Official Account" datasource](november-2022.md#dataflow-add-the-zalo-official-account-datasource)
* [Data Hub - Event sources - Add a new attribute ‘Time to live’ ](november-2022.md#data-hub-event-sources-add-a-new-attribute-time-to-live)
* [Data Hub -  Analytic models - Add "unique sketch" and improve build AM](november-2022.md#data-hub-analytic-models-add-unique-sketch-and-improve-build-am)&#x20;
* [MediaTemplate - Add Option Do not stack on mobile for Column Block ](november-2022.md#mediatemplate-add-option-do-not-stack-on-mobile-for-column-block)
* [Media template & Email template - Load event trigger and source when choosing Distance algorithm of BO Settings](november-2022.md#media-template-and-email-template-load-event-trigger-and-source-when-choosing-distance-algorithm-of)
* [Customer - Journey - Change Zoom settings flow chart](november-2022.md#customer-journey-change-zoom-settings-flow-chart)

### **Media template & Email template - Notify when there is an invalid element in the template**

* Display the error message when clicking save but on the template, there are invalid components (in BO settings, Block)
* In blocks, a warning icon will be displayed if there is an error.
* The fields in the settings of the components will show detailed error messages.

<figure><img src="../../../.gitbook/assets/image (708).png" alt=""><figcaption></figcaption></figure>

### Data Hub - Event source - Open auto-suggestion setting for Event attribute

Add Auto suggestion checkbox for event attribute

<figure><img src="../../../.gitbook/assets/image (810).png" alt=""><figcaption></figcaption></figure>

### All - Displays the DateTime fields according to the portal's time zone on the object list and object details page

On the list of objects page, the DateTime fields such as: created date, last modified on, ... display information according to the portal timezone.

In the object details page, time fields such as: start date, start time, end date, ... display information by portal timezone and display timezone labels to know that this field is being retrieved by timezone any.

### Customer Journey - Add “add personalization” feature to “Viber yondu” destination

<figure><img src="../../../.gitbook/assets/image (1168).png" alt=""><figcaption></figcaption></figure>

### Insight - Report - Pages & Navigation bar

<figure><img src="../../../.gitbook/assets/image (2165).png" alt=""><figcaption></figcaption></figure>

### Personas - Segment - Add the “Next computed on” column and rename “Computation status” column to “Last computation status” column&#x20;

* Rename "Computation status" column to "Last computation status" column&#x20;
* Add the "Next computed on" column to display the time for the next computation

<figure><img src="../../../.gitbook/assets/image (472).png" alt=""><figcaption></figcaption></figure>



### Media template & Email template - Add feature set index for Slide show block and Column block

* When adding a dynamic block to a slide or column, the default will get the index of that slide/column for the dynamic block.
* Add the SetIndex function to automatically set the index of dynamic blocks for all slides/columns, the index will be within the specified range. All dynamic blocks in the same slide/column will have the same index. Note: Index limit to 90.

<figure><img src="../../../.gitbook/assets/image (1023).png" alt=""><figcaption></figcaption></figure>

### Data Hub - Business Object - Change the label "Import Histories" to “Upload Histories”

<figure><img src="../../../.gitbook/assets/image (638).png" alt=""><figcaption></figcaption></figure>

### Data Hub - Event source - Add “Associate with UTM” checkbox in Setting tab

When this check box is enabled, the data of the UTM, if any, will be automatically recorded to the ATM

<figure><img src="../../../.gitbook/assets/image (2210).png" alt=""><figcaption></figcaption></figure>

### Insight & Dataflow - Datasource - Add Google Analytics V4 Datasource

<figure><img src="../../../.gitbook/assets/image (2201).png" alt=""><figcaption></figcaption></figure>



### IAM - Limitation & Default Notify của Portal

Added 2 more tabs: Limitation and Notification in the detail page of Network.

* Limitation: Set limits for objects in the portal
* Notification: Set up notifications for objects in the portal.

<figure><img src="../../../.gitbook/assets/image (2545).png" alt=""><figcaption></figcaption></figure>



### Customer Journey - Send time limit for send/push channels&#x20;

Push/send channels will have an additional "Delivery Hours of the Day" field to choose the time of day to send. Includes 2 options:

All time: as now, unlimited delivery time.

Specific hours of the day: Choose a specific time of day for delivery

* Hold until next valid time frame: If the data has not been sent, it will wait until the next valid time frame and send again.
* Skip deliver at invalid time frame: If it has not yet been sent, it will skip sending those data

<figure><img src="../../../.gitbook/assets/image (2510).png" alt=""><figcaption></figcaption></figure>



### Personas & Data Hub - Add "Enable, Disable, Archive, Recover" action and automatically switch status Disable/ Archive/ Permanently delete for Business Object, BO Attributes & Collections/Segment

Add actions: Enable, Disable, Archive, Recover in the list of BOs, BO Attributes and Collections/Segment

* Enable: Enable disabled or archived BO/ BO attributes/ Collections/Segment
* Disable: Disable enabled BO/ BO attributes/ Collections/Segment
* Archive: Archive enabled or disabled BO/ BO attribute/ Collections/Segment
* Recover: Recover archived BO/ BO attribute/ Collections/Segment becomes enabled or disabled BO/ BO attribute/ Collections/Segment.

<figure><img src="../../../.gitbook/assets/image (1138).png" alt=""><figcaption></figcaption></figure>

Automatically change the status of the BOs/ BO attributes/ Collections/Segment to disabled, archived or permanently deleted.

* BO/BO Attribute/ Collections/Segment will change status when not used after X days
* X days will be set in the Limitation of the network

### Media template - Add the Get top algorithm to the Product-based group

Get top algorithm allows getting as many products based on an attribute.

<figure><img src="../../../.gitbook/assets/image (1225).png" alt=""><figcaption></figcaption></figure>

### Media template & Email template - Add the Notify algorithm to the Product-Based group&#x20;

Send notifications to users for products that the user has subscribed to or added to a wishlist under certain conditions.

<figure><img src="../../../.gitbook/assets/image (2607).png" alt=""><figcaption></figcaption></figure>

### Media template - Improvements to the Display condition feature

Change the Condition's options  of Column block and Slideshow block to

<figure><img src="../../../.gitbook/assets/image (1798).png" alt=""><figcaption></figcaption></figure>

### All - Operator matches any - Add comma as thousands separator

<figure><img src="../../../.gitbook/assets/image (1452).png" alt=""><figcaption></figcaption></figure>

### Marketing Hub - Destination - Add "eSMS" & "ZaloOA" destination

<figure><img src="../../../.gitbook/assets/image (2414).png" alt=""><figcaption></figcaption></figure>

### Customer Journey - Add BO Promotion Code into Add personalization in Customer Journey settings

Allow end users to apply BO Promotion code when setting add personalization in Destination node of the journey

<figure><img src="../../../.gitbook/assets/image (1273).png" alt=""><figcaption></figcaption></figure>

### MediaTemplate - Create Table Block For MediaTemplate

* Allow end users to add dynamic content to tables and apply sorts and filters to deliver target Marketing messages
* Allow end users to edit styles of content

<figure><img src="../../../.gitbook/assets/image (1086).png" alt=""><figcaption></figcaption></figure>

### Media template - Add toggle allows turning on and off thumbnail capture

Turn on: capture thumbnail&#x20;

Turn off: don’t capture thumbnail

<figure><img src="../../../.gitbook/assets/image (2462).png" alt=""><figcaption></figcaption></figure>

### Media template - Add Limited submit option to Optin fields block

* Limit the number of submitting information within a hour/day/month based on phone number, email address or name
* Allow applying up to 3 limitations per optin fields block

<figure><img src="../../../.gitbook/assets/image (1862).png" alt=""><figcaption></figcaption></figure>

### Data Hub - Event source - Add table and chart to event detail viewing&#x20;

When viewing details of an event, 2 new tabs appear:

* Event log:  history details of the event that CDP tracks&#x20;
  * The time range of the chart last from the last 5 minutes to the last 6 hours
  * The table of histories provide two types of event: received and rejected &#x20;
* Event attributes: details of event attributes assigned to the event

<figure><img src="../../../.gitbook/assets/image (2069).png" alt=""><figcaption></figcaption></figure>

### Dataflow - Add the "Zalo Official Account" datasource

Description: get a list of interested users Official Account

<figure><img src="../../../.gitbook/assets/image (1474).png" alt=""><figcaption></figcaption></figure>



### Data Hub - Event sources - Add a new attribute ‘Time to live’&#x20;

When viewing details of an event, 2 new tabs appear

* Time to live: adjust the time that CDP storages values of the event&#x20;
  * CDP stores the values of an event for up to 730 days, which is set by default&#x20;
  * Time to live allows adjusting the storage time within the limited storage time&#x20;
* After adjusting the storage time, CDP applies a new storage time to all sources using this event&#x20;
* The attribute requires to be filled

<figure><img src="../../../.gitbook/assets/image (604).png" alt=""><figcaption></figcaption></figure>



### Data Hub -  Analytic models - Add "unique sketch" and improve build AM

* Add measure type Unique Count Approximate (Datasketches)

<figure><img src="../../../.gitbook/assets/image (931).png" alt=""><figcaption></figcaption></figure>

* Display ID of reference objetcts

<figure><img src="../../../.gitbook/assets/image (1628).png" alt=""><figcaption></figcaption></figure>

* Add Treat as attribute when selecting BO for AM

<figure><img src="../../../.gitbook/assets/image (2311).png" alt=""><figcaption></figcaption></figure>



### MediaTemplate - Add Option Do not stack on mobile for Column Block&#x20;

Apply only to Mobile mode&#x20;

Responsive design&#x20;

* Includes 1 toggle ‘Do not stack on Mobile’ - turning on or off stacking on mobile view when the design is intended to display on Desktop type &#x20;
* Align column on a column to make components shown fit Mobile

<figure><img src="../../../.gitbook/assets/image (1279).png" alt=""><figcaption></figcaption></figure>

### Media template & Email template - Load event trigger and source when choosing Distance algorithm of BO Settings

Load the event and the source which are selected in the Action-based trigger when applying the Distance algorithm

<figure><img src="../../../.gitbook/assets/image (623).png" alt=""><figcaption></figcaption></figure>

### Customer - Journey - Change Zoom settings flow chart

Change step each increase or decrease to 5%

<figure><img src="../../../.gitbook/assets/image (2115).png" alt=""><figcaption></figcaption></figure>
