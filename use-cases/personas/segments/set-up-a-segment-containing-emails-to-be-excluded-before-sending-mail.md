# Set up a "Segment" containing emails to be excluded before sending mail

### 1. Log into the CDP 365 system.&#x20;

Hover your mouse over **Profiles** on the left hand side menu → Choose **Segments**

<figure><img src="../../../.gitbook/assets/image (3063).png" alt=""><figcaption></figcaption></figure>

### 2. Click + button and select Customer/Visitor Segment

<figure><img src="../../../.gitbook/assets/image (3064).png" alt=""><figcaption></figcaption></figure>

### &#x20;3. Fill in the necessary information for your segment

<figure><img src="../../../.gitbook/assets/image (3065).png" alt=""><figcaption></figcaption></figure>

**Update Segment:**&#x20;

* If the email to be excluded is a fixed data set, you should select "Static segment - no update"
* If the email to be excluded changes over time, you should select "Dynamic Segment - scheduled update"

**"Member input method":** Select "**Matching file"** option, then upload the file containing the email to exclude

<figure><img src="../../../.gitbook/assets/image (3066).png" alt=""><figcaption></figcaption></figure>

Mapping email data in file with email attribute in CDP

<figure><img src="../../../.gitbook/assets/image (3067).png" alt=""><figcaption></figcaption></figure>

Click **Save** button to finish creating a segment containing email to exclude

<figure><img src="../../../.gitbook/assets/image (3068).png" alt=""><figcaption></figcaption></figure>

You can see more here: [How to create segments?](broken-reference)

### 6. Set up a journey to send mail that excludes emails in the segment you created above

Log into CDP 365 system,  hover your mouse over **Marketing** on the left hand side menu.

<figure><img src="../../../.gitbook/assets/image (3069).png" alt=""><figcaption></figcaption></figure>

We have 2 channels that supporting to send:

* Email
* Journey Orchestration

<figure><img src="../../../.gitbook/assets/image (3070).png" alt=""><figcaption></figcaption></figure>

Click **+** button to create a journey.

<figure><img src="../../../.gitbook/assets/image (3071).png" alt=""><figcaption></figcaption></figure>

Choose **Start From Scratch**

<figure><img src="../../../.gitbook/assets/image (3073).png" alt=""><figcaption></figcaption></figure>

Click **+** button, choose the **Scheduled Trigger** node.

<figure><img src="../../../.gitbook/assets/image (3074).png" alt=""><figcaption></figcaption></figure>

Add the segment containing the email to be exclude when sending the mail you created above.

<figure><img src="../../../.gitbook/assets/image (3075).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (3076).png" alt=""><figcaption></figcaption></figure>

Click"**+** button to create the next note, add **Destination** node and select **G Suite Email** destination

<figure><img src="../../../.gitbook/assets/image (3077).png" alt=""><figcaption></figcaption></figure>

Choose **Design from Email Template**

<figure><img src="../../../.gitbook/assets/image (3079).png" alt=""><figcaption></figcaption></figure>



Fill out necessary information

<figure><img src="../../../.gitbook/assets/image (3080).png" alt=""><figcaption></figcaption></figure>

and choose an email template in our **Template Gallery**, or create your own in **My Template**.

<figure><img src="../../../.gitbook/assets/image (3081).png" alt=""><figcaption></figcaption></figure>

Click **Save** button to finish setting journey

<figure><img src="../../../.gitbook/assets/image (3082).png" alt=""><figcaption></figcaption></figure>

After finishing the setting of the Journey, we can **activate** and send email to customer.
