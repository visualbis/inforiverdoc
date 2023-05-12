# Select a report

## 1. Select a Power BI report

In this section, you need to provide all the report-related details and configurations. This section has the following options:

### i) Select report

In the first drop-down, select the Power BI workspace in which the report you want to schedule is published.

The 'Workspace' and 'Report' fields will get auto-populated with the workspace and report name of the report. If you want to schedule a different report, you can update the details here.

<figure><img src="../../../.gitbook/assets/select-workspace (1).png" alt=""><figcaption><p>Select workspace option</p></figcaption></figure>

Based on the selection made in the first drop-down, the second drop-down gets populated with reports available in the selected workspace.&#x20;

In the second drop-down, select the report for which you want to create a subscription.

<figure><img src="../../../.gitbook/assets/select-report.png" alt=""><figcaption><p>Select report option</p></figcaption></figure>

### ii) Pages

Here you can select the pages of the report to schedule.&#x20;

* **All pages** - Schedule all the pages of the report&#x20;
* **Select** - If this option is chosen, then a drop-down becomes available in which you can select the pages that you want to schedule. More than one page can be selected.

<figure><img src="../../../.gitbook/assets/select-pages.png" alt=""><figcaption><p>Select pages option</p></figcaption></figure>

### iii) Row-level security

Enabling this option will export the report based on the row-level security applied. If this option is enabled, initially a consent email will be sent to the selected recipients and only after the approval of the consent email, the scheduled reports will be sent to the recipients.

Recipients with 'Admin' and 'Member' access roles will be able to view the entire report whereas the recipients with 'Viewer' access would be able to view only the relevant data based on their role.&#x20;

You can manage the roles of the members using the 'Manage roles' option under the 'Modelling' tab in the Power BI toolbar.

<figure><img src="../../../.gitbook/assets/manage-roles.png" alt=""><figcaption><p>Manage roles option</p></figcaption></figure>

For example, in the following image, the 'Report Viewer' role has been set to view only the data related to the 'United states' region.

<figure><img src="../../../.gitbook/assets/rls.png" alt=""><figcaption><p>Applying security roles</p></figcaption></figure>

{% hint style="info" %}
If RLS is enabled then only the 'Email' destination is supported.
{% endhint %}

As seen below, members with the 'Report viewer' member role would be able to see only 'United States' under the categories while viewing the report.

<figure><img src="../../../.gitbook/assets/report-viewer.png" alt=""><figcaption><p>Report with RLS</p></figcaption></figure>

You can learn more about row-level security and how to define user roles and rules [here](https://learn.microsoft.com/en-us/power-bi/enterprise/service-admin-rls).

### iv) Report plus layout

You can create subscriptions based on the Report+ categories.  In this report, we have two categories - Beverages and Water. The records corresponding to these categories can be sent to different email IDs.&#x20;

You can learn more about Report+ [here](https://docs.inforiver.com/inforiver/working-with-inforiver/8.-paginated-reporting/report-layouts-report+).

<figure><img src="../../../.gitbook/assets/reportplus.png" alt=""><figcaption><p>Report plus view</p></figcaption></figure>

Once you select 'Report plus layout', the scheduler automatically detects the number of categories present in the report page selected.

<figure><img src="../../../.gitbook/assets/report-plus (1).png" alt=""><figcaption><p>Report plus layout categories</p></figcaption></figure>

These categories can be viewed and selected in the 'Select Destination' -> 'Category' section.

<figure><img src="../../../.gitbook/assets/report-plus-category.png" alt=""><figcaption><p>Report category in destination</p></figcaption></figure>

{% hint style="info" %}
If both the 'Report plus layout' and 'Row level security' options are enabled, only the 'Email' destination would be available.
{% endhint %}

## 2. Refresh dataset

### i) Refresh dataset for each run

If you have reports where the data gets frequently updated and you want the updated data to be used every time the schedule is run, then you can enable the 'Refresh dataset for each run' option.

<figure><img src="../../../.gitbook/assets/refresh-dataset.png" alt=""><figcaption><p>Refresh dataset for each run option</p></figcaption></figure>

If this option is enabled, only 'Email' can be chosen as the 'Destination' and other third-party destinations won't be available.

### ii) Dataset owner

This option becomes available only if the 'Refresh dataset for each run' option is enabled. You can add the email of the owners of the dataset.&#x20;

If the 'Refresh dataset for each run' option is enabled, then a consent email will be sent to the recipients added in the dataset owner option. The consent email is shown in the image below.

<figure><img src="../../../.gitbook/assets/consent-email (1).png" alt=""><figcaption><p>Refresh dataset consent email</p></figcaption></figure>

{% hint style="warning" %}
The subscription will be created only if the dataset owner(s) provide consent. The scheduled jobs will keep failing until consent is provided.
{% endhint %}

## 3. Notifications

### i) Notify if failed to deliver&#x20;

Here you can specify the email addresses to which notifications should be sent in case of failure in report delivery. The schedule owner's name will be added by default.&#x20;

You can choose to add other members' names by typing in the input box or choosing from the drop-down. You can also add external email addresses of members who are not part of your team/organization.

<figure><img src="../../../.gitbook/assets/notify.png" alt=""><figcaption><p>Notify if failed to deliver option</p></figcaption></figure>

If in case any of the scheduled runs fails, then an email will be sent to all the selected members, with the reason for failure, an error log, and a link to track back the error as shown in the image below.

<figure><img src="../../../.gitbook/assets/job-failure-email.png" alt=""><figcaption><p>Failed schedule email</p></figcaption></figure>

## 4. Export settings

### i) Include an appendix in PDF&#x20;

Enabling this option will display an appendix for each report page with information like the font used, page name, filters applied, etc. A sample appendix is shown below.

<figure><img src="../../../.gitbook/assets/pdf-appendix.png" alt=""><figcaption><p>PDF appendix</p></figcaption></figure>

In the next section, we'll look at [configuring the subscription frequency](set-subscription-frequency.md).
