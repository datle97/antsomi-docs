# January 2024

## FUNCTIONS & FEATURES

* **PERSONAS - Predictive Models -** [**Lifecycle Stage**](january-2024.md#lifecycle-stage)
* **DATA HUB - Events -**[ **Event schema**](january-2024.md#event-schema)
* **MARKETING HUB - Customer Journeys -** [**ZNS message templates**](january-2024.md#zns-message-templates)
* **MARKETING HUB - Blast Campaign -** [**Design from JSON**](january-2024.md#blast-campaign-design-from-json)
* **MARKETING HUB - Smart Inbox -**[ **Expiration time**](january-2024.md#smart-inbox-expiration-time)
* **MARKETING HUB - Email Templates -** [**Email Size Limitation**](january-2024.md#email-size-limitation)
* **MARKETING HUB - Media Templates -**[ **Sync data to Business Object**](january-2024.md#sync-data-to-business-objects)

## DETAILS

### **Lifecycle Stage**

The lifecycle stage model could be implemented on CDP 365 now. It helps users to understand and manage the various stages that a customer goes through in their relationship with a business. It typically includes stages such as awareness, acquisition, onboarding, retention, and advocacy.

<figure><img src="https://lh7-us.googleusercontent.com/Xl_v837rDan-7NPpg21A5WFh37QgaO6KMpS5uDeE6Y1_uXj_mc2qsBVz-q1H5ZcSUS7ytkoRClwy7VNTlEvQUY4d1sQ_vf5V2QNnyLUw2dBgxeCY8f8tCUgJyn8hXSFrAzyJaLS2Mk50NSZTdLFIiR8" alt=""><figcaption><p>Step 2 - Train Model</p></figcaption></figure>

This model is useful for businesses to tailor their interactions and communications with customers based on where they are in the customer journey. For example, in the acquisition phase, companies may focus on building awareness and converting leads, while in the retention phase, efforts might be directed towards keeping customers satisfied and engaged to encourage loyalty.

<figure><img src="https://lh7-us.googleusercontent.com/zNxPt2PCT5nswvCwFRivcnNvRtJy3gw_Fio0DrDJTKONVC7qQPr2fkK64SCqqEETFSfs-GcllHq59FjlJGSSpiJScEB3GC_0NRjNllXTdjZ3woUt6UKyUq_tArXnYSNV6zNocLW-e_pcHMCea6vHRCc" alt=""><figcaption><p>Step 3 - Apply Model</p></figcaption></figure>

By understanding the customer lifecycle, businesses can create targeted and personalized segments & strategies to enhance the overall customer experience and build long-term relationships.&#x20;

### Event Schema

In order to clarify the relations between Business Objects when being assigned to an event and simplify steps taken, the user interface has now been changed and optimized.

<figure><img src="https://lh7-us.googleusercontent.com/KTt_ndZKJz5tukxahVRE8spw_TRkjDGb8RLlT9b6cKNFrsxLEcX_siV8-OgiO4lv4dM7i6XfdrXs_mapncjBRvLRyZMFcZRhh0XZ-GXx6ZvTP5fcekS9A0f24S2jWjmOTzs_TeM0oz24tIZbrgFWBlk" alt=""><figcaption><p>Event schema</p></figcaption></figure>

### **ZNS Message Templates**

To send out a ZNS message is now much easier than before with the list of available templates and required params. Furthermore, the preview part is also visualized to an extent that is closest to the final message.&#x20;

<figure><img src="https://lh7-us.googleusercontent.com/7l3M7DZTx3XFeIldEEv-8Vly0Z_KcVox5r2u4TEk-1eVGBttqGICfB9WkJOVGBaK87nyK1dRSK12pEdNcwzyvB3TgmrHt9Bi6RVRRajmQLAv4ZclFicx3Lw9vLitqpR0Tgry_oxv2VchzRdW8FZw1wk" alt=""><figcaption></figcaption></figure>

### **\[Blast Campaign] - Design from JSON**

Aside from using Media Templates, the users are now able to create their design from JSON to use in Blast Campaign just like the normal one.&#x20;

<figure><img src="https://lh7-us.googleusercontent.com/plpQngSkkt_-io55SGEjJG9u0DVsGpmifTIOnrOvsQJy15guvFW46CGboDOn2-_aj45MhqiAbG-RqNYWevwdf4hxu0bqCnp61FqIE07rftE_WqyrK3_oz4MUzz3VNNaoBE-XHu7PIXsZHRGAQlHMnc4" alt=""><figcaption><p>Design from JSON in Blast Campaign</p></figcaption></figure>

### **\[Smart Inbox] Expiration time**

The feature allows the campaign creator to determine the amount of time that a message would stay alive. After the set time, it would expire and disappear from the notification center. This is perfectly applicable for temporary campaigns.

<figure><img src="https://lh7-us.googleusercontent.com/p1GhqBW57ZcKS6BEB-SoSsdnAJ8VlsXid9QvEQiM6k0TnR_YmpRGoF8VJPSFOURDg84CjRy5vG19eVLg6NAJiq4YefMjtpW75F2G_XfL2Qlz_wM_cTC-dgVZvZT7gHFNhf0QBQgUmHB21Z4b0VAfxa8" alt=""><figcaption></figcaption></figure>

### **Email size limitation**

To optimize the content of an email and prevent the situation of brokening the layout, an alert message will pop out if the size of the current design exceeds 95KB. It gives users a warning so that they could decide to adjust its structure or continue to save the email.

<figure><img src="https://lh7-us.googleusercontent.com/dxXGGAxWz6wrbbnBw5JURVOg08zNyBZFEA6k37wuDgxWx4muKVcyKyZ9bfJD_0aL7f9u6oGgYnxdqotd7L8_iri4n-v8vr4TSRqalhf302fQItWs4Q84tR_KifT-utgmueOzDSPeAalUo_mTA2jlJKc" alt=""><figcaption></figcaption></figure>

### **Sync data to Business Objects**

Aside from syncing lead data to Event and Business Objects which were assigned to Event structure, the users are now able to decide if they want to push the collected data to Visitors or Customers in the desired method. This could adapt with various marketing objectives.

<figure><img src="https://lh7-us.googleusercontent.com/thcYGbLbgeVsi-IF72vKFjBaiHrD31zRl1tijZHtlPyzJCB19nlvtY68tXYVAVvbm-JsT311lTPniX51WwrqeQcADG5SrURPhkSctfIs2TD18S9ILy2JHxSfZKdDP_jx12kEttFzhv2TvDXA8ekSA2s" alt=""><figcaption></figcaption></figure>

## UPCOMING PLAN

Stay tuned for new features to be released next month

* **Article Algorithms -** Recommend the appropriate news&#x20;
* **Line Message Template** - Advanced Imagemap - Determine specific actions on chosen areas in an image
* **Advanced Calendar -** Choose time using calculation & decide its semantic format
* **Media Templates - OTP Verification -** Implement OTP related marketing scenarios
