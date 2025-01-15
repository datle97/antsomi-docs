# October 2022

These are the features and improvements released during the month of Oct 2022

## Releases

* [Email Template (beta) - Improve UI Email destination in Journey](october-2022.md#email-template-beta-improve-ui-email-destination-in-journey)
* [Media template - Grouping for recommendation algorithms](october-2022.md#media-template-grouping-for-recommendation-algorithms)
* [PEP - Viber Rich media -  Change the maximum number of characters of the label from 50 to 30](october-2022.md#pep-viber-rich-media-change-the-maximum-number-of-characters-of-the-label-from-50-to-30)
* [Dataflow - Hide all mapping information except email and phone when pushing data Facebook/Google audiences](october-2022.md#dataflow-hide-all-mapping-information-except-email-and-phone-when-pushing-data-facebook-google-audie)
* [Insight - SQL Workspace - Allow edit AT table](october-2022.md#insight-sqlworkspace-allow-edit-at-table)
* [Insight - Report - Add "Metric slider" and "Control slider" feature](october-2022.md#add-metric-slider-and-control-slider-feature)
* [Data Hub - Download and Create attribute from upload for BO Attributes](october-2022.md#data-hub-download-and-create-attribute-from-upload-for-bo-attributes)
* [Improved Segment upload flow and allows creating upload segments from within Journey](october-2022.md#improved-segment-upload-flow-and-allows-creating-upload-segments-from-within-journey)
* [Improve Upload UI/UX](october-2022.md#improve-upload-ui-ux)
* [Improvement when creating Segment Dynamic and Computation](october-2022.md#improvement-when-creating-segment-dynamic-and-computation)
* [Email template (beta) - Add "Table" block](october-2022.md#email-template-beta-add-table-block)
* [Email Template (beta) - Add "Countdown" block](october-2022.md#email-template-beta-add-countdown-block)
* [Email Template (beta) - Add "Unsubscribe" box](october-2022.md#email-template-beta-add-unsubscribe-box)
* [Marketing Hub - Customer Journey - Update UX for Edit Journey](october-2022.md#marketing-hub-customer-journey-update-ux-for-edit-journey)
* [Marketing Hub - Customer Journey - Support Bullet Points & Emoji for Viber Content](october-2022.md#marketing-hub-customer-journey-support-bullet-points-and-emoji-for-viber-content)
* [Marketing Hub - Customer Journey- Add blank template creation feature](october-2022.md#marketing-hub-customer-journey-add-blank-template)
* [Marketing Hub - Customer Journey - Preview viber & inforbip viber](october-2022.md#marketing-hub-customer-journey-preview-viber-and-inforbip-viber)
* [Add Description for Segment status, Last computation status and Journey status](october-2022.md#add-description-for-segment-status-last-computation-status-and-journey-status)
* Marketing Hub - Support short link when Quick test SMS
* [Dataflow - Destination channel- Suggest names for some destination channels](october-2022.md#dataflow-destination-channel-suggest-names-for-some-destination-channels)

### Email Template (beta) - Improve UI Email destination in Journey

<figure><img src="../../.gitbook/assets/image (642).png" alt=""><figcaption></figcaption></figure>

### Media template - Grouping for recommendation algorithms

<figure><img src="../../.gitbook/assets/image (1746).png" alt=""><figcaption></figcaption></figure>

### PEP - Viber Rich media -  Change the maximum number of characters of the label from 50 to 30

<figure><img src="../../.gitbook/assets/image (680).png" alt=""><figcaption></figcaption></figure>

### Dataflow - Hide all mapping information except email and phone when pushing data Facebook/Google audiences

<figure><img src="../../.gitbook/assets/image (991).png" alt=""><figcaption></figcaption></figure>

### Insight - SQL Workspace - Allow edit AT table

* Can add a new column + edit columns already in the Analytic table
* Can push data into the newly added or edited column

### Insight - Report - Add "Metric slider" and "Control slider" feature

<figure><img src="../../.gitbook/assets/image (2105).png" alt=""><figcaption></figcaption></figure>



### Data Hub - Download and Create attribute from upload for BO Attributes

### Improved Segment upload flow and allows creating upload segments from within Journey

* There is an additional option to both create a segment and insert customers / visitors into Customers / Visitors Business Object

<figure><img src="../../.gitbook/assets/image (2505).png" alt=""><figcaption></figcaption></figure>

* Allows creating segments in the journey

<figure><img src="../../.gitbook/assets/image (1838).png" alt=""><figcaption></figcaption></figure>

**NOTE:** For Segment never built (member = null) => display warning icon and hover show message: “Data of the segment will be ready after 3 hours to compute. You need to choose the right time to run the journey.”

<figure><img src="../../.gitbook/assets/image (2433).png" alt=""><figcaption></figcaption></figure>



### Improve Upload UI/UX

* Remove popup select Local
* Synchronize Upload screens

<figure><img src="../../.gitbook/assets/image (1659).png" alt=""><figcaption></figcaption></figure>

### Improvement when creating Segment Dynamic and Computation

* Add "Waiting initial" status for segments that do not run immediately upon creation.
* Change the label of the "Build" button when creating the segment to "Save"
* When creating Segment / Computed Attribute with type Dynamic and Repeat by other than None. Clicking Save will display a pop up with a successful creation message and ask if the user wants to calculate it too?&#x20;
  * If you click Yes, you will return to the all segment screen and the process compute segment just created. This compute time will not count occurrences. Change "last computation status" to "Waiting"
  * If you click No, return to the all segment screen and wait for the compute schedule. Change "last computation status" to "Waiting initial"

### Email template (beta) - Add "Table" block

<figure><img src="../../.gitbook/assets/image (430).png" alt=""><figcaption></figcaption></figure>

### Email Template (beta) - Add "Countdown" block

<figure><img src="../../.gitbook/assets/image (1308).png" alt=""><figcaption></figcaption></figure>

### Email Template (beta) - Add "Unsubscribe" box

<figure><img src="../../.gitbook/assets/image (2204).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (438).png" alt=""><figcaption></figcaption></figure>

### Marketing Hub - Customer Journey - Update UX for Edit Journey

Change the Cancel button to Close to avoid confusing the user. Apply when Create and Edit Journey

Show confirmation popup after clicking close button

<figure><img src="../../.gitbook/assets/image (2394).png" alt=""><figcaption></figcaption></figure>

### Marketing Hub - Customer Journey - Support Bullet Points & Emoji for Viber Content

<figure><img src="../../.gitbook/assets/image (2314).png" alt=""><figcaption></figcaption></figure>

### Marketing Hub - Customer Journey- Add blank template creation feature

<figure><img src="../../.gitbook/assets/image (2499).png" alt=""><figcaption></figcaption></figure>

### Marketing Hub - Customer Journey - Preview viber & inforbip viber

<figure><img src="../../.gitbook/assets/image (806).png" alt=""><figcaption></figcaption></figure>

### Add Description for Segment status, Last computation status and Journey status

**Computation status:**

* Waiting Initial: Segment is waiting for the computed schedule.
* Waiting: Segment has entered the queue to be computed
* Computing: Segment in progress
* Ready to use: Segment ready to use for journeys or another segments. However, still in the process of updating to profiles
* Success: Segment has been built successfully
* Unsuccess: Segment has been built unsuccessfully

Example:

<figure><img src="../../.gitbook/assets/image (1833).png" alt=""><figcaption></figcaption></figure>

**Journey status:**

* In design: Journey is in design, not ready to run
* Active: Journey is in progress
* Scheduled: The campaign is about to run.
* Closed: Journey is coming to processing time
* Paused: The campaign is temporarily paused but still allowing new audiences enter
* Prozen: The campaign is on hold and does not allow new audiences enter
* Error: An error occurred during journey processing.
* Aborted: Journey is forced to a complete stop
* Removed: Journey is deleted

Example:

<figure><img src="../../.gitbook/assets/image (2098).png" alt=""><figcaption></figcaption></figure>



### Dataflow - Destination channel- Suggest names for some destination channels

When creating a destination, the default name will be displayed: **Untitled destination # {destination number}**

Destination channels will support:&#x20;

* Postgres Database
* Export Google Ads Audiences
* Export Facebook Audiences
* Export Google BigQuery
* Tiktok Audience
* Sale force
