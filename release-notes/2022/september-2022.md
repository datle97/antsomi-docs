# September 2022

These are the features and improvements released during the month of Sept 2022

## Releases

* [Media Template - Improvements to image block ](september-2022.md#media-template-improvements-to-image-block)
* [Media Template - Allow to enter and display more than 2 digits in Countdown block](september-2022.md#media-template-allow-to-enter-and-display-more-than-2-digits-in-countdown-block)
* Portal Setting - Account - Allow create a new account from email of a previously removed account
* [Marketing Hub - Promotion pool - Add "Unique Coupon" allocation configuration](september-2022.md#marketing-hub-promotion-pool-add-unique-coupon-allocation-configuration)
* [Data Hub - Add Computation Schedule for the Computed Attribute](september-2022.md#data-hub-add-computation-schedule-for-the-computed-attribute)
* [Data Hub - Support auto suggestion for attributes whose datatype is array](september-2022.md#data-hub-support-auto-suggestion-for-attributes-whose-datatype-is-array)
* [Marketing Hub - Customer Journey - Move the "Quick test" button to be on the same line as variant name](september-2022.md#marketing-hub-customer-journey-move-the-quick-test-button-to-be-on-the-same-line-as-variant-name)
* [Send Journey ID, Campaign ID, Variant ID when tracking "Submit Lead" even](september-2022.md#send-journey-id-campaign-id-variant-id-when-tracking-submit-lead-event)
* [Email template (beta) & Media template - Add display format for Date field](september-2022.md#media-template-add-display-format-for-date-field)
* [Media template - Improve "Distance" algorithm](september-2022.md#media-template-improve-distance-algorithm)
* [Email template (beta) & Media template - Change default appearance of pop up Filter in BO Setting](september-2022.md#media-template-add-display-format-for-date-field)
* [Email template (beta) - Add the "subject" & "send as" default](september-2022.md#email-template-beta-add-the-subject-and-send-as-default)
* [All listing - Export - The default is csv instead of excel](september-2022.md#all-listing-export-the-default-is-csv-instead-of-excel)
* [Add "Select all" feature for search results](september-2022.md#add-select-all-feature-for-search-results)
* [Marketing Hub - Add "Messenger" Destination](september-2022.md#marketing-hub-add-messenger-destination)
* [Dataflows - Datasource - Add "Facebook Messenger" connector](september-2022.md#dataflows-datasource-add-facebook-messenger-connector)
* [Marketing Hub - Add "Telerivet" Destination](september-2022.md#marketing-hub-add-telerivet-destination)
* [Marketing Hub - Add "Klasik SMS" Destination](september-2022.md#marketing-hub-add-klasik-sms-destination)
* [Marketing Hub - Add "Firebase Cloud Messaging" Destination](september-2022.md#marketing-hub-add-firebase-cloud-messaging-destination)
* [Marketing Hub - Remove required for Phone and Email fields in Caresoft Destination](september-2022.md#remove-required-for-phone-and-email-fields-in-caresoft-destination)
* [Email template (beta) - Integrate new email templates into Journey](september-2022.md#email-template-beta-integrate-new-email-templates-into-journey)
* [Media Template - Add "UTM tracking" setting](september-2022.md#mediatemplate-add-utm-tracking-setting)
* [Marketing Hub - Add "SMS LACHONG MEDIA" destination](september-2022.md#marketing-hub-add-lac-hong-destination)
* [Dataflows - Datasource - Add "CDP 365 Segment's Members" connector](september-2022.md#dataflows-datasource-add-cdp-365-segments-members-connector)
* [Marketing Hub - Promotion center - Add Journey ID, Variant name, Campaign name](september-2022.md#marketing-hub-promotion-center-add-journey-id-variant-name-campaign-name)
* [Marketing Hub - Promotion code - Update status flow of Promotion code](september-2022.md#marketing-hub-promotion-code-update-status-flow-of-promotion-code)
* [Marketing Hub - Improve UI Include/ Exclude Audiences interface and Is member of filter interface](september-2022.md#marketing-hub-improve-ui-include-exclude-audiences-interface-and-is-member-of-filter-interface)
* [Marketing Hub - Improve UI to Promotion Code Detail](september-2022.md#marketing-hub-improve-ui-to-promotion-code-detail)
* [Marketing Hub - Destination - Support Enter character when entering Content in some Variant sending message](september-2022.md#marketing-hub-destination-support-enter-character-when-entering-content-in-some-variant-sending-mess)

### Media Template - Improvements to image block&#x20;

* Add Image URL
* Add Input for edit height of image
* Add unit (%, px, auto) for width of image and unit (px, auto) for height of image

<figure><img src="../../.gitbook/assets/image (1506).png" alt=""><figcaption></figcaption></figure>

### Media Template - Allow to enter and display more than 2 digits in Countdown block

<figure><img src="../../.gitbook/assets/image (2425).png" alt=""><figcaption></figcaption></figure>

### Marketing Hub - Promotion pool - Add "Unique Coupon" allocation configuration

<figure><img src="../../.gitbook/assets/image (2312).png" alt=""><figcaption></figcaption></figure>

For every: Audience Allocation (Default). You can add "Or every":

1. Visitor (Default)
2. Customer
3. Email
4. Phone&#x20;

Example: If select "For Every" : "Audience Allocation" and add "Or every" : "Phone" => When allocating will check that the allocated object only needs to match 1 of 2 information (Visitor ID or Phone), it will not allocate new code.

### Data Hub - Add Computation Schedule for the Computed Attribute

<figure><img src="../../.gitbook/assets/image (859).png" alt=""><figcaption></figcaption></figure>

### Data Hub - Support auto suggestion for attributes whose datatype is array

<figure><img src="../../.gitbook/assets/image (1544).png" alt=""><figcaption></figcaption></figure>

### Marketing Hub - Customer Journey - Move the "Quick test" button to be on the same line as variant name

<figure><img src="../../.gitbook/assets/image (2303).png" alt=""><figcaption></figcaption></figure>

### Send Journey ID, Campaign ID, Variant ID when tracking "Submit Lead" event

<figure><img src="../../.gitbook/assets/image (2360).png" alt=""><figcaption></figcaption></figure>

### Email template (beta) & Media template - Add display format for Date field

<figure><img src="../../.gitbook/assets/image (403).png" alt=""><figcaption></figcaption></figure>

### Media template - Improve "Distance" algorithm

* Add the operator: greater than in range, greater than or equal in range, less than in range, less than or equal in range, absolute distance in range
* When selecting these operators will display 2 value lines to enter min and max values. It is not required that 2 lines must be the same value or the same %

<figure><img src="../../.gitbook/assets/image (2061).png" alt=""><figcaption></figcaption></figure>

### Email template - Media template - Change default appearance of pop up Filter in BO Setting

<figure><img src="../../.gitbook/assets/image (811).png" alt=""><figcaption></figcaption></figure>

### Email template (beta) - Add the "subject" & "send as" default

<figure><img src="../../.gitbook/assets/image (2320).png" alt=""><figcaption></figcaption></figure>

### All listing - Export - The default is csv instead of excel

<figure><img src="../../.gitbook/assets/image (1875).png" alt=""><figcaption></figcaption></figure>

### Add "Select all" feature for search results

<figure><img src="../../.gitbook/assets/image (2156).png" alt=""><figcaption></figcaption></figure>

### Marketing Hub - Add "Messenger" Destination

<figure><img src="../../.gitbook/assets/image (1454).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (567).png" alt=""><figcaption></figcaption></figure>

### Dataflows - Datasource - Add "Facebook Messenger" connector

<figure><img src="../../.gitbook/assets/image (2590).png" alt=""><figcaption></figcaption></figure>

### Marketing Hub - Add "Telerivet" Destination

<figure><img src="../../.gitbook/assets/image (513).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (1201).png" alt=""><figcaption></figcaption></figure>

### Marketing Hub - Add "Klasik SMS" Destination

<figure><img src="../../.gitbook/assets/image (564).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (1058).png" alt=""><figcaption></figcaption></figure>

### Marketing Hub - Add "Firebase Cloud Messaging" Destination

<figure><img src="../../.gitbook/assets/image (1537).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (487).png" alt=""><figcaption></figcaption></figure>

### Remove required for Phone and Email fields in Caresoft Destination

<figure><img src="../../.gitbook/assets/image (1038).png" alt=""><figcaption></figcaption></figure>

### Email template (beta) - Integrate new email templates into Journey

<figure><img src="../../.gitbook/assets/image (1488).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (1286).png" alt=""><figcaption></figcaption></figure>

### MediaTemplate - Add "UTM tracking" setting

<figure><img src="../../.gitbook/assets/image (565).png" alt=""><figcaption></figcaption></figure>

### Marketing Hub - Add "SMS LACHONG MEDIA" destination

<figure><img src="../../.gitbook/assets/image (2068).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (2067).png" alt=""><figcaption></figcaption></figure>

### Dataflows - Datasource - Add "CDP 365 Segment's Members" connector

<figure><img src="../../.gitbook/assets/image (1484).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (2278).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (738).png" alt=""><figcaption></figcaption></figure>

### Marketing Hub - Promotion pool - Add Journey ID, Variant name, Campaign name

<figure><img src="../../.gitbook/assets/image (1950).png" alt=""><figcaption></figcaption></figure>



### Marketing Hub - Promotion code - Update status flow of Promotion code

* Promotion code status
  * Available: promotion code has not been allocated to the campaign
  * Allocated: The promotion code has been allocated to the campaign, but the campaign has not confirmed that the code has been sent
  * Sent: The promotion code has been allocated to the campaign, and the campaign confirms that the code has been sent
  * Used: The promotion code has already been used by the user
* Promotion code info - delivery status
  * Sent: Campaign has been sent but has not received a successful response
  * Delivered: Campaign sent and received a successful response
  * Fail: Campaign sent and received a response sent failed
* **NOTE: When resend code, update delivery status, do not change status code**

### Marketing Hub - Improve UI Include/ Exclude Audiences interface and Is member of filter interface

* Remove drag & drop icon
* Add Members infomation

<figure><img src="../../.gitbook/assets/image (2087).png" alt=""><figcaption></figcaption></figure>

### Marketing Hub - Improve UI to Promotion Code Detail

<figure><img src="../../.gitbook/assets/image (2219).png" alt=""><figcaption></figcaption></figure>

### Marketing Hub - Destination - Support Enter character when entering Content in some Variant sending message

<figure><img src="../../.gitbook/assets/image (1433).png" alt=""><figcaption></figcaption></figure>
