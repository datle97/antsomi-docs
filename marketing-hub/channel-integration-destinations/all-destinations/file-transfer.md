# File Transfer

In order to prevent the situation that some systems could not bear the high frequency of data sent from CDP 365, File Transfer destination was created.

This type of destination allows users to connect with a third-party storage system to deliver a large amount of data by intervals. This destination will be used in File Transfer channel in Customer Journeys

Hover your mouse over **Settings**, choose **File Transfer**, then click **+** button.

<figure><img src="../../../.gitbook/assets/image (3926).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (3927).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (3929).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="254">Field</th><th>Description</th></tr></thead><tbody><tr><td>Bucket Name</td><td>The name of the Bucket in the Cloud</td></tr><tr><td>Credentials</td><td>The credentials of the Cloud</td></tr><tr><td>File Name</td><td>The name of files which would be sent from CDP 365 to the Cloud. You could set the file name dynamically so the new data would not overwrite the old one by using functions.</td></tr><tr><td>File Format</td><td>The file type you want: tsv, csv</td></tr><tr><td><strong>General Setting</strong><br>Delivery Interval Setting</td><td><p>Choose that the file will be sent after reaching a certain number of records or sent by time period. <br>It provides 4 options:</p><ul><li>Send the file after reaching {x} records<br><img src="../../../.gitbook/assets/image (2127).png" alt=""></li></ul><ul><li>Send the file every {x} day/ week/ month<br><img src="../../../.gitbook/assets/image (1622).png" alt=""></li><li>Send the file after the journey completed</li></ul><p>       <img src="../../../.gitbook/assets/image (1847).png" alt=""></p></td></tr></tbody></table>

