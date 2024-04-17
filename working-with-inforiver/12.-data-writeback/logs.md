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

#### 1.1. Search bar&#x20;

In the search bar, users could search and filter writeback logs based on their ID, report, or environment.

<figure><img src="../../.gitbook/assets/image (555).png" alt=""><figcaption><p>Search bar</p></figcaption></figure>

#### 1.2. Report

You can use the dropdown to select a particular report name.

<figure><img src="../../.gitbook/assets/image (556).png" alt=""><figcaption><p>Report filter</p></figcaption></figure>

#### 1.3. Started by

You can use this filter to view logs based on the person who triggered the writeback. Select the person(s) from the list of users.

<figure><img src="../../.gitbook/assets/image (557).png" alt=""><figcaption><p>Started by filter</p></figcaption></figure>

#### 1.4. Environment&#x20;

Use the drop-down to filter the writeback logs based on the environment from which writeback was triggered.

<figure><img src="../../.gitbook/assets/image (559).png" alt=""><figcaption><p>Filter based on writeback environment</p></figcaption></figure>

**1.5. Destination**

Use the drop-down to filter the writeback logs based on the writeback destination.

<figure><img src="../../.gitbook/assets/image (558).png" alt=""><figcaption><p>Destination filter</p></figcaption></figure>

#### 1.6. More - Status

Click on More and select Status to enable the dropdown. Use the below drop-down to filter the log based on the writeback status.&#x20;

<figure><img src="../../.gitbook/assets/image (560).png" alt=""><figcaption><p>Status filter</p></figcaption></figure>

#### 1.7. More - Event source

Select the **Event source** option under the More section - this will enable another dropdown that can be used to filter logs based on the writeback mode i.e. Writeback, Auto Writeback, or Reset.

<figure><img src="../../.gitbook/assets/image (561).png" alt=""><figcaption><p>Event source filter</p></figcaption></figure>

#### 1.8. More  - Create time&#x20;

Select the **Start Time** option under the More section - this will enable another dropdown that can be used to filter logs based on the writeback start time.

<figure><img src="../../.gitbook/assets/image (562).png" alt=""><figcaption><p>Create time filter</p></figcaption></figure>

* **Within the last** - If you select this option, you can specify the number of hours, minutes, or seconds. The logs will be fetched if the writeback start time falls within this period.
* **Last 7 days** - Selecting this option will filter the logs within the last 7 days&#x20;
* **Last 30 days** - This option will filter the logs that were created in the last 30 days.
* **Between** - If you select this option, then you can specify the starting and ending date within which you can filter your writeback logs.

<figure><img src="../../.gitbook/assets/image (563).png" alt=""><figcaption><p>Specifying a time range</p></figcaption></figure>

#### 1.9. Reset all

Clicking on this link will reset all the applied filters.

### 2. Writeback log columns

In this section, let's explore the columns in the writeback logs portal.

<figure><img src="../../.gitbook/assets/image (564).png" alt=""><figcaption><p>Writeback log console</p></figcaption></figure>

#### 2.1. ID&#x20;

This column displays a unique log ID that is used to identify the writeback log. You can sort the ID in ascending or descending order using the up/down arrows respectively.

Clicking on the writeback ID will open up a page with a detailed summary of the writeback.&#x20;

Clicking the 'General' tab will display a summary of the writeback along with the milestones and their status.

<figure><img src="../../.gitbook/assets/image (300).png" alt=""><figcaption><p>Writeback summary</p></figcaption></figure>

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

#### 2.2. Report &#x20;

This specifies the report the writeback belongs to. You can sort the reports alphabetically in ascending or descending order using the up/down arrows respectively.

#### 2.3. Destination&#x20;

Destination(s) the data was written back to.

#### 2.4.Duration&#x20;

The total duration of the writeback.

#### 2.5. Status&#x20;

Shows whether the writeback succeeded or failed. You can sort the status alphabetically in ascending or descending order using the up/down arrows respectively.

#### 2.6. Created at&#x20;

The data and time at which the writeback was started. You can sort the created date in ascending or descending order using the up/down arrows respectively.

#### 2.7. Started by

Name of the user who started the writeback. You can sort the user name in ascending or descending order using the up/down arrows respectively.

#### 2.8. Scenario

Lists any scenarios that were written back. If there are no scenarios for writeback, the console will display 'Base'.

#### 2.9.  Writeback type

Specifies whether the writeback was in Long, Wide, Long with Changes, or Wide with Changes format.

#### 2.10.  Incoming cell count

Specifies the number of cells in your report that were written back.

#### 2.11. Environment

The environment of the writeback. You can sort the environments in ascending or descending order using the up/down arrows respectively.

#### 2.12. Event

Use this field to identify whether the log is for a regular writeback, auto writeback, or a reset operation.

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
