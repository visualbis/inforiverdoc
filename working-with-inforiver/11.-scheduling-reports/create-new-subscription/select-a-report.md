# Select a report

## 1. Select a Power BI report

In this section, you need to provide all the report-related details and configurations. This section has the following options:

### i) Select report

In the first drop-down, choose the Power BI workspace where the report you want to schedule is published.

If you schedule the subscription from the Power BI report, the 'Workspace' and 'Report' fields will be auto-populated with the workspace and report names, respectively. If you wish to schedule a different report, you can update the details here.

<figure><img src="../../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Select workspace</p></figcaption></figure>

Based on the selection made in the first drop-down, the second drop-down gets populated with reports available in the selected workspace.&#x20;

In the second drop-down, select the report for which you want to create a subscription.

<figure><img src="../../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Select report </p></figcaption></figure>

### ii) Pages

Here you can choose which pages of the report to schedule.&#x20;

* **All pages:** Send all the pages of the report.
* **Select:** If you select this option, a drop-down menu appears, allowing you to choose which pages to schedule and send. Multiple pages can be selected.

<figure><img src="../../../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Select pages</p></figcaption></figure>

### iii) Include hidden pages&#x20;

You can also publish reports containing hidden pages. When you set up your subscription, you will have the option to include hidden pages.&#x20;

<figure><img src="../../../.gitbook/assets/image (1114).png" alt=""><figcaption><p>Include hidden pages</p></figcaption></figure>

### iv) Row-level security

Enabling this option will export the report based on the row-level security applied. If this option is enabled, initially a consent email will be sent to the selected recipients, and only after the approval of the consent email will the scheduled reports be sent to the recipients.

Recipients with 'Admin' and 'Member' access roles will be able to view the entire report, whereas the recipients with 'Viewer' access would be able to view only the relevant data based on their role.&#x20;

You can manage the roles of the members using the 'Manage roles' option under the 'Modelling' tab in the Power BI toolbar.

<figure><img src="../../../.gitbook/assets/manage-roles.png" alt=""><figcaption><p>Manage roles option</p></figcaption></figure>

For example, in the following image, the 'Report Viewer' role has been set to view only the data related to the 'United States' region.

<figure><img src="../../../.gitbook/assets/rls.png" alt=""><figcaption><p>Applying security roles</p></figcaption></figure>

{% hint style="info" %}
If RLS is enabled then only the 'Email' destination is supported.
{% endhint %}

As seen below, members with the 'Report viewer' member role would be able to see only 'United States' under the categories while viewing the report.

<figure><img src="../../../.gitbook/assets/report-viewer.png" alt=""><figcaption><p>Report with RLS</p></figcaption></figure>

You can learn more about row-level security and how to define user roles and rules [here](https://learn.microsoft.com/en-us/power-bi/enterprise/service-admin-rls).

### v) Report plus layout

You can create subscriptions based on the Report+ categories. In this report, we have two categories: _Beverages_ and _Water_. These categories are available with page breaks, with each category taking up a page. You can send the records corresponding to each category to separate email IDs.&#x20;

Learn more about Report+ [here](../../8.-paginated-reporting/report-layouts-report+.md).

<figure><img src="../../../.gitbook/assets/image (1121).png" alt=""><figcaption><p>Report plus view</p></figcaption></figure>

Once you select 'Report plus layout', the scheduler automatically detects the number of categories present in the report page selected.

<figure><img src="../../../.gitbook/assets/image (1122).png" alt=""><figcaption><p>Report plus layout categories</p></figcaption></figure>

These categories can be viewed and selected on the 'Select Destinations' page, under the 'Category' section.

<figure><img src="../../../.gitbook/assets/image (1123).png" alt=""><figcaption><p>Report category in destination</p></figcaption></figure>

{% hint style="info" %}
If both the 'Report plus layout' and 'Row level security' options are enabled, only the 'Email' destination would be available.
{% endhint %}

## 2. Refresh dataset

### i) Refresh dataset for each run

If you have reports where the data gets frequently updated and you want the updated data to be sent every time the schedule is run, then you can enable the 'Refresh dataset for each run' option. If this option is enabled, only 'Email' can be chosen as the 'Destination' and other third-party destinations won't be available.

<figure><img src="../../../.gitbook/assets/image (1124).png" alt=""><figcaption><p>Refresh dataset for each run option</p></figcaption></figure>

### ii) Dataset owner

If the 'Refresh dataset for each run' option is enabled, a consent email must be sent before the data refresh. This email will be sent to the recipients specified in the dataset owner option.

When you enable the 'Refresh dataset for each run' option, the dataset owner's name is automatically populated in this field. You can also include the email addresses of additional dataset owners or users if needed.&#x20;

<figure><img src="../../../.gitbook/assets/image (1125).png" alt=""><figcaption><p>Dataset owner</p></figcaption></figure>

A sample consent email is shown in the image below.

<figure><img src="../../../.gitbook/assets/consent-email (1).png" alt="" width="563"><figcaption><p>Refresh dataset consent email</p></figcaption></figure>

{% hint style="warning" %}
The subscription will be created only if the dataset owner(s) provide consent. The scheduled jobs will keep failing until consent is provided.
{% endhint %}

## 3. Notifications

### Notify if failed to deliver&#x20;

Here you can specify the email addresses to which notifications should be sent in case of failure in report delivery. The schedule owner's name will be added by default.&#x20;

You can choose to add other members' names by typing in the input box or choosing from the drop-down. You can also add external email addresses of members who are not part of your team/organization.

<figure><img src="../../../.gitbook/assets/image (1126).png" alt=""><figcaption><p>Notify if failed to deliver option</p></figcaption></figure>

If in case any of the scheduled runs fails, then an email will be sent to all the selected members with the reason for failure, an error log, and a link to track back the error as shown in the image below.

<figure><img src="../../../.gitbook/assets/job-failure-email.png" alt=""><figcaption><p>Failed schedule email</p></figcaption></figure>

## 4. Legacy mode

We have recently optimized our processes, significantly reducing job run times. Scheduler jobs now run three times faster than before. This high-performance mode is the default, but the standard mode can be selected if necessary.

<figure><img src="../../../.gitbook/assets/image (1127).png" alt=""><figcaption><p>Legacy Mode</p></figcaption></figure>

## 5. Export settings

### Include an appendix in PDF&#x20;

Enabling this option will display an appendix for each report page with information like the font used, page name, filters applied, etc.

<figure><img src="../../../.gitbook/assets/image (1128).png" alt=""><figcaption><p>Include Appendix</p></figcaption></figure>

A sample appendix is shown below.

<figure><img src="../../../.gitbook/assets/pdf-appendix.png" alt=""><figcaption><p>PDF appendix</p></figcaption></figure>

In the next section, we'll look at configuring the subscription frequency.
