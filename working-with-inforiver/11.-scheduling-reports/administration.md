# Administration

Inforiver provides a comprehensive and business-friendly user interface for managing and administering schedules. The 'All subscriptions' page is similar to the 'My subscriptions' page except for the fact that it is available only for admin users to view and manage the subscriptions of all other members.

<figure><img src="../../.gitbook/assets/all-subscriptions.png" alt=""><figcaption><p>All subscriptions page</p></figcaption></figure>

The options available on the 'All subscriptions' page are the same as the ones available on the 'My subscriptions' page. Refer [Manage your subscriptions](manage-your-subscriptions.md) section to learn more about each of these options in detail.

{% hint style="info" %}
'All subscriptions' and 'User management' pages are available only for admin users
{% endhint %}

You can also monitor, view, and gather insights into the subscriptions of other members.

## 1. Monitoring subscription jobs

All the scheduled jobs will be displayed here. The 'Subscription jobs' page has the following columns.

<figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption><p>Subscription jobs</p></figcaption></figure>

### a) Job details

* **ID** - Unique ID of the scheduled job
* **Subscription** - The name of the subscription
* **Workspace** - the name of the workspace the subscription belongs to
* **Report** -The name of the report
* **Started by** - Name of the person who started the schedule
* **Job type** - The job type of the schedule
* **Started** - The date and the time the job started
* **Duration -** The exact duration the job ran
* **Status -** Displays the current status of the job

{% hint style="info" %}
Each of these column values can be sorted in ascending/descending order by clicking on their respective column headers.
{% endhint %}

Clicking on any of the scheduled job IDs will display a detailed summary of the job in the 'Summary' tab.

<figure><img src="../../.gitbook/assets/subscription-summary (1).png" alt=""><figcaption><p>Subscription summary</p></figcaption></figure>

Clicking on the 'Email' tab will display a summary of all the emails sent along with the delivered at date, time, status, filter and bookmarks.

<figure><img src="../../.gitbook/assets/all-subscriptions-email.png" alt=""><figcaption><p>Subscription jobs email summary</p></figcaption></figure>

You can filter the jobs using the following:

<figure><img src="../../.gitbook/assets/subscription-jobs-filters.png" alt=""><figcaption><p>Subscription jobs filter option</p></figcaption></figure>

### **b) Search bar**&#x20;

Using this search bar you can search for the job you need. If you have an enormous list of job subscriptions this feature comes in handy

### **c) Subscription**&#x20;

Using this drop-down you can filter the jobs based on the subscription. Only the jobs of the selected subscriptions will get displayed.

<figure><img src="../../.gitbook/assets/subscription-jobs-filter.png" alt=""><figcaption><p>Subscription jobs filter</p></figcaption></figure>

### **d) Workspace**

Using this drop-down you can filter the jobs based on the workspaces. Only the jobs of the selected workspaces will get displayed.

<figure><img src="../../.gitbook/assets/subscription-jobs-workspace.png" alt=""><figcaption><p>Subscription jobs workspace filter</p></figcaption></figure>

### **e) Report**&#x20;

Using this drop-down you can filter the jobs based on the reports. Only the jobs of the selected reports will get displayed.

<figure><img src="../../.gitbook/assets/subscription-jobs-reports.png" alt=""><figcaption><p>Subscription jobs reoprt filter</p></figcaption></figure>

### **f) Started by**&#x20;

Using this drop-down you can filter the jobs based on the users who started the jobs. Only the jobs started by the selected users will get displayed.

<figure><img src="../../.gitbook/assets/subscription-jobs-startedby.png" alt=""><figcaption><p>Subsription jobs starteby filter</p></figcaption></figure>

### **g) More**&#x20;

Click on this option to view additional filter options for the jobs. The additional filter options include filtration by

* **Destination** - Enabling this option will filter your jobs based on the selected destination
* **Status** - Enabling this option will filter your jobs based on the job status
* **Job type** - Enabling this option will filter your jobs based on the job type
* **Start time** - Enabling this option will filter your jobs based on the start time

<figure><img src="../../.gitbook/assets/subscription-jobs-more-filter.png" alt=""><figcaption><p>Subscription jobs more filter</p></figcaption></figure>

### **h) Reset all**&#x20;

Clicking on this option will reset all the applied filters.

## 2. Insights

This view displays all the insights about the subscriptions

### a) Metrics&#x20;

Dashboard with details about the number of completed, queued, running, and failed jobs.

Clicking on either of the job types will take you back to the subscription jobs page of the monitoring section with the corresponding status filter applied

<figure><img src="../../.gitbook/assets/metrics-page.png" alt=""><figcaption><p>Insights page</p></figcaption></figure>

You can also filter the job metrics for today, the last 7 days, or the last 30 days using the drop-down filter as highlighted

<figure><img src="../../.gitbook/assets/metrics-more-option.png" alt=""><figcaption><p>Metrics page</p></figcaption></figure>

### b) All reports

In the 'All reports' tab, you can see a list of all the reports.&#x20;

<figure><img src="../../.gitbook/assets/all-reports-page.png" alt=""><figcaption><p>All reports page</p></figcaption></figure>

Clicking on any of the report names will redirect to the 'Report details' page which displays several details.&#x20;

#### i) Lineage

In the 'Lineage' tab, you can see the lineage view of the report. You can see the data sources such as Excel/CSV/Databases, followed by the Power BI dataset, the Power BI report, and the Inforiver subscriptions.

<figure><img src="../../.gitbook/assets/all-report-workspace.png" alt=""><figcaption><p>Report lineage view</p></figcaption></figure>

#### ii) Subscription

In the 'Subscriptions' tab, you can see the list of job subscriptions related to the selected report.

<figure><img src="../../.gitbook/assets/all-report-subscription.png" alt=""><figcaption><p>Report subscriptions list</p></figcaption></figure>

#### iii) Writeback

In the 'Writeback' tab of the 'All reports' page, you can view a list of the writebacks performed in the report.

<figure><img src="../../.gitbook/assets/all-report-writeback.png" alt=""><figcaption><p>Reports writeback page </p></figcaption></figure>

#### iv) Comments

In the 'Comments' tab of the 'All reports' page, you can see details regarding all the comments in the report

<figure><img src="../../.gitbook/assets/all-reports-comments.png" alt=""><figcaption><p>Reports comments page</p></figcaption></figure>

Clicking on any of the 'Datasets' in the 'All reports' page will redirect to the 'Dataset details' page.

<figure><img src="../../.gitbook/assets/datasets.png" alt=""><figcaption><p>Datasets in all reports page</p></figcaption></figure>

#### i) Lineage

The lineage tab displays the lineage view of the dataset.

<figure><img src="../../.gitbook/assets/all-reports-dataset.png" alt=""><figcaption><p>Dataset lineage view</p></figcaption></figure>

In this section, we covered subscription administration. Navigate to the next section to learn more about [data writeback](../12.-data-writeback/).
