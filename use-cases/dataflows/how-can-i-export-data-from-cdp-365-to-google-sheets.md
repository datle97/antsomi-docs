# How can I export data from CDP 365 to Google Sheets?

## I. Create a new Google Sheets destination

Navigate to the **Destination** menu and click **Create**.

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

After that, select an account that owns the new destination.

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

Find the '**Destination Export Google Sheets**' connector and click **Select** to open the configuration interface.

<figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

Enter your destination name (e.g., 'GG Sheet Destination 1') and click **Authenticate** to connect to your Google account.

<figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

Next, click **Authenticate** at 3rd Party Authentication section.

<figure><img src="../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

The system will open a new tab. Click the **Google Sheets icon** to allow CDP 365 to connect to your Google account.

<figure><img src="../../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

Select an account you want to connect to.

<figure><img src="../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

Click **Continue** to allow Google to share your name, email address, language preference, and profile picture with CDP 365.

<figure><img src="../../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

Click **Continue** to confirm the services that CDP 365 will have access to.

<figure><img src="../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

Choose the sheet you want to receive data from CDP 365 and click **OK** to complete the connection process.

<figure><img src="../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

Finally, click **Save** to confirm the creation of the new destination.

<figure><img src="../../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

## II. Creat a new dataflow

Go to the **Batch Stream** menu and click **Create**.

<figure><img src="../../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

Select an account that is assigned the owner role for the new dataflow. The source list below will update based on the account you selected. Choose a data source that contains data and click **Create stream** to enter the settings interface.

<figure><img src="../../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

Set up the schedule for your dataflow to run automatically.

<figure><img src="../../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

At '**Add data**' node:

* \[1]: select fields you want to access
* \[2]: filter your data by adding conditions

<figure><img src="../../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

After the '**Add Data**' node, use a '**Destination Channel**' node. If you want to export data to Google Sheets, select the **Google Sheet destination** you created earlier.

<figure><img src="../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

At '**Destination channel**' node:

* **Sheet\_id**: select a sheet which will contains your data
* **Mode**: including **Append** and **Overwrite**. Select Append mode if you want the new data to be added after the last row of the selected sheet. Choose Overwrite mode to delete or replace the existing data in the selected sheet
* **Owner**: display the owner of the Google Sheet document

<figure><img src="../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

Click **Review** to preview the data that will be exported.

<figure><img src="../../.gitbook/assets/image (4135).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (4136).png" alt=""><figcaption></figcaption></figure>

Click **Save** to confirm the creation of the new dataflow.

<figure><img src="../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

Click **Activate** to run your dataflow.

<figure><img src="../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

## III. Check the run log of batch streams

**Streaming Log** will display all run logs of batch streams. As a result, you can verify the status of your dataflows here.

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

