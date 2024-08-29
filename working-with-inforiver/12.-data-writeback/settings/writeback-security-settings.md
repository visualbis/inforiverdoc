# Writeback security settings

Inforiver allows both admin-level and user-level security for writebacks. Admin-level settings can be accessed from the Inforiver console. Click on your user profile and select **Inforiver Console**.

<figure><img src="../../../.gitbook/assets/image (742).png" alt=""><figcaption><p>Navigating to Inforiver Console</p></figcaption></figure>

After navigating to the console, go to the **Admin Portal.**

<figure><img src="../../../.gitbook/assets/image (924).png" alt=""><figcaption><p>Accessing admin portal</p></figcaption></figure>

In the admin portal, go to **Settings** and look for the 'Writeback' section, which contains admin-level writeback settings.

<figure><img src="../../../.gitbook/assets/image (925).png" alt=""><figcaption></figcaption></figure>

## **1. Writeback -> Connections Page**

This page lists all writeback destinations configured by all users in your organization using Inforiver. Admin can create new connections, edit existing connections, or delete connections.

If you are working with multiple writeback connections used by multiple reports to write to multiple destinations, you can access these writeback connections effortlessly. Inforiver provides comprehensive filters and search bars to access your connections quickly.

* The _search bar_ narrows down the list based on the full/partial connection name that is keyed in.
* The _Connection Type_ filter can be used to view all the connections to a particular type of destination.
* The _Updated By_ filter can be used to search for connections that a particular user has updated.

<figure><img src="../../../.gitbook/assets/image (744).png" alt=""><figcaption><p>Writeback connections</p></figcaption></figure>

{% hint style="info" %}
Refer to this [page](../../../admin-console/settings/writeback.md#id-1.-connections) to know more on adding and editing writeback connections.
{% endhint %}

### **1.1. Role-based access control for writeback admin connections**

Admins can specify who can access a particular connection by clicking on the pencil icon beside it.

<figure><img src="../../../.gitbook/assets/image (745).png" alt=""><figcaption><p>Edit access control for the connection</p></figcaption></figure>

On the 'Edit Connection' page, the admin can specify the users' email IDs or an Active Directory list of who should have access to this connection.

<figure><img src="../../../.gitbook/assets/1.2.2. rba for connections-2.png" alt=""><figcaption><p>Specify users</p></figcaption></figure>

Only these users can view and connect to this admin connection while configuring a new destination. Other users without access cannot view it in the list of connections, as shown below.

<figure><img src="../../../.gitbook/assets/1.2.3. rba for connections-3.png" alt=""><figcaption><p>list of connections shown while configuring a new destination</p></figcaption></figure>

If a user who created the admin connection has their access revoked, they can still view the connection details in their profile's 'My Connections' tab. However, they cannot connect to it or modify its accessibility.

## **2. Writeback -> Settings Page**

This page allows admins to enable/disable users from creating and configuring specific writeback destination types. Due to data security and confidentiality requirements, organizations would prefer users to export data to destinations created and configured by admins. This setting will allow the admin to achieve that by disabling users from creating certain destination types.

When the toggle button for a particular destination type is disabled, users will only be able to use admin-configured destinations and cannot create their own. The settings configured in the admin console will be applied to the 'Add Destination' page as well. Users will only see the destination types they have permission to add.

<figure><img src="../../../.gitbook/assets/image (746).png" alt=""><figcaption><p>Destination type settings</p></figcaption></figure>

### **2.1. User Access control to manage writeback destinations**

Apart from choosing the allowed destination types a user can configure, admins can also limit the users who can manage writeback destinations. For example, you can let only certain users add, edit, or delete writeback destinations. Other users would be disabled from adding writeback destinations from the visual or the console.&#x20;

This is done by specifying the email IDs of specific users or adding an Active Directory list in the admin console, as shown below, who will be given permission to add writeback destinations.&#x20;

<figure><img src="../../../.gitbook/assets/image (747).png" alt=""><figcaption><p>user access control to add writeback destinations</p></figcaption></figure>

If access is revoked for a user who has previously added a destination, they can still view their added destination but cannot edit or delete it.
