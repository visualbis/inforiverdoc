# User management

The user management feature allows you to manage all users and members of your team/organization from a single, easy-to-use dashboard. You can add or remove users, assign user roles, and grant them associated permissions.&#x20;

In addition to default roles, admins can create custom roles and policies to grant users specific permissions for selected features in Inforiver reports.&#x20;

## 1. Overview&#x20;

This page displays a list of all the users in the team. The right side of the page displays a summary of the selected user. By default, your name would be displayed as the first member in the list.

<figure><img src="../../.gitbook/assets/image (932).png" alt=""><figcaption><p>User management dashboard</p></figcaption></figure>

{% hint style="info" %}
The user management feature is available only for the workspace admins within the admin portal.
{% endhint %}

The summary displays the following details:

* **Email** - The email ID of the user.
* **Subscriptions** - Number of subscriptions created by the user.
* **Added by** - The name of the member who added this user.
* **Added at** - The date and the time when the user was added.
* **Last login** - The date and the time when the user last logged in to the console.
* **Role -** This drop-down displays the user's current role, which is dynamically updated based on the option selected.
* **Delete user** - Clicking on this button will [delete the user](./#id-5.-delete-user-or-group).

{% hint style="info" %}
You can add only the maximum limit of users configured for the tenant.
{% endhint %}

This window has the following options to search and filter the user list:

* **Search bar -** In the search bar, you can type any input and the user list will get dynamically filtered based on the entered input. Click 'x' to remove all the entered input.

<figure><img src="../../.gitbook/assets/image (4) (13).png" alt=""><figcaption><p>Search user</p></figcaption></figure>

* **Filter dropdown menus -** You can filter the users based on their roles and the product workspaces they can access. By default, 'All members' for 'All Products' are displayed. You can choose to display specific users based on their role, such as users with the 'Admin' role or users with the 'Members' role. You can also filter based on their product access, such as users with access to Inforiver or EDITable.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Filter by role/product access</p></figcaption></figure>

* **Sort drop-down menu -** This menu allows you to sort users by their names, last login time, or added time. To sort the list, simply choose the desired option from the dropdown menu. Depending on your selection, the user list will be sorted from the latest to the oldest (by last login time/added time) or in descending order (by name). You can reverse the sorting order by clicking the sort arrow next to this menu.
* **Sort arrow -** If the sort arrow is pointing up, the list is sorted in ascending order for the chosen filter in the drop-down. If the sort arrow is pointing down, the list is sorted in descending order. You can toggle the order by clicking on the arrow.

<figure><img src="../../.gitbook/assets/image (5) (13).png" alt=""><figcaption><p>Sort users</p></figcaption></figure>

* **Sort arrows -** You can also use the sorting arrows beside the corresponding header to sort the user list as required.

<figure><img src="../../.gitbook/assets/image (6) (14).png" alt=""><figcaption><p>Sorting arrows</p></figcaption></figure>

## 2. Add member

Click 'Add Member' to add a single member to the application.&#x20;

<figure><img src="../../.gitbook/assets/image (7) (13).png" alt=""><figcaption><p>Add member</p></figcaption></figure>

A pop-up opens as shown. Enter the user's email ID in the textbox provided. You can also use the dropdown menu to select the member.

<figure><img src="../../.gitbook/assets/image (8) (12).png" alt=""><figcaption><p>select the member</p></figcaption></figure>

After entering the email ID, assign their role and click **Add.**

<figure><img src="../../.gitbook/assets/image (9) (10).png" alt=""><figcaption><p>Add member</p></figcaption></figure>

{% hint style="info" %}
You will get a warning message if the given email ID already exists.
{% endhint %}

The user gets added and the below message will be shown.

<figure><img src="../../.gitbook/assets/image (10) (9).png" alt=""><figcaption><p>User added successfully </p></figcaption></figure>

You can choose the 'role' for the added user as either 'member' or 'admin'.

<figure><img src="../../.gitbook/assets/update-member-role.png" alt=""><figcaption><p>Update user role</p></figcaption></figure>

{% hint style="info" %}
Users assigned with an Inforiver Writeback Matrix license from AppSource will get automatically added when they sign-in for the first time.
{% endhint %}

## 3. Bulk upload from CSV

You can choose the 'Bulk upload from CSV' option to add multiple users at a time by uploading the user details in a CSV file.&#x20;

From the 'Bulk upload' drop-down, select the 'From CSV' option.

<figure><img src="../../.gitbook/assets/bulk-upload-from-csv.png" alt=""><figcaption><p>Bulk upload from CSV option</p></figcaption></figure>

In the modal that opens up, click on the 'Upload' button and select the CSV file that you need to upload.

<figure><img src="../../.gitbook/assets/upload-csv.png" alt=""><figcaption><p>Upload CSV button</p></figcaption></figure>

Click the 'Download sample' link to download a sample CSV file and update the user details in the same format given in the downloaded file.

<figure><img src="../../.gitbook/assets/Sam (1).png" alt=""><figcaption><p>Downloaded sample CSV file</p></figcaption></figure>

{% hint style="info" %}
You can also configure the roles of the users as either members or as admins in the CSV file before uploading.
{% endhint %}

Click 'Upload', and upload the CSV file from the file manager in your system.

After the CSV file is uploaded,  click 'Add' in the 'Bulk Upload' modal that displays all the uploaded CSV data.

<figure><img src="../../.gitbook/assets/bulk-upload-option-add.png" alt=""><figcaption><p>Bulk upload add option </p></figcaption></figure>

On successful addition of the users, the users with their corresponding roles get added.

## 4. Bulk upload from AD Group&#x20;

With Inforiver, you can bulk upload from the 'AD Group' to add a group of users at a time without having to manually add or upload a file.

Click the down caret icon in the 'Bulk upload' button on the 'User management' page. From the drop-down select the 'From AD group' option.&#x20;

<figure><img src="../../.gitbook/assets/bulk-upload-from-ad.png" alt=""><figcaption><p>Bulk upload from AD group</p></figcaption></figure>

Clicking on this option will open the 'From AD group' page. By default, no groups are added and the page is displayed as shown below.

<figure><img src="../../.gitbook/assets/ad-group.png" alt=""><figcaption><p>Default screen</p></figcaption></figure>

To add a group, click on the 'Add group' button at the top right corner of the page. This will open up the 'Add group' pop-up.

Enter the group name or select the group name from the drop-down.

<figure><img src="../../.gitbook/assets/add-ad-group.png" alt=""><figcaption><p>Add group modal</p></figcaption></figure>

In the below image, 'Inforiver-Documentation' has been added. Once someone from the group logs in, an account will be created for the user on the user management page with member access to the workspace.

<figure><img src="../../.gitbook/assets/add-ad-group (1).png" alt=""><figcaption><p>Add group button</p></figcaption></figure>

The 'Derived from' field shows the AD group name that the member belongs to.

You can see the following details of the members of the AD group such as the date and time when they are added and their last login details as shown.

<figure><img src="../../.gitbook/assets/ad-member-details.png" alt=""><figcaption><p>AD member details</p></figcaption></figure>

You can delete the added group by clicking on the 'Delete group' button in the top right corner as highlighted in the below image.

<figure><img src="../../.gitbook/assets/delete-ad-group.png" alt=""><figcaption></figcaption></figure>

Clicking on this button will open up a 'Delete group' confirmation modal. Click 'Delete' to confirm the deletion.

<figure><img src="../../.gitbook/assets/delete-ad-group-confirmation.png" alt=""><figcaption></figcaption></figure>

## 5. Delete user or group

The delete option is available only for the users who are manually added through the 'Add member' option or 'bulk uploaded' via CSV file.

Select the user from the list and click 'Delete User'.

<figure><img src="../../.gitbook/assets/delete-user.png" alt=""><figcaption><p>Delete user option</p></figcaption></figure>

A pop-up opens as shown.

<figure><img src="../../.gitbook/assets/delete-user-confirmation.png" alt=""><figcaption><p>Delete user confirmation modal</p></figcaption></figure>

Click 'Remove', to remove the user from the user management page.

{% hint style="info" %}
All the schedules and jobs created by the user will be deleted and cannot be retrieved.
{% endhint %}

The delete option is not available for the users added through the AD group as shown.

<figure><img src="../../.gitbook/assets/no-delete-option.png" alt=""><figcaption><p>No delete option</p></figcaption></figure>

However, you can contact the respective support team and make a request to delete the particular user from the AD Group list.

If any changes/updates are made in the Active Directory AD group, click the 'Sync' button to synchronize or update those changes to the AD group data in the user management dashboard.

<figure><img src="../../.gitbook/assets/sync-data.png" alt=""><figcaption><p>Sync AD group data</p></figcaption></figure>

You can delete the entire group by clicking the 'Delete group' button.

<figure><img src="../../.gitbook/assets/delete-group.png" alt=""><figcaption><p>Delete group option</p></figcaption></figure>

A delete group confirmation modal opens up, click 'Delete' to confirm the deletion.

<figure><img src="../../.gitbook/assets/delete-ad-group-confirmation (2).png" alt=""><figcaption><p>Delete group confirmation modal</p></figcaption></figure>

When an AD group is deleted, then the member accounts associated with that group also get removed from the workspace.

{% hint style="info" %}
The user can belong to more than one AD group and if the user is removed from a group or the entire group is deleted, the user account will not get removed as the user still holds the member permission in the other groups.&#x20;
{% endhint %}

In this section, we covered user management. Navigate to the next section to learn more about [settings](../settings/).
