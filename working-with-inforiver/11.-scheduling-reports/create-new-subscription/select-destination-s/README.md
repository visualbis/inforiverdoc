# Select destination(s)

Here you can select the destination(s) to which you want the send the reports. The scheduled reports can be exported to any of the following destinations: Email, OneDrive, Microsoft Teams, SharePoint, and Google Drive.

<figure><img src="../../../../.gitbook/assets/image (82).png" alt=""><figcaption><p>Destination option</p></figcaption></figure>

{% hint style="info" %}
By default, the email option is chosen in the destinations section.
{% endhint %}

Inforiver provides the capability to export any filters or bookmarks that have been applied to the report, to the chosen destination.

#### **Filter**&#x20;

If this option is set to 'Filter', a new input field becomes available right next to the drop-down. In this field, you can specify the queries to filter the report.&#x20;

{% hint style="info" %}
Hover over the '?' icon to find help links on how to use filter/bookmark
{% endhint %}

<figure><img src="../../../../.gitbook/assets/image (91).png" alt=""><figcaption><p>Tooltip in email destination</p></figcaption></figure>

Click the 'Add new' option to add a new filter/bookmark.

<figure><img src="../../../../.gitbook/assets/add-new.png" alt=""><figcaption><p>Add new link option</p></figcaption></figure>

#### **Bookmark**&#x20;

You can select the bookmark option to include the configured bookmarks in the scheduled reports.

{% hint style="info" %}
The bookmark option is disabled by default and becomes available only if you have added bookmarks to the report
{% endhint %}

A bookmark has been created for the report as shown in the image below.

<figure><img src="../../../../.gitbook/assets/bookmark-addition.png" alt=""><figcaption><p>Adding bookmark to the report</p></figcaption></figure>

The bookmark option will be available if you have added and configured a bookmark in your report.

<figure><img src="../../../../.gitbook/assets/bookmark-option.png" alt=""><figcaption><p>Enable bookmark option</p></figcaption></figure>

Once you select the bookmark option, the second drop-down gets populated with all the configured bookmarks in the report.

<figure><img src="../../../../.gitbook/assets/select-bookmark.png" alt=""><figcaption><p>Select bookmark</p></figcaption></figure>



#### **Bulk Upload**

You can also bulk upload a CSV file containing the filters and bookmarks applied on the report. Click the 'Bulk upload' option. This will open up the bulk upload modal as shown in the image below.

<figure><img src="../../../../.gitbook/assets/image (9) (3).png" alt=""><figcaption><p>Bulk upload option</p></figcaption></figure>

\
Click the 'Upload' button or drag and drop to upload the CSV file with the recipient's details.

The CSV file requires the following details:

1. **Email ID**: Email ID of the recipient of the report if the selected destination is Email.
2. **Filter**: If a filter is applicable, use the format: \<Table name>/\<Field name> eq 'Value'.           Consider a filter applied to select US regions only. If the name of the table is 'Region' and the name of the field is 'Country', the filter value should be <mark style="color:green;">Region/Country eq 'US'.</mark>
3. **Bookmark**: The name of the bookmark, if applied.
4. **Name:** A relevant name for the filter or book applied for destinations like Teams, SharePoint and OneDrive.

{% hint style="info" %}
While uploading, ensure that the csv file used for bulk upload is not open in any application.
{% endhint %}

**Download sample**&#x20;

Click 'Download sample' to download a sample CSV document to understand how the uploaded CSV file should be structured.\
\
The image below displays the structure of the download sample CSV file for Emails:

<figure><img src="../../../../.gitbook/assets/download-sample.png" alt=""><figcaption><p>Download sample csv file</p></figcaption></figure>

The image below displays the structure of the download sample CSV file for OneDrive/Teams/SharePoint:

<figure><img src="../../../../.gitbook/assets/image (10) (1).png" alt=""><figcaption><p>Sample csv file for non-email destinations</p></figcaption></figure>



In the next sections, we'll explore the configuration options for each type of destination.
