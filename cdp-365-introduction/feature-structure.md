# Feature Structure

## <img src="../.gitbook/assets/1 (1).png" alt="" data-size="line"> [Personas](broken-reference)

It includes 3 apps: Visitors, Customers, Segments, and Plannings.&#x20;

The module portrays a 365-degree picture of an audience from data pulled from first parties. The pictures based on types of audiences are classified into 2 types: Visitor profiles and Customer profiles.

Besides, these audiences could be segmented by complex conditions in the Segments app.&#x20;

<figure><img src="../.gitbook/assets/image (1187).png" alt=""><figcaption><p>Apps of Personas</p></figcaption></figure>

### <img src="../.gitbook/assets/image (2342).png" alt="" data-size="line"> [Visitors](../personas/visitors-and-customers/)

Visitors are a Business Object in CDP 365 that manages the data of visitors.

A visitor is recorded at the moment that they enter a website or an app. By cookies, the Visitor IDs are created, and their interactions on the domain are tracked even anonymously.&#x20;

The interactive behaviors are events, for example, entering pages, viewing products, submitting consultation forms, searching keywords, etc.&#x20;

### <img src="../.gitbook/assets/image (1751).png" alt="" data-size="line"> [Customers](../personas/visitors-and-customers/)

Customers are a Business Object in CDP 365 that manages the data of customers.

A customer profile of a visitor is created, if CDP 365 has an identity attribute of that visitor. The identity attribute is selectable which could be a phone number or an email address.

While a visitor ID has a sole relationship with a customer ID, a customer ID has multiple relationships with visitor IDs in CDP 365.

### <img src="../.gitbook/assets/image (531).png" alt="" data-size="line"> [Segments](../personas/segments.md)

Segments app allows segmenting Visitors or Customers.

A segment is a group of audiences created by methods that could be simple or complex. Each method allows combining data inside or outside of CDP 365. Based on the types of audiences, segments are classified into Customer and Visitor ones.&#x20;

If aiming to send congrats emails to customers who have birthdays in a month or targeting visitors who have viewed a specific product item more than two times per week, create segments based on those constraints in the Segments app.

### <img src="https://c0-platform.ants.tech/images/2022/11/30/yacvzdpr5y.png" alt="" data-size="line"> Plannings

Plannings app allows the simulation of a result got from a combination of segments.

Based on audience types, plan is classified into two types: Customer Plan and Visitor Plan.&#x20;

A plan is created by groups that include or exclude other groups. The settings of a group include member input method and segment members which are similar to the settings of segments.

For example, a complex segment targets premium customers who have revenue of at least 1,000 dollars in the year and purchased online only excluding those that are streamed from the telesales.&#x20;

* If it was built in the Segments app, the forecast of the segment couldn't provide the number of members after excluding the telesales source.&#x20;
* However, Plannings app allows the complex segment built and explored easily.

## <img src="../.gitbook/assets/image (1019).png" alt="" data-size="line"> [Data Hub](broken-reference)

Data Hub module includes 4 apps: Event Sources, Business Objects, Analytic Models, and Data Schema.&#x20;

The module manages the data pushed into CDP 365 from the first parties as well as from uploading directly.&#x20;

These data are pushed into CDP 365 by connections created in Event Sources and managed by objects called Business Objects.

<figure><img src="../.gitbook/assets/image (1460).png" alt=""><figcaption><p>Apps of Data Hub module</p></figcaption></figure>

### <img src="../.gitbook/assets/image (1413).png" alt="" data-size="line"> [Event Sources](../data-hub/event-sources/)

Event Sources module includes 3 subcategories: Event Attributes, Events, and Sources.&#x20;

Sources app manages bridges of data between CDP 365 and the first parties. Events are interactions of the audience and event attributes give these events deep descriptions.

To record the number of products sold in months on a website, for example, connecting that website to CDP 365 in Sources app and defining event purchases for the buying behavior in Events app. Besides, to have insightful reports on the behavior, event attributes are also defined such as the name of the customer who takes the action, the number of items bought, the date of purchase, etc.

<figure><img src="../.gitbook/assets/image (995).png" alt=""><figcaption><p>Subcategories of Event Sources app</p></figcaption></figure>

### <img src="../.gitbook/assets/image (443).png" alt="" data-size="line"> [Business Objects](../data-hub/business-objects/)

Business Objects app includes 3 subcategories: Business Objects, Upload Histories and Export Histories.

Business Objects are objects that represent data stored in CDP 365. The business objects are customers, visitors, products, stores, campaigns or journeys, etc. Depending on specific requirements, these business objects are defined and assigned to manage data.&#x20;

Upload Histories and Export Histories subcategories give information of uploading and exporting data into/from CDP 365.&#x20;

<figure><img src="../.gitbook/assets/image (1794).png" alt=""><figcaption><p>Subcategories of Business Objects app</p></figcaption></figure>

### <img src="../.gitbook/assets/image (1363).png" alt="" data-size="line"> [Analytic Models](../data-hub/analytic-models.md)

<figure><img src="../.gitbook/assets/Analytic Model.png" alt=""><figcaption></figcaption></figure>

The **Analytic Models** feature is a workspace where you can select and process data, then use it in the [Insights](broken-reference)

It allows you to use the stored attribute information to create a customer view or customer/visitor segmentation. Moreover, you can create a number of analytic models to afford the usage demand, it includes 2 types of models: **Event -oriented Model** and **Object-oriented Model**

The **Event-oriented Model** analyzes data that chooses events as the center, while the **Object-oriented Model** analyzes data that chooses the **Business Object** as the center

Each created model will be corresponding with a data source of the [Insights](broken-reference).

### [![](<../.gitbook/assets/image (1699).png>)Data Schema](../data-hub/data-schema.md)

Data Schema gives an overview of Business Objects, Events, and Sources and their attributes in CDP 365. The feature illustrates the relationships between an event and Business Objects filtered by Source.

<figure><img src="../.gitbook/assets/image (1396).png" alt=""><figcaption><p>Data Schema</p></figcaption></figure>

## <img src="../.gitbook/assets/image (1835).png" alt="" data-size="line"> [Marketing Hub](broken-reference)

Marketing Hub module includes apps: Customer Journeys, Destinations, Promotion Center, Media Template, Form, and Email Template.&#x20;

The module manages marketing automation in Customer Journeys app and the output channels of these scenarios in Destination app. It also manages promotion codes in Promotion Center app and manages the designs of marketing messages in the rest apps.

<figure><img src="../.gitbook/assets/image (695).png" alt=""><figcaption><p>Apps of Marketing Hub module</p></figcaption></figure>

### <img src="../.gitbook/assets/image (1541).png" alt="" data-size="line"> [Customer Journeys](../marketing-hub/customer-journeys/)

The app manages marketing automation scenarios that deliver hyper-personalized experiences across multiple channels and devices. It also allows following through different life stages of the customer journey to drive relevant engagements at different times.

<figure><img src="../.gitbook/assets/image (1226).png" alt=""><figcaption><p>Customer Journeys app</p></figcaption></figure>

### <img src="../.gitbook/assets/image (420).png" alt="" data-size="line"> [Destinations](../marketing-hub/channel-integration-destinations/)

The app manages the output channels of marketing automation scenarios such as Email, Web push notification, App push notification, Facebook Messenger, etc.

<figure><img src="../.gitbook/assets/image (2289).png" alt=""><figcaption><p>Destinations app </p></figcaption></figure>

### <img src="../.gitbook/assets/image (1815).png" alt="" data-size="line"> [Promotion Center](../marketing-hub/promotion-center.md)

The app manages promotion codes sent in marketing automation scenarios such as the number of codes, allocation limitation, etc.

<figure><img src="../.gitbook/assets/image (647).png" alt=""><figcaption><p>Promotion Center app</p></figcaption></figure>

### ![](<../.gitbook/assets/image (1748).png>)[Media Template](../marketing-hub/media-template/)

The app manages the types of templates displayed on websites such as inline templates, pop-ups, banners, floating bars, etc.

<figure><img src="../.gitbook/assets/image (538).png" alt=""><figcaption><p>Media Templates app</p></figcaption></figure>

### &#x20;![](<../.gitbook/assets/image (2213).png>)[Email Template](broken-reference)

The app manages templates displayed on email channels.

<figure><img src="../.gitbook/assets/image (853).png" alt=""><figcaption><p>Email Templates app</p></figcaption></figure>

### ![](<../.gitbook/assets/image (1426).png>)[Form](broken-reference)

The app makes data on audiences enriched by collecting information via forms. Besides, it allows monitoring of the performance by metrics such as submission rate, view, etc.

<figure><img src="../.gitbook/assets/image (1721).png" alt=""><figcaption><p>Form app</p></figcaption></figure>

## <img src="../.gitbook/assets/image (2056).png" alt="" data-size="line"> [Insights](broken-reference)

Insights module includes apps: Analysis, Reports, Data Source, and Gallery Template.&#x20;

The module manages results that are data, including querying and processing data in Analysis, reporting built by the business intelligence dashboards with multiple data sources either from CDP 365 or third-party integration such as Google Ads, Facebook Ads, or databases, etc. in Reports.

<figure><img src="../.gitbook/assets/image (1108).png" alt=""><figcaption><p>Insights module</p></figcaption></figure>

### <img src="https://c0-platform.ants.tech/images/2022/01/31/d9bocnz68z.svg" alt="" data-size="line"> Analysis&#x20;

Analysis app includes 3 subcategories: SQL Workspace, Explore, and Schedule Query.&#x20;

The app allows querying and processing data in SQL Workspace and manages the updated activity schedules in Schedule Query. The app also supports reporting on the processed data.

<figure><img src="../.gitbook/assets/image (2532).png" alt=""><figcaption><p>Subcategories of Analysis module</p></figcaption></figure>

### ![](https://c0-platform.ants.tech/images/2021/04/03/ttquf5uer5.svg) Reports

Reports app allows reporting by dashboards of data from third parties or CDP 365.

<figure><img src="../.gitbook/assets/image (2072).png" alt=""><figcaption><p>Reports app</p></figcaption></figure>

### ![](https://c0-platform.ants.tech/images/2021/04/03/mchw5uue95.svg) Data Sources

Data Sources app manages and creates connections between third parties and CDP 365 to get the data that are used in Reports.

<figure><img src="../.gitbook/assets/image (1505).png" alt=""><figcaption><p>Data Sources app</p></figcaption></figure>

### ![](<../.gitbook/assets/image (1906).png>)Gallery Template

The app manages report templates that can be used in Reports app.&#x20;

<figure><img src="../.gitbook/assets/image (1638).png" alt=""><figcaption><p>Gallery Template app</p></figcaption></figure>

## <img src="../.gitbook/assets/image (980).png" alt="" data-size="line"> Dataflows

Dataflows module includes 3 apps: Dataflows, Data Destination, and Data Source.&#x20;

Dataflows module delivers data output to third parties such as Google Sheets, Facebook Ads, or CDP 365.

Dataflows app sets scenarios and output destinations of processed data. Those output destinations are managed in Data Destination app. Data processed in Dataflows app are managed in Data Sources.

<figure><img src="../.gitbook/assets/image (1516).png" alt=""><figcaption><p>Dataflows module</p></figcaption></figure>

## <img src="../.gitbook/assets/image (2162).png" alt="" data-size="line"> Portal Settings

Portal Settings module includes apps: Data Encryption, General Settings, Roles, Accounts, Menus, and Account Sharing.&#x20;

The module manages accounts, their permissions, and the confidentiality of data in CDP 365.

<figure><img src="../.gitbook/assets/image (635).png" alt=""><figcaption><p>Portal Settings module</p></figcaption></figure>

## <img src="../.gitbook/assets/image (2606).png" alt="" data-size="line"> Development

Development module includes 2 apps: My Connectors and Destinations.

<figure><img src="../.gitbook/assets/image (2451).png" alt=""><figcaption><p>Development module</p></figcaption></figure>

## 8.  Ticket Management

This Ticket Management module is for user to raise a request/question related to CDP 365 with ease and will receive quick reply from CDP CS support team.

<figure><img src="../.gitbook/assets/image (1604).png" alt=""><figcaption></figcaption></figure>

*
