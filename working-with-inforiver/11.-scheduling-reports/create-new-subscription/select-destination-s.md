# Select destination(s)

Here you can select the destination(s) to which you want the send the reports. The scheduled reports can be exported to any of the following destinations: Email, OneDrive, Microsoft Teams, SharePoint, and Google Drive.

<figure><img src="../../../.gitbook/assets/image (82).png" alt=""><figcaption><p>Destination option</p></figcaption></figure>

{% hint style="info" %}
By default, the email option is chosen in the destinations section.
{% endhint %}

## i) Email

The following options are available if the email destination is chosen.

The 'To' option has the following fields: Recipients and Filter/bookmark.

### **a) Recipients**&#x20;

Here you can specify the recipient's email address to which the report should be sent. AD groups can also be used.&#x20;

### **b) Filter/bookmark**&#x20;

Here you can specify if you want to apply any filter or bookmark to the report for the selected recipients before exporting it. This value is set to 'None' by default.&#x20;

<figure><img src="../../../.gitbook/assets/recipients-option.png" alt=""><figcaption><p>To field in email destination option</p></figcaption></figure>

#### **Filter**&#x20;

If this option is set to 'Filter', a new input field becomes available right next to the drop-down. In this field, you can specify the queries to filter the report.&#x20;

{% hint style="info" %}
Hover over the '?' icon to find help links on how to use filter/bookmark
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (91).png" alt=""><figcaption><p>Tooltip in email destination</p></figcaption></figure>

Click the 'Add new' option to add a new filter/bookmark.

<figure><img src="../../../.gitbook/assets/add-new.png" alt=""><figcaption><p>Add new link option</p></figcaption></figure>

#### **Bookmark**&#x20;

You can select the bookmark option to include the configured bookmarks in the scheduled reports.

{% hint style="info" %}
The bookmark option is disabled by default and becomes available only if you have added bookmarks to the report
{% endhint %}

A bookmark has been created for the report as shown in the image below.

<figure><img src="../../../.gitbook/assets/bookmark-addition.png" alt=""><figcaption><p>Adding bookmark to the report</p></figcaption></figure>

The bookmark option will be available if you have added and configured a bookmark in your report.

<figure><img src="../../../.gitbook/assets/bookmark-option.png" alt=""><figcaption><p>Enable bookmark option</p></figcaption></figure>

Once you select the bookmark option, the second drop-down gets populated with all the configured bookmarks in the report.

<figure><img src="../../../.gitbook/assets/select-bookmark.png" alt=""><figcaption><p>Select bookmark</p></figcaption></figure>

### **c) Bulk upload**&#x20;

You can also bulk upload a CSV file of recipients' emails. Click the 'Bulk upload' option. This will open up the bulk upload modal as shown in the image below.\
\
Click the 'Upload' button or drag and drop to upload the CSV file with the recipient's details.

<figure><img src="../../../.gitbook/assets/image (9) (3).png" alt=""><figcaption><p>Bulk upload option</p></figcaption></figure>

**Download sample**&#x20;

Click 'Download sample' to download a sample CSV document to understand how the uploaded CSV file should be structured.\
\
The image below displays the structure of the download sample CSV file.

<figure><img src="../../../.gitbook/assets/download-sample.png" alt=""><figcaption><p>Download sample csv file</p></figcaption></figure>

**Download filterss/bookmark**

Clicking on this option will download the entered recipient's email address, and filter/bookmark selection as a CSV file.

<figure><img src="../../../.gitbook/assets/download.png" alt=""><figcaption><p>Download email recipients option</p></figcaption></figure>

The downloaded CSV file looks as shown in the below image.

<figure><img src="../../../.gitbook/assets/email-recipients.png" alt=""><figcaption><p>Email recipients</p></figcaption></figure>

**Clear all**&#x20;

Click the 'Clear all' link to clear or reset all the entered filter/bookmarks and recipients' details.

### **d) Report preview**&#x20;

This option shows a preview of the report with the applied filter/bookmark. You can preview the report in PDF or Excel formats.

{% hint style="info" %}
If the report size is less than 2 MB it will be displayed as an inline preview. However, if the file size exceeds 2 MB the preview report will get downloaded as a zip file.
{% endhint %}

Clicking on the preview icon will display a 'Preview available' toast message at the bottom of the page (if the report/page size is less than 2 MB).

<figure><img src="../../../.gitbook/assets/pdf-preview.png" alt=""><figcaption><p>PDF preview option</p></figcaption></figure>

Click the 'View' link to view an inline preview of the report.

<figure><img src="../../../.gitbook/assets/preview.png" alt=""><figcaption><p>Preview report toast</p></figcaption></figure>

The report preview will be displayed as shown in the image below. You can also download the report preview by clicking on the 'Download' button on the preview.

<figure><img src="../../../.gitbook/assets/download-preview.png" alt=""><figcaption><p>Report preview download</p></figcaption></figure>

**Delete icon**&#x20;

Click the 'Trash' icon to delete the applied filter/bookmark.

### **e) Subject**&#x20;

Enter the subject line of the email. Clicking the 'Insert variable' link will open up a 'Suggested variables' modal from which you can select the pre-declared variables to be inserted into the subject line.&#x20;

<figure><img src="../../../.gitbook/assets/insert-variable (1).png" alt=""><figcaption><p>Insert variables option</p></figcaption></figure>

### **f) Body**&#x20;

Enter the body/content of the email. Pre-configured variables can be included in the email body as well.&#x20;

### g) Send report as&#x20;

You can select the format you want the report to be sent.&#x20;

Currently, we offer the following three options: 'PDF', 'Excel', and 'Preview images' of high quality.&#x20;

If you have selected either the 'All pages' option or more than one page in the 'Select' option of the 'Pages' option, then you can export the report as a merged file or as multiple files.

<figure><img src="../../../.gitbook/assets/send-report-as.png" alt=""><figcaption><p>Send report as option</p></figcaption></figure>

## **ii) OneDrive**

To set OneDrive as the destination, select the 'OneDrive' option from the left pane. If you haven't connected your OneDrive account, you will get the following screen shown in the image below.

Click on 'Connect' and authenticate with your One Drive account.

<figure><img src="../../../.gitbook/assets/one-drive.png" alt=""><figcaption><p>OneDrive connection</p></figcaption></figure>

After a successful connection, you will see the configuration screen with the following options:

### **a) Folder**&#x20;

You can specify the destination folder in OneDrive where you want the report to be exported. You can optionally specify a subfolder as well.&#x20;

Click on the 'Browse' button. This will open up a 'Select folder' modal in which you can select the OneDrive destination folder.

<figure><img src="../../../.gitbook/assets/image (90).png" alt=""><figcaption><p>OneDrive destination folder selection modal</p></figcaption></figure>

Clicking the 'Insert variable' link next to the subfolder field will suggest pre-defined variables that can be easily inserted into the subfolder field in a single click.

<figure><img src="../../../.gitbook/assets/folder-insert-variable.png" alt=""><figcaption><p>Subfolder insert variable option</p></figcaption></figure>

### **b) File name**&#x20;

This field is pre-populated with the file name that you entered in the 'Select report' section.&#x20;

Clicking the 'Insert variable' link next to the file name field will suggest pre-defined variables that can be easily inserted into the file names field in a single click.

<figure><img src="../../../.gitbook/assets/file-insert-variable.png" alt=""><figcaption><p>Filename insert variable option</p></figcaption></figure>

### **c) Send report as**&#x20;

Here you can select how you want the report to be exported as. You can select either PDF or Excel format. Both PDF and Excel can be exported in merged or multiple formats.

### **d) Filter/bookmark**&#x20;

You can select if you want the applied filters/bookmarks to be exported to the chosen destination. It is set to 'None' if no filters/bookmarks are applied to the report.

<figure><img src="../../../.gitbook/assets/one-drive-pdf.png" alt=""><figcaption><p>OneDrive send report as option</p></figcaption></figure>

You can create more than one OneDrive destination folder to export the report. Click on the 'Add folder' button on the top right corner to add another destination folder.

## **iii) Microsoft Teams**

To set Microsoft Teams as the destination, select the 'Microsoft Teams' option from the left pane. If you haven't connected your Microsoft account, you will get the following screen shown in the image below.

{% hint style="info" %}
If Microsoft teams are chosen as the destination, a notification will be sent to the chosen channel whenever a schedule runs.
{% endhint %}

Click on 'Connect' and authenticate with your Microsoft account.

<figure><img src="../../../.gitbook/assets/teams-login.png" alt=""><figcaption><p>Microsoft teams connection</p></figcaption></figure>

After a successful connection, you will see the configuration screen with the following options:

### **i) Team**&#x20;

Select the Microsoft team

### **ii) Channel**&#x20;

Select the channel from the chosen team

### **iii) Sub folder**&#x20;

Specify an optional sub folder to be created inside the chosen team's channel

### **iv) File name**&#x20;

This field is pre-populated with the file name that you entered in the 'Select report' section

### **v) Webhook URL**&#x20;

Enter the webhook URL of the team's channel you have selected as the destination.

To learn more about how to configure the incoming webhook, click on the 'How to configure incoming webhook?' tooltip as highlighted in the below image.

<figure><img src="../../../.gitbook/assets/webhook.png" alt=""><figcaption><p>Webhook url option</p></figcaption></figure>

### **vi) Send report as**&#x20;

Here you can select how you want the report to be exported as. You can select either PDF or Excel format.

### **vii) Filter/bookmark**&#x20;

You can select if you want the applied filters/bookmarks to be exported to the chosen destination. It is set to 'None' if no filters/bookmarks are applied to the report. You can learn more about it [here](select-destination-s.md#filter).

<figure><img src="../../../.gitbook/assets/team-settings-1.png" alt=""><figcaption><p>Microsoft teams send report as option</p></figcaption></figure>

You can add more than one destination channel to export the report. Click on the 'Add channel' button to add a destination channel.

In the next section, we'll look at [reviewing and saving subscriptions](review-and-save-subscription.md).
