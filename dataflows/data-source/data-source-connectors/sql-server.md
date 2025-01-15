# SQL Server

## Description

Use data on SQL Server as Data Source of CDP 365 by choosing SQL Server Connector. [How to Create datasource](../create-a-data-source.md)

<figure><img src="../../../.gitbook/assets/image (1461).png" alt=""><figcaption></figcaption></figure>

## Connect step

### **1. Database Authentication**

After selecting the connector, SQL Server will display the datasource creation interface as shown below.

<figure><img src="../../../.gitbook/assets/image (992).png" alt=""><figcaption></figcaption></figure>

Authentication information for SQL Server Database includes:&#x20;

* Host Name or IP: host name or IP server. Required.
* Port: Port sever. Number only. Required
* DB name: Database name. Required.
* Username: Username to login. Required.
* Password: Password to login. Required.

Fill out the information completely. Click the Authenticate button to authenticate.&#x20;

### **2. Select access object**

The successful authentication interface is displayed as shown below. Select the object you want to connect to get information. Includes options: Table, View, Custom Query.&#x20;

<figure><img src="../../../.gitbook/assets/image (1680).png" alt=""><figcaption></figcaption></figure>

#### Tables

* Clicking on the table item will show a list of tables that the authentication login account has access to.
* Clicking on the table want to create datasource



<figure><img src="../../../.gitbook/assets/image (1984).png" alt=""><figcaption></figcaption></figure>

#### Views

* Clicking on the View item will show a list of view that the authentication login account has access to.
* Clicking on the table want to create datasource

<figure><img src="../../../.gitbook/assets/image (1564).png" alt=""><figcaption></figcaption></figure>

#### Custom Query

* Use the command to retrieve the desired data set. Only Select statements are allowed. Allow query input note: -- or /\* \*/
* Enter a query to create a dataset.

<figure><img src="../../../.gitbook/assets/image (570).png" alt=""><figcaption></figcaption></figure>

### 3. Click on Connect

After selecting the object, click the connect button to create the datasource
