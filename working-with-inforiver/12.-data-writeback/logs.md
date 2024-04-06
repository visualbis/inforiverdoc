---
description: Comprehensive and Searchable Writeback Logs
---

# Logs

Inforiver offers milestone-based tracking as soon as the writeback button is clicked. There are multiple ways to view a comprehensive log of an ongoing writeback instance or previous writeback instances:

* Click on Logs under the Export tab of the Inforiver toolbar.&#x20;
* Click View Log in the modal that opens upon completion of writeback.
* Go to the Writeback Logs tab under the Monitoring section of the Inforiver console.

<figure><img src="../../.gitbook/assets/image (15) (3).png" alt=""><figcaption></figcaption></figure>

### 1. Writeback log filters

The writeback logs page allows us to search through writeback logs using several filter criteria. Let's explore each of these filters.

#### a) Search bar&#x20;

In the search bar, users could search and filter writeback logs based on their ID, report, or environment.

<figure><img src="../../.gitbook/assets/image (267).png" alt=""><figcaption><p>Search bar</p></figcaption></figure>

#### b) Report

The drop-down menu can be used to select a particular report name.

<figure><img src="../../.gitbook/assets/image (268).png" alt=""><figcaption><p>Report filter</p></figcaption></figure>

#### c) Environment&#x20;

Use drop-down to filter the writeback log based on the environment.

<figure><img src="../../.gitbook/assets/image (269).png" alt=""><figcaption><p>Environment filter</p></figcaption></figure>

**d) Destination**&#x20;

Use the below drop-down to filter the writeback logs based on the writeback destination.

<figure><img src="../../.gitbook/assets/image (270).png" alt=""><figcaption><p>Destination filter</p></figcaption></figure>

#### e) Status

Use the below drop-down to filter the log based on the writeback status.&#x20;

<figure><img src="../../.gitbook/assets/image (271).png" alt=""><figcaption><p>Status filter</p></figcaption></figure>

#### f) More - Event source

&#x20;Enable the **Event source** option under the _More_ section - this will add another dropdown that can be used to filter logs based on the writeback mode i.e. Writeback, Auto Writeback, or Reset.

<figure><img src="../../.gitbook/assets/image (272).png" alt=""><figcaption><p>Event source filter</p></figcaption></figure>

#### g) More  - Start time&#x20;

Enable the **Start Time** option under the _More_ section - this will add another dropdown that can be used to filter logs based on the writeback start time.

<figure><img src="../../.gitbook/assets/image (273).png" alt=""><figcaption><p>Start time filter</p></figcaption></figure>

* **Within the last** - If you select this option, you can specify the number of hours, minutes, or seconds. The logs will be fetched if the writeback start time falls within this period.
* **Last 7 days** - Selecting this option will filter the logs within the last 7 days&#x20;
* **Last 30 days** - This option will filter the logs that were created in the last 30 days.
* **Between** - If you select this option, then you can specify the starting and ending date within which you can filter your writeback logs.

<figure><img src="../../.gitbook/assets/image (274).png" alt=""><figcaption><p>Between start and end date</p></figcaption></figure>

#### f) Reset all

Clicking on this link will reset all the applied filters.

### 2. Writeback log columns

In this section, let's explore the columns in the writeback logs portal.

<figure><img src="../../.gitbook/assets/image (299).png" alt=""><figcaption></figcaption></figure>

#### a) ID&#x20;

This column displays a unique log ID that is used to identify the writeback log. You can sort the ID in ascending or descending order using the up/down arrows respectively.

Clicking on the writeback ID will open up a page with a detailed summary of the writeback.&#x20;

Clicking the 'General' tab will display a summary of the writeback along with the milestones and their status.

<figure><img src="../../.gitbook/assets/image (300).png" alt=""><figcaption></figcaption></figure>

The writeback log summarizes the following milestones:

#### i) Data processing&#x20;

This indicates the events and steps that occurred during data processing. Click on the 'View events' link to view the data processing events in detail.

<figure><img src="../../.gitbook/assets/image (301).png" alt=""><figcaption></figcaption></figure>

The data processing event, logs the performed action, the date and time the event was last updated, and the status of the event.

#### ii) Deliver to destination

This milestone displays the events logged while the writeback data was delivered to the destination. You can click on the 'View destination events' link to view the summary of the writeback destination, the date and the time at which the destination was updated, and the status of the writeback.

<figure><img src="../../.gitbook/assets/image (302).png" alt=""><figcaption></figcaption></figure>

#### iii) Post processing

The post processing milestone indicates the events that occurred after processing the writeback. You can click on the 'View events' link to view the post processing action, the date and time the action was updated, and the status of the action/event.

<figure><img src="../../.gitbook/assets/image (303).png" alt=""><figcaption></figcaption></figure>

Clicking on the name of the destination will display the connection details about the configured writeback destination.

<figure><img src="../../.gitbook/assets/image (304).png" alt=""><figcaption></figcaption></figure>

#### b) Report &#x20;

This specifies the report the writeback belongs to. You can sort the reports alphabetically in ascending or descending order using the up/down arrows respectively.

#### c) Page

This specifies the page of the report the writeback belongs to.

#### d) Environment

The environment of the writeback. You can sort the environments in ascending or descending order using the up/down arrows respectively.

#### e) Destination&#x20;

Destination the data was written back to.

#### f) Duration&#x20;

The total duration of the writeback.

#### g) Started by

Name of the user who started the writeback. You can sort the started by date in ascending or descending order using the up/down arrows respectively.

#### h) Started at&#x20;

The data and time at which the writeback was started. You can sort the started date in ascending or descending order using the up/down arrows respectively.

#### i) Status&#x20;

The status of the writeback. You can sort the status alphabetically in ascending or descending order using the up/down arrows respectively.

Navigate to the next chapter, to learn more about display settings.

### 3. Exporting logs

You can easily export the logs for a specified period by following the steps outlined below.

**Step 1:** Click on the export button at the top right corner to open the export dialog box.

* Choose the format: CSV or Excel
* Choose the period range: the default range is 30 days or you can set a custom range

<figure><img src="../../.gitbook/assets/image (523) (1).png" alt=""><figcaption><p>Writeback logs export settings</p></figcaption></figure>

If you choose a custom range, you can select the start and end dates from the calendar widget.

<figure><img src="../../.gitbook/assets/image (524).png" alt=""><figcaption><p>Choosing a custom date range</p></figcaption></figure>

**Step 2:** Click Export. The status of the export will be displayed in the top right corner. After the export is complete, you can click the Download link to save the file to your system.

<figure><img src="../../.gitbook/assets/image (525).png" alt=""><figcaption><p>Download logs</p></figcaption></figure>

**Step 3:** Open the file to analyze the logs. You can quickly root cause and debug writeback failures with the Failure Reason column in the writeback log export.

<figure><img src="../../.gitbook/assets/image (526).png" alt=""><figcaption><p>Writeback export </p></figcaption></figure>
