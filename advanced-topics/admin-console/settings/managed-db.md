# Managed DB

Inforiver provides a managed Azure SQL database connection for writeback POC purposes. You will be provided with access to the tables created. The administrator can either enable or disable the managed DB connection.

The destination details contain the following information:&#x20;

<figure><img src="../../../.gitbook/assets/manage-db-columns.png" alt=""><figcaption><p>Managed DB columns</p></figcaption></figure>

* **Destination name** - The name of the created database destination. Clicking on any of the destination names will display an overall summary of the destination along with the read only credentials for the table.

<figure><img src="../../../.gitbook/assets/wb-database-summary.png" alt=""><figcaption><p>Managed db destinations summary</p></figcaption></figure>

* **Report name** - The name of the report to which this database destination belongs to
* **Created at** - The date and time at which the database was created
* **Created by** - The name of the user who created it
* **Action** - A 'Trash' to delete the created DB destination. Clicking on this icon will display a confirmation model. Enter the table name of the destination to be deleted in the modal and click 'Confirm' to confirm the deletion.

<figure><img src="../../../.gitbook/assets/delete-destination-confirmation.png" alt=""><figcaption><p>Delete destination confirmation modal</p></figcaption></figure>

The managed DB settings page also has a 'Created by' filter.&#x20;

Clicking on this drop-down will display a list of all the users who have created a database destination and you can easily filter the destinations based on the creator.

<figure><img src="../../../.gitbook/assets/settings-created-by.png" alt=""><figcaption><p>Created by filter</p></figcaption></figure>

Click the 'Reset all' link to clear all the applied filters.

<figure><img src="../../../.gitbook/assets/reset-all-db-filter.png" alt=""><figcaption><p>Rest all filter</p></figcaption></figure>

## Create a ManagedDB destination

To create a new Azure Managed DB destination, Click the 'Writeback' option in the toolbar of your Inforiver report.

<figure><img src="../../../.gitbook/assets/writeback-destination.png" alt=""><figcaption><p>Writeback option</p></figcaption></figure>

If you haven't previously configured any writeback destinations, clicking the writeback option will open up the 'Configure destination' modal. Click 'Continue'.

<figure><img src="../../../.gitbook/assets/configure-destination.png" alt=""><figcaption><p>Configure destination</p></figcaption></figure>

Else if you have already configured the destination, then click the 'Settings' option in the toolbar and navigate to the 'Destination' settings.

<figure><img src="../../../.gitbook/assets/writeback-destination-settings.png" alt=""><figcaption><p>Configure destination from settings</p></figcaption></figure>

Click the 'Manage' link under the destinations tab.

<figure><img src="../../../.gitbook/assets/manage-wb-destination.png" alt=""><figcaption><p>Manage destinations</p></figcaption></figure>

Either of these options will take you to the destinations page. On the destinations, page click on the 'Add new destination' button at the top right corner.&#x20;

<figure><img src="../../../.gitbook/assets/add-new-destination.png" alt=""><figcaption><p>Add new destination button</p></figcaption></figure>

This will open up the 'Add Destination' modal. In the modal, select the 'Azure SQL' option with the managed DB label and click 'Continue'&#x20;

<figure><img src="../../../.gitbook/assets/azure-destination.png" alt=""><figcaption><p>Configure azure SQL destination</p></figcaption></figure>

The 'Terms of service' modal opens up. Click 'Continue' as an acknowledgment of accepting the terms of services.

<figure><img src="../../../.gitbook/assets/accept-tos.png" alt=""><figcaption><p>Accept terms of service</p></figcaption></figure>

On the next page, the 'Connections details' are displayed. Enter your table name in the 'Table name' field and click 'Save destination'&#x20;

<figure><img src="../../../.gitbook/assets/add-new-destination (1).png" alt=""><figcaption></figcaption></figure>

The new destination will get saved and it will also get displayed both on the destinations page as well as in the managed DB settings page.

<figure><img src="../../../.gitbook/assets/inforiver-db-summary.png" alt=""><figcaption><p>Inforiver destination list</p></figcaption></figure>

In this section, we have covered the managed DB settings. Navigate to the next chapter to learn more about the [asset settings](assets.md).
