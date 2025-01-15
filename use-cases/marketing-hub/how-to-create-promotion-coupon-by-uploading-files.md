# How to create "Promotion"/"Coupon" by uploading files?

&#x20;1\. Log into the **CDP 365** system. After logging in, look at the menu on the left hand side.

&#x20;2\. Hover your mouse over **Content** → Choose **Coupons**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfl_g0gc72qDEB1FXNa571efZBKQGXy2Qc92yEMFrcx84Gt0NdU-ZfQ08U1XJzud4nUxBEOJgVBMel7ELdYn6s6NqvZBULX0k6Ze-ChtjDNW5TDDx1elrMjuIyus_KO5uUtQMvSePBN8rXKDzC0fv2uhoU8?key=LMlVAWJnPLCnQdmRxsDSnw" alt=""><figcaption></figcaption></figure>

&#x20;3\. Click **+** button

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcfgF2brRR8uX0RZw6TVdzl7GnfzP8b8reqCVfVZzmL8qafmQfAG9_cB7oGrTU-N5qdZaR2667IaHT-eUJKNdQkJrwL4x8zIU5819OluYCsBQB4hhA6SjjEUpWUmY0Kk1tqa3-8aFwniJWi1lnAi0b49VE?key=LMlVAWJnPLCnQdmRxsDSnw" alt=""><figcaption></figcaption></figure>

&#x20;4\. Fill promotion pool info

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXemKjWcBb2FzAQJdCypwtFZ0-yWSlsX-6hGtot-xjs1H57D6B0CoK4geiqq8Y8jq_qxg1337wawnHPwzvl_vITZgvl4OmgKh-SmKVEIdlf3V_Y8fzNixhLVgbtZgMl7Nnt-4q9MGuuvyoFgZ2RpajDIbrAn?key=LMlVAWJnPLCnQdmRxsDSnw" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="80">No</th><th width="273">Field</th><th>Description</th></tr></thead><tbody><tr><td>1</td><td>Pool name</td><td>Name of pool</td></tr><tr><td>2</td><td>Pool code snippet</td><td>Internal name of the pool, used by the campaign when there is a need to use this pool's promotion codes</td></tr><tr><td>3</td><td>Describe your pool</td><td>User's description of pool</td></tr><tr><td>4</td><td>Upload your file of promotion codes</td><td><p>To upload codes to the pool as soon as the pool is created, the user needs to install the upload setting information, including: </p><p>  - Step 1: User browses the file containing the promotion codes to import into the pool. </p><p>  - Step 2: User conducts mapping attribute Promotion code to file's column containing promotion codes to upload. </p><p>Note: from the user's uploaded file, only the promotion codes that do not exist in other pools will be considered as valid codes and uploaded to this pool, otherwise, the system will ignore the existing codes and not upload these codes to pool. </p><p>If the user skips the upload settings step, the pool is still created but contains no promotion code. (User can create a pool first and then upload codes to the pool)</p></td></tr><tr><td>5</td><td>Set pool expiration</td><td>Users can choose to install (or not install) information about the expiration date of this pool. When the expiration date is reached, the promotion codes that have not been sent to the end-users of the pool will be blocked, at this time the system will not allow campaigns to send these codes to the end-users. Expiry date setting UI includes choosing Date (select from range Today → Future day only), and selecting Time</td></tr><tr><td>6</td><td>Allocation restriction type</td><td>With 2 options: always allocate a unique code or allocate a new code each time (for each user in a journey)</td></tr><tr><td>7</td><td>Set up alert</td><td><p>Send an alert when one of the following criteria is met: </p><p>  - Remind code expiration before x day(s): is allow checked when Set pool expiration selected option All remaining codes expire on </p><p>  - Remind when less than x code(s) left</p></td></tr></tbody></table>

&#x20;   5\. Click **Save** button

<figure><img src="../../.gitbook/assets/image (3541).png" alt=""><figcaption></figcaption></figure>

&#x20;    Then you will be received success messages as:

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdLKxIzeDQlbTpVABPXbJwRu-F06ZpWLG6cxs8Bt4Sc5WU43aYm95PSaETJAw0uoHrXkGlTFWxlb9PNzpDBPVGgkDITIuLGYPTUqzkuhxHNuMoHEfq4sxHamchUb4Mr_WzXInXY2WYnIqQJOmC-bSjSErN4?key=LMlVAWJnPLCnQdmRxsDSnw" alt=""><figcaption></figcaption></figure>
