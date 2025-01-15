# Data Views

## INTRODUCE

A data view contains a portion or the entirety of data derived from a data object. Data views are employed when an individual only wishes to share specific data from a data object.

**For example**, let's say account 1 creates a new data object called 'All customer.' Subsequently, account 1 generates a data view containing only those customers whose names start with 'A,' utilizing the data from the 'All customer' data object. Similarly, account A also produces additional data views consisting of customer names starting with 'B,' 'C,' 'D,' etc.

<figure><img src="../../.gitbook/assets/2024-03-13_10-18-34.png" alt=""><figcaption></figcaption></figure>

## DATA VIEW LISTING INTERFACE

* **Owner View \[1]**: display data views created by user or other accounts (if user has **View everything** permission toward **Data Views** menu)
* **Shared with me \[2]**: display data views shared by other accounts

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcosFqwHYPPulhAM25gif8sA1DKG0cFQAMVDFY2A_WbprRN4w0gBb82b2qGQ1ZyimnlGPqzuSzPhqNoKMXVcUlCWLVhPYaUGHJlL25hcJm1uny9XD8-FOFcz0pzdAGu4KYNZGN1TOQyh9o3keOkuqdGgtsv?key=BCSPTaQMmpd0_7NM9VMNCw" alt=""><figcaption></figcaption></figure>

## CREATE A NEW DATA VIEW

Click ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcBJSZM0XF7WSwaiD_y7BFUoh5kz7Qcv18jWDwYaQNPAMUEFulptogkASeV15fwm2HjKWZ55GaDXp4sejOCfwTJrBizQBwihB6J5DF_Pn9s7t7lOkErZPBTYQnlBiHEg602RGw7DpC8ZsFUUkuhqnJdGzk?key=BCSPTaQMmpd0_7NM9VMNCw) to generate a new data view.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdt7f7Q9L3t3m0A-HXsOpZKQPviiuhdlHjxwaIr2pefnaZzOGIsJ4LkdjRRPWf9qf1-8tCnchGUf3_S6-kPUnpk6bVraolGie2GbdpaojsRysRds6eYigrdr1i1vJK7ZBX1kuCcfcn00Fcj4qa1f8PcamiG?key=BCSPTaQMmpd0_7NM9VMNCw" alt=""><figcaption></figcaption></figure>

Afterwards, you need to input some necessary information:

* **Name of the data view**: insert a unique name for your data view
* **Description**: describe your data view if desired
* **Based On Data Object**: a data view gets data from a data object. Therefore, you have to choose a data object (popup \[1] only includes data objects you have permission to) for creating a new data view

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeKLZGVljtsd8zuI5oFiuCezub92H1dsyYDRKapIM9PeNGfSZTY50O8R74Bv9uk5fZ989wWowluNDtjLNF4Y_BeeOWWo0USHs_C7Wf80FfsoVnh2_5Ifdax2XhlVLUvpK-hjR1ZhHD6smoM5gRIg59z7Fk?key=BCSPTaQMmpd0_7NM9VMNCw" alt=""><figcaption></figcaption></figure>

### Row access

**Row access** feature allows users to define conditions by utilizing selected data object attributes. Subsequently, the system will identify data rows that adapt to these conditions. Let's use **OR/AND** logic to define conditions that suit your needs.

Additionally, we provide you with two options: **All rows** and **Specific rows**. With the former option, the system retrieves the entire dataset of the selected data object. As for the latter option, the system will follow the rules you configure.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcyyXz9iTVV-63lLPvR_zxSKtkDUnql2QwyPO2cB0Ztp_IDOeKSkl8hp2eM2G7bTBUkS8er_Kja8EKXPpqQhw0qmF-lC6IggYmCOh2wVIc7xZhL7eGg8fNlkzr1XWqUAy6G1VkY_xW_Yib3GqoiesX0EDg?key=BCSPTaQMmpd0_7NM9VMNCw" alt=""><figcaption></figcaption></figure>

### Column access

A data object consists of a wide range of attributes. Therefore, when creating a new data view based on a data object, you need to choose the attributes you want to use for your data view. **Please note that we always require two attributes: ID and Name**. For other attributes, you can rename them to suit your needs.

Similar to **Row access**, we offer two options: **All columns** and **Specific columns**. With **All columns**, the system will include all available columns of the selected data object, while for the **Specific columns** option, only the columns selected by the user will be applied.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd406hrRvP_V2_LpH703UREer0Y-cBUU9Ikx5tPkXeQhK75IK4naYg0mjmKS-YE8s4S8izkYYRAwJKUTNY5Ee5vL9onB_0dusD2LyQB8S9AMTKr0ETNWmF5uuuHiY15pJwfoMgDwt5bd_1xKt907gSJL5U?key=BCSPTaQMmpd0_7NM9VMNCw" alt=""><figcaption></figcaption></figure>

### Share access

This feature enables users to share a data view with other accounts.

**Add people**: enter email addresses of accounts you want to invite.

**People with access**: display accounts you invited

* **Viewer**: allows only viewing of the data view and prohibits any modifications
* **Editor**: permits modifications to the configuration of the data view
* **Transfer ownership**: if you wish to change the owner of a data view, you can use this option. Please note that the 'Transfer ownership' option is displayed in the configuration of a data view only if you are the creator of it
* **Remove access**: allows for the deletion of added accounts

<table><thead><tr><th width="518">Permission</th><th width="118" align="center">Viewer</th><th align="center">Editor</th></tr></thead><tbody><tr><td>Search/ filter/ modify column data table</td><td align="center">x</td><td align="center">x</td></tr><tr><td>Search/ filter/ modify column attribute</td><td align="center">x</td><td align="center">x</td></tr><tr><td>View attribute computation histories</td><td align="center">x</td><td align="center">x</td></tr><tr><td>View configuration of existing attribute</td><td align="center">x</td><td align="center">x</td></tr><tr><td>Action toward attribute (change status)</td><td align="center">x</td><td align="center">x</td></tr><tr><td>View configuration of data view</td><td align="center">x</td><td align="center">x</td></tr><tr><td>Modify configuration of data view</td><td align="center">-</td><td align="center">x</td></tr><tr><td>Use data view for segmentation</td><td align="center">x</td><td align="center">x</td></tr><tr><td>Use data view at 'Customer' &#x26; 'Visitor' menu</td><td align="center">x</td><td align="center">x</td></tr></tbody></table>

**General access**

* **Restricted**: share your data view only with accounts added to **People with access**
* **Public**: allows you to share your data view with all accounts

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXffMTBOYjQeJoiUt9hdggHYQdDREPqmOSV5GhSFH70sA5BxSdzmCeTUr7BhtAJMXAFS_elP5vNxcfQGVF5UxH51PWJ3P95V8o9KJMtz3FohlhYuLIAq3rSzJbaE4WB8-yNzZgG6frawpiyLJ2jT1vgz_zB1?key=BCSPTaQMmpd0_7NM9VMNCw" alt=""><figcaption></figcaption></figure>

## CHECK YOUR DATA VIEW

**Settings Tab**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcLV7smZseauJfU43zoszqk0j80Ow0NX2D2EjVkccJuj8JbFb9hsjIArm15ccg6aMg6CKiCl-yOtNx3StBormu1pjEafSjEQanTGBTLyw2VLUbm-7ceVb2EieEiDhfHCDHz6mNIc0TsZoPIdn7rNxfemPSo?key=BCSPTaQMmpd0_7NM9VMNCw" alt=""><figcaption></figcaption></figure>

**Data Tab**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXe4TeeqslqdlWLCTQ3BLZwsK9uuthqj6EmAHBfdwRFu5UwL6nbcj1KdqIdyH8J_vPCwpPeI9J7h1KJsMfPPTacfFyskIi9uHsDApRCGmWWAtcGQodMig0gg-FelZtKMhqVmML28H3AgWI6SNIa9YNxXZvlr?key=BCSPTaQMmpd0_7NM9VMNCw" alt=""><figcaption></figcaption></figure>

**Attributes Tab**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdeV8qQpPwN4XbPySJ3rr_ZOLI4gsafpIfe7vuCIzbIKf_F4Xr9j9Yuh0IaPqvjqL45AD5N3LTdXODtWsIvL2sD7iRBtM34eLwcxuqPL7yhDMp9aLC0C-FjS4C9sWKSOf0LXqpLJT_MSI1shLdFFJXby0sE?key=BCSPTaQMmpd0_7NM9VMNCw" alt=""><figcaption></figcaption></figure>
