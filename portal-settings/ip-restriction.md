# IP Restriction

## I. Introduction

The IP restriction feature allows users to restrict access permissions to the CDP for one or multiple accounts based on their IP address.

By default, if no IP addresses are configured, all accounts are allowed to connect to the CDP.&#x20;

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

## II. Create a new IP address

Navigate to the **IP Restriction** menu and click ![](<../.gitbook/assets/image (1).png>)

In the **Create new IP address** popup:

<table><thead><tr><th>Fields</th><th width="566">Description</th></tr></thead><tbody><tr><td>IP address</td><td>Enter a single IP, an IP range, or multiple IP addresses you want to restrict. For example:<br>- <strong>Single IP</strong>: 192.168.1.1<br>- <strong>IP range</strong>: 192.168.1.1 - 192.168.1.5<br>- <strong>Multiple IP addresses</strong>: 192.168.1.1, 192.168.1.3, 192.168.1.7 - 192.168.1.9</td></tr><tr><td>Description</td><td>Provide your description</td></tr><tr><td>Accounts</td><td>There are two options:<br>- <strong>All accounts</strong>: All accounts must use the IP addresses entered in the IP address field to access CDP 365.<br>- <strong>Specific accounts</strong>: Access restrictions apply only to the accounts specified.</td></tr></tbody></table>

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

**For example**: enter '192.168.1.1' in the IP address field

* Case 1: Select '**Specific accounts**' and add the 'Antsomi Product' account. The 'Antsomi Product' account will only be able to access CDP 365 using the IP address '**192.168.1.1**' If it attempts to connect from any other IP address, access to CDP 365 will be denied.
* Case 2: Select '**All accounts**'. Only the IP address '**192.168.1.1**' is permitted for all accounts to access CDP 365. Any attempt to connect using a different IP address will be denied.

## III. Edit an existing IP address

In the **IP address list**, click on an address to modify its settings.

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

## IV. Request access

CDP 365 will reject your connection if your IP address is not allowed. You can enter a message and click '**Request Access**' The system will then send your message to Super Admins. Additionally, you can click '**Switch Account**' to select an account that is allowed to access.

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>
