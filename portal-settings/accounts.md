# Accounts

This app manage the list of portal accounts

<figure><img src="../.gitbook/assets/image (1157).png" alt=""><figcaption></figcaption></figure>

## Create account

* Click create icon <img src="../.gitbook/assets/image (2198).png" alt="" data-size="line">
* Set the configuration&#x20;
  * Email: the email of the account to be created
  * Request verify email: the account is active only when the user verifies via email
  * Full Name: Full name of account
  * Gender: select Male or Female
  * Account type has account and manager account
    * Account is a normal account that has permissions only when manager account grants them
    * Manager account has a primary account that has authority to grant permission to others
* Click SAVE

<figure><img src="../.gitbook/assets/image (1409).png" alt=""><figcaption></figcaption></figure>

## Account Details

Click on Name of account on datagrid will display account detail page.

<figure><img src="../.gitbook/assets/image (2529).png" alt=""><figcaption></figcaption></figure>

There are 3 tab in account detail page: Summary, Permission, Account sharing

### Summary

The summary tab displays basic information of the account.

* Click on button <img src="../.gitbook/assets/image (1223).png" alt="" data-size="original"> to change information.
* Click the Switch button ![](<../.gitbook/assets/image (924).png>) to enable 2-step authentication to secure your account. To know further details, click [here](../cdp-365-introduction/cdp-365s-interface.md#two-step-authentication).

### Permission

Permission tab includes the role in which the account is granted&#x20;

<figure><img src="../.gitbook/assets/image (1609).png" alt=""><figcaption></figcaption></figure>

You can assign permissions to the account by selecting roles or assigning permissions directly by Function Permission&#x20;

#### Roles

<figure><img src="../.gitbook/assets/image (2321).png" alt=""><figcaption></figcaption></figure>

* List Roles: display the list of roles in the [Roles app](general-setting/roles.md). Click on <img src="../.gitbook/assets/image (1246).png" alt="" data-size="original">to select role for account.
* Selected Roles: displays a list of roles assigned to this account. Click on <img src="../.gitbook/assets/image (559).png" alt="" data-size="original">to remove selected roles.

![](<../.gitbook/assets/image (512).png>)

* Click on Dropdown in role will show options to choose permission&#x20;
  * Permission Only: only have view/edit permission on the menu by role
  * Grant Permission Only: You can only assign view/edit permissions on the menu by role to another account
  * Both: have permission and grand permission on menu by role.

{% hint style="info" %}
Super Admin: This is the role that has permission to everything on all menus on the portal.

Public: By default, when a new account is created, it will have the Public role. That account will have view rights on some menus.
{% endhint %}

#### Function Permission

Displays a list of menus and the corresponding permissions on that menu.

<figure><img src="../.gitbook/assets/image (1192).png" alt=""><figcaption></figcaption></figure>

The table contains the following columns:

* Menu: List of menu in poral
* Roles: roles to which this account is assigned
*   Permission: Account permissions on the menu. There are two permission: View and Edit.

    * Click on dropdown list View will show options:
      * None: user can't see this menu.
      * Created by user: account only can view data created by themselves
      * Management by user: account can view data of accounts managed by this account
      * {Permission}(via Role): view permission is granted by role
      * Everything: Account can see all data in this menu.



    <figure><img src="../.gitbook/assets/image (1103).png" alt=""><figcaption></figcaption></figure>
* Click on dropdown list Edit will show options:
* Everything: Account can edit all data in this menu. This option only display when View select Every thing.
* Management by user: account can edit data of accounts managed by this account. This option only display when View select Every thing and Management by user
* Created by user: account only can edit data created by themselves. This option only display when View select Every thing, Management by user or Created by user.
* None: account can't edit in menu. This option display when View select Everything, Management by user, Created by user or None.
* {Permission} (via Role): permission is granted by role

<figure><img src="../.gitbook/assets/image (898).png" alt=""><figcaption></figcaption></figure>

### Account Sharing

Account sharing tab manages the emails which have the right to use this account

<figure><img src="../.gitbook/assets/image (1284).png" alt=""><figcaption></figcaption></figure>

* Click on <img src="../.gitbook/assets/image (1626).png" alt="" data-size="line"> to add account access

<figure><img src="../.gitbook/assets/image (855).png" alt=""><figcaption></figcaption></figure>

After clicking **+ Users** will show the **INVITE OTHERS TO ACCESS THIS ACCOUNT** section

* App: Select the app that the account access can access.&#x20;
* Email address: Enter the email of the account access. This email must exist in the portal's account list
* Name: name will load by email
* Access level: Includes 2 options:&#x20;
  * Administrative access: Has the same permissions as the main account on the selected app.
  * Read only access: Only view permission as the main account on the selected app

Click on Send invitation to send email to account access

