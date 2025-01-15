# How to create Branded domain in Link Management?

If you want the short link included in marketing message has your brand domain, please follow below instructions.

## Step 1: Open Link Management app

In CDP 365, Go to **Content** and choose **Short Link**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd5ChCNeyv8Bx83RvK31pNOPSWhfBHoo1-emOftJIuE7556AuUmr92qXNKvsVZHJj7ePvNTBJRpIsEiPkwT4hKDduyxQL7t6DrEnLsnv_K_QNppr16UmInqpeRzgXzFHY9Km0Z8QF9LgvY4Mifym-wR7j5e?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

## Step 2: Locate Domain Management tab

In the Data table, choose **Default Internal Vendor Account**

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcNkve4T7RBRjZ92RaXzWtQic-JavwOuYoptPWXa9hETfkBvZHJe5k-KQCL8ULWVM_ESmOS1amSZ7vAp3M1ZaVlInxW0rAocg0GXP-X-8yALVFi5XqdNi1zoJMtiqvrFhygHXewgo5um0YT9pORAgOZUyz8?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

## Step 3: Create a new Branded Domain

In Domain Management tab, click on button ![](<../../.gitbook/assets/image (1764).png>) and follow these steps:

1. In the pop up **Add a domain you own**, input your domain on domain textbox.
2. Tick on checkbox “_I understand that this domain will not be used for anything else except for Antsomi Shortlink_”.
3. Click on **Create**.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXesRCGr_YfGTRLE3x1eHAQDHCfgzIYv5e_fzzFOJovdBc28qiK70xt_gTlmb1ubEI7vqVZ2XYaWG8U0t1Md1mJaHUtrszhyUUW2ycvRVZqkpvBcfERBl2KTBFJanT0WNL1xF8qCGVV4Pp9MUNmLL0CmUzN-?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

## Step 4: Add CNAME for your branded domain.

<figure><img src="https://lh4.googleusercontent.com/_fekBjpGgyNAiwtXkN2RVOHrKznh7rgy2SorLJ2dez12KMdRv1DYDvyVx0VH1xqp03O2FlY3A_SuMwMmQDcYWlUO9GJcHANirKwLRmRfayieIAmu558mYNwHjvWcyu_HsN1DTrMo83WiRO0I-mFaekk" alt=""><figcaption></figcaption></figure>

To add A Canonical Name record (a type of resource record in the Domain Name System that maps one domain name to another), follow below steps:

1. Sign in to your domain host&#x20;
2. Go to DNS setting
3. Go to your domain’s DNS records
4. Add a record to your DNS settings, selecting **CNAME** as the record type.
5. Copy the information in column **Domain** in pop up and paste into the **Label/Host field**.
6. Copy the information in column **Canonical Name** and paste into the **Destination/Target field**&#x20;
7. Save your record
8. In the pop up **Branded Domain**, click **Check Now** to check if the CNAME has been successfully added to the DNS settings.

## Step 5: Set up an SSL certificate

There are 2 ways to set up SSL certificate for your branded domain:

1. Use Antsomi SSL certificate: If you choose this option, you will use Antsomi SSL certificate for your branded domain.
2. Upload certificate: If you choose this option, you must upload a certificate for your branded domain. You must input or upload the following information for SSL Certification: **Primary Key, Certificate, CA Root Chain**.

<figure><img src="https://lh3.googleusercontent.com/upLvWqtjyHWginXltJgQqHhvxPB15Cw780gQU0XhP-lrT6ZuWomF--L4hKGtY8_kObthkK6Z9bcgzn8E2cqYGkk5mZKw2ExXLrRTBQoqjEtnN31bDgLHe2LnU3mQ2DTWl9k74J4ambjeD0ukxahXmqA" alt=""><figcaption></figcaption></figure>

## Step 6: Save your branded domain&#x20;

After filling all the information, click ![](<../../.gitbook/assets/image (1763).png>) to complete create branded name

## EXTENSION

To add short links to your message in a Journey, please follow below instructions:

### Step 1: Open your Customer Journey

### Step 2: Choose destination node

### Step 3: In Compose step, click on the Personalization icon, then choose "Add short link" option

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc9ktp-PWKEHi7oeDG0qxUrz-5pOd61ZOsCEODaX2dvoh78EVcLcAFPFjcSOLeyAPbUaWK8JDekFO7MFOzDAKdk2zD6jrPaSynDy5LC3KEtWMob1Ac6poC834BxtaA1dti9dpJ1HG4HMjx6dm5wOsM_IKw?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

### Step 4: Insert the link you want to be shortened in the pop-up, then click Insert

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcfATiLMeiNVNoCuHwOEG7PYaAUNvr9vZ0j2E8kKdF0VbiNgA_ctvkyCm16O_f-tARo2XODwRn86R3H0RiCSbsdv-e1fHBcsiXS7DvGZcW5366CFhOb5CuQ4KKFW47TMtnq1WMNX4aR0rWkVFh1e5mu67k?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

The link will be immediately shortened and appear in the blue tag (Receiver will see this link), you could click **Preview** to see the original link.&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeJ62DDHf73UuTJI7rTJJvxWEDt5hlWU3vXlsZ8_tOZjiuo9L4I4rehQ9SSKhBJsNkX7ilGWs83oZJOS8MZd_IbGzIE0eLhC4GBStBiii-jMcYUacd52goXrBOQX8bmFtbmlxBXgJ4GHeHqkPQTEWvd0NBH?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>

<mark style="background-color:red;">**NOTE**</mark>: Even though the link created here is having ants.ly domain, but if your branded domain was turned on, the link in the message would have your brand domain.&#x20;

For example:

You have marked the domain "antsomi.com" as Primary.&#x20;

* The original link: <mark style="color:blue;">https://www.antsomi.com/2020/07/29/cdp-institute-antsomi-cdp-365-is-a-delivery-cdp/</mark>
* The shortened link: <mark style="color:blue;">https://www.antsomi.com/12543</mark>

So when the message was sent out, even though the tag was "<mark style="background-color:blue;">ants.y/12543</mark>", the link in the message would be the shortened link:  <mark style="color:blue;">https://www.antsomi.com/12543</mark>

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdg9SiaTvh8Wy4EffOdDbVhkY0--f5HynKtLYVWcSejqbOzFqK9WgnLCPLQ7YOJnj6dG0TyCob4KNeyxhhZ5L73qP_dFy1jnGYFuMypHKKPW4nNBqgRuUJTiZrs8uEChxQQ62rD7sPwaPFhT5HhMKMsgDc?key=jqlrLHcQRq84j2mU-bHqrw" alt=""><figcaption></figcaption></figure>
