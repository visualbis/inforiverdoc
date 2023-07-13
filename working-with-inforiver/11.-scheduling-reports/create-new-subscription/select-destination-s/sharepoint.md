# SharePoint

To set SharePoint as the destination, select the 'SharePoint' option from the left pane. The following configurations need to be setup to deliver reports to Sharepoint destinations:

### **a) Site address**&#x20;

Select the SharePoint site address. E.g. <mark style="color:green;">https://\<your company>.sharepoint.com</mark> or <mark style="color:green;">https://\<your company>sharepoint.com/sites/\<your folder></mark>.

### b)Document library

Select the SharePoint document library to which the report should be delivered.

### c)Folder/subfolder

You can optionally specify the destination subfolder the report will be delivered to.

### **d) File name**&#x20;

This field is pre-populated with the file name.&#x20;

Clicking the 'Insert variable' link next to the file name field will suggest pre-defined variables that can be easily inserted into the file names field in a single click.

### e) Send report as&#x20;

You can select the format in which the report has to be sent. Currently, we offer three options: 'PDF', 'Excel', and 'Preview images' of high quality.&#x20;

If you have selected either the 'All pages' option or more than one page in the 'Select' option of the 'Pages' option, then you can export the report as a merged file or as multiple files.

### **f) Filter/bookmark**&#x20;

You can select this option if you want the applied filters/bookmarks to be exported to the chosen destination. It is set to 'None' if no filters/bookmarks are applied to the report. You can learn more about it [here](sharepoint.md#filter).

You can also [bulk upload](https://app.gitbook.com/o/Bi5mNLq31yHE9Ep9vISb/s/EbkCXCUXmtUq5tcnUtZE/\~/changes/237/working-with-inforiver/11.-scheduling-reports/create-new-subscription/select-destination-s/onedrive#e-bulk-upload) filters and bookmarks in csv format.

<figure><img src="../../../../.gitbook/assets/image (16).png" alt=""><figcaption><p>Configuring SharePoint Destinations</p></figcaption></figure>

{% hint style="info" %}
You can create more than one SharePoint destination folder to export the report. Click on the 'Add folder' button on the top right corner to add another destination folder.
{% endhint %}

In the next section, we'll look at [reviewing and saving subscriptions](../review-and-save-subscription.md).
