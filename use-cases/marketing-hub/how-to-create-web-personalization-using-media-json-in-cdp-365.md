# How to create Web Personalization using Media JSON in CDP 365?

## STEP 1: Create a Customer Journey

### **1. Go to Marketing Hub --> Choose Customer Journey**

<figure><img src="https://lh3.googleusercontent.com/AKyzsSg8Zed61ggFli3aTSy73xtMNgxQ_-bktNkNSgQF1UTRYuJL2I5J9Z-Bv1zSJLRkp8FnTNeZ017GHaHb80BD3qXOJhKT4gLS__ctjCxYddOHK2n-ljpvkSd7LVaM8n4M-RPnmTkWQo3mi5rXUoM" alt=""><figcaption></figcaption></figure>

### **2. Choose Web Personalization channel --> Click** <img src="https://lh3.googleusercontent.com/d2hhiuCUlbLl5QsP3AjYNiS-veGGRsdkrWkMaFMacnTdh4KYFHueAO0XRVUMqMNDbbbtoAfbDJMdQLSsfGqAADvc9hvfH_HkJ8nyX1HoxOJh52FAJws9_Q1nkL9LNtqnATi5VvtCtc5Fc4Lkecsld8U" alt="" data-size="line">&#x20;

<figure><img src="https://lh5.googleusercontent.com/EH_aAjsaJGGNnh6rfP3iX9zPMzqib6TEIuP4pZjOzef9OW4lfHbFRvQE-io4OrGXhvrmUA6PrGuTtxDh30MdnwbTmG-2llxT2yxHPSo9kvRUJYaSUQPkpaEKTNo055uRBVdoEoAJIKySPvMj8dyjkTk" alt=""><figcaption></figcaption></figure>

### **3. Setup Action-based Trigger**

Choose the Event and Source you want

<figure><img src="https://lh6.googleusercontent.com/gytAlknKvuK97-bIvdhZIbIrnLG5ZDBm8DGCsc4YLmjcx15HpTY97xLmdf56esfyIi7aaTwuuq_XdLqdRqODopWOhty9-yG-k5kGoZ8mW8y-no_btC8Pcj4FP3jLzagCUb35WjUikwWdTmyTDMx41oo" alt=""><figcaption></figcaption></figure>

### **4. Setup Destination node**

* Click on Web Embedded node --> Choose Design from JSON

<figure><img src="https://lh3.googleusercontent.com/lI-NuWMLLNmkVMhToDKueJsdMV8ieK9jjyI061n8zGrywndE3lVSBaAGUcbd1csqA7EjzMBrAXxC3lu_14J5UfjQgGVok3NSWm7bN6JH8vsN-1OJBIttzegTUPXjPnBdhC0RVnI9ocRRcrA28hBFo1g" alt=""><figcaption></figcaption></figure>

* Input neccessary information for campaign

<figure><img src="https://lh6.googleusercontent.com/irhYC8IOlwiYSIgK4G5OuukFtxzVw_zSEP6yvhH9BzlV09XQT6GiPiRMU7Iyae0shne9fidyLFEvMVpXMXXXlvHhG-PIR9_RoS9gHOlXQdXLuB4xk7vNijb0v85plx7OPtQklcBFphlwFmtNAywrZ3k" alt=""><figcaption></figcaption></figure>

* Go to step 2: Compose --> Click Blank Template

<figure><img src="https://lh6.googleusercontent.com/2e-hY7eJs_TXTuU-EKthbDR7aehAjsi4_Xb_To6xBjswhHEpGm_CTXcOMDeMdVmpPm9-arkuPKW0HMda7DUnrwAaP_ikAaGc3Il9umvcjzzMleheDGhffRyhNhufvGEVVbhqaVZJs-vw44oj-HY76OY" alt=""><figcaption></figcaption></figure>

* Design the media by drag and drop blocks in to the left area. To see details of each block, [click here.](../../marketing-hub/customer-journeys/work-with-journey/destination-nodes/web-embedded/design-from-json/setting/blocks-and-settings/)

<figure><img src="https://lh5.googleusercontent.com/pSwrhMIzOTpCGsZ6-zrmwl82Nj40usO59vCUkTTGdgbdaEHKBDWsbR90RBIn7vIu878D3LXXzW8oz6JXbnCQtpW_K1ytAYcgwbzU7ClEyrv9cK3lUaKZzQpfs8dQOUPX5HTqwskXA7-NBwSx7E2Kj28" alt=""><figcaption></figcaption></figure>

* Click Apply

<figure><img src="https://lh6.googleusercontent.com/Gz-P-oLe0HL161CEbwBwrZmPdCrVyRy2vK36mJONNu4wVQrEQ-1IkxS3nOJOnI2jRun1dvIDpApZwdFWIPmoTRg_Mt0VxGGZKeWs-gWQZHu47YVEmKffipm9UmpkhDOI_-FqNtfrXZZIrvLatNz-hds" alt=""><figcaption></figcaption></figure>

### 5. Save & Activate the journey

* Click "Save change" to save the journey
* Click "Activate" to start running the journey

<figure><img src="https://lh5.googleusercontent.com/BCon1DPx5oVUt5fYN6ow4sQVuxvieA_QpDe63KkZYxzKdQomAiviY3xeSz5YZ6Jo_Lu2IBBIwbwfH_1VY0Ln_OaItD_IFLoVBY8gph-TEQjc0cgYuYX_CsD2DFFZRORjzLzKCXqBr_hYolbggQ1J4Ug" alt=""><figcaption></figcaption></figure>

## STEP 2: Verify the data

After the Journey has successfully run, go to your website to check the data.

### **1. Inspect your website**

* Click the right mouse --> choose Inspect in the pop-up or press F12 on your keyboard

### **2. Find the event**

In tab Network, enter keyword in to search box:

* Delivery or code of the event chosen in Action-based trigger node (Ex: Add to cart --> add\_to\_cart)

### 3. Find & check API

* In the list of API, find the API that has the event in Action-based trigger node

<figure><img src="https://lh4.googleusercontent.com/9XWPNizx30S13aZ_cyYyH_gbvbReGPXhLhN6qlZZ9r3bTllwc1DeJy_BlDNsmMgFV4ri7KvCgFuZOFrcso1PhZVirJHxtntdU4EA6JJ6-JeQ7btXFcyB245I9qt5Ji7ouEOb6bsWDB3ByVWfNtiw10Y" alt=""><figcaption></figcaption></figure>

* Double click on that API --> in the URL, change "v3" into  --> "app"

<figure><img src="https://lh6.googleusercontent.com/KaczTui8PI1x4ZqezbEtyoveg0dxD4MmrKA7IXFHXHuKmTDByNyIutniTUqiCAk5AIiDXqLLiNFEOvEYu5ZYeJmkUGz49HUm5e2eVWqvbCd4Z9RfJDJQumw_ibjeXDQrMjPxCgSjOaJyT76mDFwR-NQ" alt=""><figcaption></figcaption></figure>

NOTE: You can install JSON Formatter to check the data of API

## STEP 3: Get API

After the Journey has successfully run, go to your website to check the data.

### **1. Inspect your website**

* Click the right mouse --> choose Inspect in the pop-up or press F12 on your keyboard

### 2. Find API

* In tab Control, enter function used to build the Media JSON and Enter. [Function detail](https://docs.google.com/document/d/1ksejw2Vjwpll69pL0GEjKPaVb2RWv9-itEJyhF6VuDw/edit?usp=sharing)
* Copy API response and paste in URL, request this API to get data.

<figure><img src="../../.gitbook/assets/image (2013).png" alt=""><figcaption></figcaption></figure>

\
