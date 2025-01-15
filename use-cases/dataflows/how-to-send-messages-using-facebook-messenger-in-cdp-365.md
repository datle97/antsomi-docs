# How to send messages using "Facebook Messenger" in CDP 365

In order to send messages through Faceboook Messenger, you should follow the instructions below:

1. Create a Data Source - Facebook Messenger&#x20;
2. Create a Data Destination - CDP Business Object
3. Create a Dataflow (To push data from Facebook Page to CDP 365)
4. Create a Segment of Visitor
5. Create a Destination (Facebook Messenger)
6. Create a Customer Journey (To send messages via Facebook Messenger)



DETAILED INSTRUCTION

## STEP 1 - Create Facebook Messenger data source <a href="#i.-create-a-new-data-source-to-get-the-list-of-users-who-have-sent-messages-to-your-page" id="i.-create-a-new-data-source-to-get-the-list-of-users-who-have-sent-messages-to-your-page"></a>

This step is to take the data of users who sent messages to your Facebook Page

### 1.  Access the "DATAFLOWS" app and go to the "Data Source" menu <a href="#id-1.-access-the-dataflows-app-and-go-to-the-data-source-menu" id="id-1.-access-the-dataflows-app-and-go-to-the-data-source-menu"></a>

<figure><img src="https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FUeKUuVd9H6Qacei9gBw0%2Fimage.png?alt=media&#x26;token=a028f24a-f7ad-4339-9c17-e396294a8551" alt=""><figcaption></figcaption></figure>

### 2. Click ![](<../../.gitbook/assets/image (1630).png>) to create new a Data source <a href="#id-2.-click--to-create-new-a-data-source" id="id-2.-click--to-create-new-a-data-source"></a>

<figure><img src="https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FbMebD2Hh3fnFho1nu0xB%2Fimage.png?alt=media&#x26;token=a023408a-631b-4783-ac6c-55c497dc0ae3" alt=""><figcaption></figcaption></figure>

### 3. Select "Facebook Messenger" connector <a href="#id-3.-select-facebook-page-connector" id="id-3.-select-facebook-page-connector"></a>

<figure><img src="../../.gitbook/assets/image (1911).png" alt=""><figcaption></figcaption></figure>

### 4. Login your Facebook account <a href="#id-4.-login-your-facebook-account" id="id-4.-login-your-facebook-account"></a>

<figure><img src="../../.gitbook/assets/image (894).png" alt=""><figcaption></figcaption></figure>

### 5. Select the page that you want & click Connect <a href="#id-5.-select-the-page-that-you-want" id="id-5.-select-the-page-that-you-want"></a>

<figure><img src="../../.gitbook/assets/image (2268).png" alt=""><figcaption></figcaption></figure>

#### 6. Choose fields & Click Apply <a href="#id-7.-click-apply-button-to-finish-creating-data-source" id="id-7.-click-apply-button-to-finish-creating-data-source"></a>

* After clicking Connect, a pop-up is shown to let you select the fields you want to take the data
* Click apply so save your selection and save the Data Source

<figure><img src="../../.gitbook/assets/image (749).png" alt=""><figcaption></figcaption></figure>

## STEP 2 - Create a Data Destination

This step is to&#x20;

## STEP 3 - Create a Data Flow <a href="#ii.-set-up-dataflow-to-push-facebook-user-id-data-to-visitor-business-object-in-the-cdp-system" id="ii.-set-up-dataflow-to-push-facebook-user-id-data-to-visitor-business-object-in-the-cdp-system"></a>

### 1. Access the "DATAFLOWS" app and go to the "Dataflows" menu <a href="#id-1.-access-the-dataflows-app-and-go-to-the-dataflows-menu" id="id-1.-access-the-dataflows-app-and-go-to-the-dataflows-menu"></a>

<figure><img src="https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2Fx2fs6NH4qLYZR9pr1mV3%2Fimage.png?alt=media&#x26;token=8915dcf8-9723-4ec7-8885-b0f10e86040f" alt=""><figcaption></figcaption></figure>

### 2. Click _+ Blank Dataflow_ <a href="#id-2.-click--blank-dataflow" id="id-2.-click--blank-dataflow"></a>

<figure><img src="../../.gitbook/assets/image (1853).png" alt=""><figcaption></figcaption></figure>

### 3. Select Data Source  <a href="#id-3.-select-the-facebook-page-data-source-that-you-created-then-click-the-create-dataflow-button" id="id-3.-select-the-facebook-page-data-source-that-you-created-then-click-the-create-dataflow-button"></a>

* Select the data source that you created in [STEP 1](how-to-send-messages-using-facebook-messenger-in-cdp-365.md#i.-create-a-new-data-source-to-get-the-list-of-users-who-have-sent-messages-to-your-page), then click the "Create dataflow" button

<figure><img src="../../.gitbook/assets/image (649).png" alt=""><figcaption></figcaption></figure>

### 4. Configure Add data node <a href="#id-4.-select-the-field-you-want-to-get-the-data" id="id-4.-select-the-field-you-want-to-get-the-data"></a>

* The first node in a data flow is **Add data** node. Here, you can choose which fields you want to get data from.
* Drag the fields on the left box and drop it to ![](<../../.gitbook/assets/image (2560).png>)
* You can preview the data by clicking ![](<../../.gitbook/assets/image (2153).png>)

<figure><img src="https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2Fj3Duu2FHppNBH21LOnKd%2Fimage.png?alt=media&#x26;token=f5e8a6ed-5c62-4310-96d9-aafeb6bdfa04" alt=""><figcaption><p>The configuration of <em>Add data</em> node</p></figcaption></figure>

<mark style="background-color:red;">NOTE:</mark>

* "User ID" is the ID of the Facebook accounts who have sent message to your page
* Facebook only returns a list of User id that have sent message to your page within 24 hours

### 5. Add "Destination channel" node <a href="#id-5.-add-destination-channel-node" id="id-5.-add-destination-channel-node"></a>

<figure><img src="https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2Fun5y1YX95CL7fM8D2ZPA%2Fimage.png?alt=media&#x26;token=99817fd5-eb1e-4e6a-80a2-fcc14984265e" alt=""><figcaption></figcaption></figure>

You can see how to create a destination channel for a Business Object [here](https://docs.antsomi.com/cdp-365-user-guide/quick-start-guide/how-to-create-a-destination-channel-in-dataflows)​Select "Visitor" Business Object, then map facebook's User id with Visitor's User ID on CDP system![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2F8EHCl5acSo9jszzpJQ7i%2Fimage.png?alt=media\&token=41574f70-67b2-4aab-8b62-09a11ad9e3d8)You need to create a "Custom attribute" in the "Visitor" Business Object to know it's the Facebook user ID pushed from the dataflowYou can see how to create a "Custom attribute" [here](https://docs.antsomi.com/cdp-365-user-guide/quick-start-guide/how-to-create-attribute-for-customer-visitors)​For example: Create a Custom attribute of "Is Facebook user\_id" with data type of Number![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FI5wMP3dZCDMuP8HtW2Tn%2Fimage.png?alt=media\&token=f0ebda7b-60bb-420f-b8a5-9d622990777a)

* If the value of this attribute is 1, it is the User ID of Facebook

Set value pushed from dataflow to 1 for this Customer attribute![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2F1clvYgO7CYnx9aoiTs5B%2Fimage.png?alt=media\&token=8fee2779-4949-4d58-ad6e-fe2b9acdd42c)Select write mode is Insert all

#### 6. Save Dataflow <a href="#id-6.-save-dataflow" id="id-6.-save-dataflow"></a>

![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FjD0mMGQHOCJu87FY86Ic%2Fimage.png?alt=media\&token=c9920864-f695-4a96-8d30-dc641a466441)

#### 7. **REVIEW & TURN ON** <a href="#id-7.-review-and-turn-on" id="id-7.-review-and-turn-on"></a>

Used to view setup information in dataflows and setup execution time![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FCpBT9BEbapa0GD93rOZi%2Fimage.png?alt=media\&token=912a4d07-5502-4610-a9f4-f890ad94c4f9)![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2Fz07OgDzR3nNT1I3EZUVM%2Fimage.png?alt=media\&token=aec991a3-cc16-4dee-ba77-f50d1935bd8c)**Force Run:** Used to run immediately without timeout in dataflows![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FRHjWEYyhS8iEx7JwwQHR%2Fimage.png?alt=media\&token=45c8d868-b7e7-4912-b1ed-7fc94c670e54)After the dataflow has finished running, you can go to the Visitor menu in Personas App to check the creation of Facebook User ID in CDP:![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2Fz2Su0aKnYypJYn9ULyMx%2Fimage.png?alt=media\&token=b4e5ed35-432b-47b3-8ed6-f93588356b7a)![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FhjA8YVV7pYvREe2yWJlt%2Fimage.png?alt=media\&token=006a9bc1-12ea-447a-a224-9100a99a2852)

### III. Create a new Visitor Segment to get a list of Facebook User IDs <a href="#iii.-create-a-new-visitor-segment-to-get-a-list-of-facebook-user-ids" id="iii.-create-a-new-visitor-segment-to-get-a-list-of-facebook-user-ids"></a>

The conditions you set in the segment are as follows:![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FFZXgoNGQ2WWY7nr7dewv%2Fimage.png?alt=media\&token=5e3d5500-ebb4-4c49-b497-f6fc1d233183)Note: You can see how to create a new segment [here](https://docs.antsomi.com/cdp-365-user-guide/quick-start-guide/how-to-create-a-new-segment)​

### IV. Create a "Messenger" destination  <a href="#iv.-create-a-messenger-destination" id="iv.-create-a-messenger-destination"></a>

#### 1. Access the "MARKETING HUB" app and go to the "Destinations" menu <a href="#id-1.-access-the-marketing-hub-app-and-go-to-the-destinations-menu" id="id-1.-access-the-marketing-hub-app-and-go-to-the-destinations-menu"></a>

![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FRB7p3czQw62dLyG5fe3a%2Fimage.png?alt=media\&token=5b5e2bce-12fd-4e38-b3ac-de7a6e1d3ebe)

#### 2. Click "+" button and select "Conversation" <a href="#id-2.-click--button-and-select-conversation" id="id-2.-click--button-and-select-conversation"></a>

![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FeXOPnfMcORroQSeQ3yJ4%2Fimage.png?alt=media\&token=35386e34-b079-4df4-b94d-b8122eab9610)

#### 3. Select "Destination catalog": "Messenger" <a href="#id-3.-select-destination-catalog-messenger" id="id-3.-select-destination-catalog-messenger"></a>

![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2F8U6lsMvyIcNQkJ8TgVdF%2Fimage.png?alt=media\&token=039e3ac7-f67a-4b96-9cc7-baedfe254957)

#### 4. Fill in the necessary information for the destination <a href="#id-4.-fill-in-the-necessary-information-for-the-destination" id="id-4.-fill-in-the-necessary-information-for-the-destination"></a>

![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FExXFefswk3vHAr50Qepk%2Fimage.png?alt=media\&token=17167bfa-077e-453a-adfe-f435d9560cd8)

| Field               | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Page scoped user id | User ID Facebook of the recipient of the messageYou can click![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2Fe5GNX79BQkdc2wru0gQr%2Fimage.png?alt=media\&token=bb7a2947-cb86-40bc-b2c8-1be9cd72f634)icon to add Personalization![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FaK2Onn4iUKS7obVPwv6R%2Fimage.png?alt=media\&token=38496508-3116-44d2-b58a-273635687ffb)​![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FCAFOxcD2195HNTP7Cfbw%2Fimage.png?alt=media\&token=f36e874e-6fe2-435b-a68b-37826fbac79f)​ |
| Access token        | Access token of your page on Facebook.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

**Note: Currently, please share your page with us with the following permission: "Send and respond to message as the Page"​**![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2Ffl39rp7WsSm9xY9deaTZ%2Fimage.png?alt=media\&token=f4e82a44-480e-4e5c-a234-6a523ddbd361)**​-> We will help you set up the necessary information in destination​**

#### V. Sending "Messenger" via Customer Journey <a href="#v.-sending-messenger-via-customer-journey" id="v.-sending-messenger-via-customer-journey"></a>

Log into CDP system, access **"MARKETING HUB"** app and go to **"Customer Journeys"** menu![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FVP19xnZV2JvVmId0MRIC%2Fimage.png?alt=media\&token=d9cceea5-710d-45f1-92fc-d01f2e584b3a)We have 2 channels that supporting to send:

* "Conversation"
* "Journey Orchestration"

![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2F8B6y2tmzF1iMkY4PnNry%2Fimage.png?alt=media\&token=1dbf11d5-83fd-4cba-b97e-1dee90e51669)At the "Schedule trigger" node, select the segment containing the Facebook user id that you created![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FxAmhCAzW8VcUaBRtRGr0%2Fimage.png?alt=media\&token=87f42fb9-bb77-4b52-ab69-bd5f77987b5c)Click "+" button to Create Journey, add "Destination" node and select "Messenger" destination![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FZluJCMk5vCyiOqUQYff4%2Fimage.png?alt=media\&token=2da41f6d-be98-440b-940e-f02431a85503)Fill out necessary information![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2FUbpQ2U0OMB2QpFnHMVWd%2Fimage.png?alt=media\&token=317063db-8afd-4d53-b58c-615a4b7b93fe)Click "Save change" button to finish setting journey![](https://2980605795-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FmECwNqMNUmu6OXHSYgDv%2Fuploads%2F0XauWU0JULWsJGs0YYmR%2Fimage.png?alt=media\&token=4b923c50-598a-42f2-887b-dc080a3a4957)After finishing the setting of the Journey, we can activate and send message to customer

##
