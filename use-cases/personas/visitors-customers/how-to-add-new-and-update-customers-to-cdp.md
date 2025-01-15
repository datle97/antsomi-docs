# How to add new and update Customers to CDP

Use case:

You have a file data of Customer (stored as file .xlsx format) - file name is Customer, you want to add new customers (who have not existed ID in the CDP365) and update the information of customers (who existed ID in CDP) into the system&#x20;

<figure><img src="../../../.gitbook/assets/Customer - Excel.png" alt=""><figcaption></figcaption></figure>

## Prerequisites:

A file of Customers (file formats include: .csv, .xls, .xlsx)

### Step 1. Click the Upload icon

Hover your mouse over **Data**, click **Data Objects**.

<img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcIxLtyVmqMJ6w-nK_tcKhYijrOcNzd3XrltKbRGzq8HlyYxdZ_Lj1pvrBZdJjhzzh4Zwr6Wk3kyFR9gP0fXNICULNBLl26jjZiCzxkdcDf5FnccTLVTRjYlkqUVl9A7tXQpytnJjA6OUvdGTTQg9U4QyTV?key=LMlVAWJnPLCnQdmRxsDSnw" alt="" data-size="original">

Then choose **Customer**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdnKfH80iUgReqMn4qbYKUJ9sqAmECwGSzcYnBpcMZ-ZQnsL2oftA0LWKKXoF5dnlBqAoxKNQtaJXHAZz_ebnzjZIHjerunY3_iUu91Eim7l0G1ST_9MifZf-MBUYBHx5arzzfQPFnz4_pgOLs1EOxXx4lB?key=LMlVAWJnPLCnQdmRxsDSnw" alt=""><figcaption></figcaption></figure>

Click **Data** on the left hand side menu and find the **Import** icon on the top left.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfQ4w6bEC2G0VTCe-B28DvkCYIJHO6n1woa6yMNYBx6sPIVKV1asiOLv0L5OtH9ZHrpgbJePU5Argyb2QSjWrNzOdnK-dg18lLCBME48Ho2HxCS8byn3bFLwExTXFf9yHHi01LM6nYps0IHKX76L95Q1pQ?key=LMlVAWJnPLCnQdmRxsDSnw" alt=""><figcaption></figcaption></figure>



Then filling the **Upload settings**.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcBRbpTtud0gK4lLDgv0ckQFsDR1MtgCc5ft6IfDt2Y9Qrtf8orustTfEuI2hiwTZIkpIg2HIpVWH1g4SbH2SlWZPcMP9fJelqHq3E0M9z26wmnP4v1mGo6yBThqjknMj3I3P1NyoEeKjOnWNRveiy2cVWG?key=LMlVAWJnPLCnQdmRxsDSnw" alt=""><figcaption></figcaption></figure>

### Step 2. Click **Browse** in the Upload display

In the **Upload settings**, click **Browse** to select your local file.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd02a0RAs7aQt9AlaVD0xIc_vedGbcb2c4lMTUkgwPAgMN135Ws3hlwtk1dAffijEW2K85iuplIXGcfeh3iAa17u_IyPmA7kByrEKQKitdk2h025j6cCmYHkv_BVCwIQ84MjoeL5Sm_ItS6fJQklpNJ0kh3?key=LMlVAWJnPLCnQdmRxsDSnw" alt=""><figcaption></figcaption></figure>

### Step 3. Select **the file name - Customer** from the Local

Select your local file want to be uploaded to CDP 365, then click **Open**.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXejzh_zvsDSt-LPhvGfDsyvNzAzDL7GSBtYrLb514mZpebKMSypPWh_Xk_4DiM9i2k44s0sZAHFVOtOuVSTeYsW1ELGIsHyqhyqLJYIDZ1qdbiEU30zfeb6rhvNgwnf4GMH5Oy35smCY7RYCXiWEkByrXcH?key=LMlVAWJnPLCnQdmRxsDSnw" alt=""><figcaption></figcaption></figure>

### Step 4. Select the Import type

After selecting the uploaded file, set the **Import type**.

For the Use case, please select the **Add new & Update** type.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcqOLp3DjR-EqC5q_Of48pkl8FLr1a5H-R7ZnW2bIr_RsFx_kXuDEyBywJvS8wndxGGPg-kM__xHiWXiGTxXqZEaaBGMS9dvXMxIfPdFdkrsrG4qrff-4BSKcdy07Xx66b9EPK_4l8nu-_CtqXRKI9_sR51?key=LMlVAWJnPLCnQdmRxsDSnw" alt=""><figcaption></figcaption></figure>

* **Add new & Update**: the type allows importing all data from your local file
* **Add new only**: the type allows importing only **new** data from your local file that is not existing in CDP 365
* **Update only**: the type allows importing data from your local file that is **existing** in CDP 365&#x20;
* **Remove**: the type allows removing data in CDP 365 that exists in your local file

### 5. Select the matching field in **Required and Optional**&#x20;

#### **Required field**

* The **Customer ID (customer\_id)** field matches the **ID** column
* The **Name (name)** field matches the **Name** column

Notes: if your uploaded file doesn't have the ID column, but you have an email address column or phone number column, then use it to map with the customer ID. First, please ensure either the email address or the phone number is the identifier of the customer ID. Second, ensure which hash method is used (MD5 or SHA-256).

For example, if the email address is the identifier of the customer ID and the hash method is MD5, then the mapping should be (image below)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfExoaCnxvQMKhc01kIgg0fgS5S9uiieopRx9Lja1WfH9wImO0MzmJ5xcC_dqrubReZdL1gPGQ30m2p13Iysqt_onHoDg-15vegeQWkeN-pi2HquC1AYpJVSOclmF4G0tDUG2qLVI_SmxihU6WlHgcGiVM?key=LMlVAWJnPLCnQdmRxsDSnw" alt=""><figcaption></figcaption></figure>

#### **Updated field**

* You can map the Customer attributes with the corresponding-value columns of your local file.

For example, you want to update the Email address from your local file into CDP 365 or add more customers in case their data doesn't exist in CDP 365. First, select the Import type: Add new & Update. Second, please follow the mapping of the [Required file](how-to-add-new-and-update-customers-to-cdp.md#required-field). Third, map the Email (email) attribute with the Email column from your local file.&#x20;

Notes: please check the box Allow Null, if some customers in your local file miss the email addresses.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfKYp4qAi7-s9uQSsM0OcurL8pC9KQQD4fpvk7qFwImIa7c8y-mC8LCFQjXnfu1zm6cD2DiCiSU5fMiD9yTW9g7MUtW75OhzgfesMafoKxkZUfjQJ3nzieEjG3OJuk7eHPNiws0FGDPSWtGLYD5kIh_4VQ?key=LMlVAWJnPLCnQdmRxsDSnw" alt=""><figcaption></figcaption></figure>

#### 6. Click **Save** and find the process in Upload **Histories**

Click the Upload Histories to view the upload status

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc-WrNI4LqXMsWIpcjjmjwDwECCV24KEeFQKolmiYUHTX1gK9jKh7ka9CepF7Wk6fvQL7RWgddKV9V2r6-HtTPUWaMC_D1ScUu7Tdhnbgm5oavkFpvBe4IzhDOEbZLxDZ2gp6qGhQJe_JEkoi_6i7wi_32v?key=LMlVAWJnPLCnQdmRxsDSnw" alt=""><figcaption></figcaption></figure>

Or you can go to the **Upload Histories** to view the upload status.

Hover over the **Settings**, click **Upload**, then the **Upload Histories** will be shown on the screen.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfIko32ZWwk5ALBoDgZZ-EXfg7IIburb3ZWkMPrnKwn9DZ9-G9KqdRWpZBsI3QE_RaoFO0Wt39336zHnSqHOaz308ik3m1q7xgZiYIp_TlT85hj6Eh5lJ2sWJiiN383sP43BG5BTO5AOpc_Ymwv6NRYZ_Q?key=LMlVAWJnPLCnQdmRxsDSnw" alt=""><figcaption></figcaption></figure>

Notes: record is a data row of your local file.&#x20;
