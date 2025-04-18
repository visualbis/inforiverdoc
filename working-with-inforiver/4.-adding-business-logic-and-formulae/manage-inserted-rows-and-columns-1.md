# Manage inserted measures & columns

Measures and columns inserted in the visual such as calculations or data input columns can be managed using the **Manage Measures** option.

## 1. Measures and columns

Similar to the [Manage Rows](manage-inserted-rows-and-columns-1.md#id-1.-manage-rows) option, the **Manage Measures** option displays a list of inserted columns/measures with options to edit, delete, or hide them. All the measures created in a visual can be viewed in the Measures tab. Visual columns can be viewed and managed in the Columns tab.

In addition, there is also an 'Insert New' option which lets you insert calculated columns or data input columns right from this panel.

<figure><img src="../../.gitbook/assets/image (689).png" alt=""><figcaption><p>Managing inserted columns</p></figcaption></figure>

## 2. Settings

The **Manage Measures** side panel has a **Settings** tab that lets you control and configure important settings concerning the rows and measures, such as user permissions, time interval mapping, row dimension ID mapping, etc.

<figure><img src="../../.gitbook/assets/image (4) (1) (1).png" alt=""><figcaption><p>Settings pane</p></figcaption></figure>

### 2.1. Data input access

Inforiver Writeback Matrix allows setting explicit read/write access for specific users on data input and forecast columns.&#x20;

To set it, click **Insert -> Manage Measures -> Settings** **->** **Manage** in the **Data Input Access.** You can add the required users in the pop-up window.

<figure><img src="../../.gitbook/assets/image (691).png" alt=""><figcaption><p>Data Input Access</p></figcaption></figure>

{% hint style="info" %}
Access control for all the columns can also be set through the **Manage Columns** dropdown as explained [here](insert-manual-input-columns.md#id-3.-access-control). Specifically for the forecast columns, the user access can be configured [here](../7.-planning-budgeting-and-forecasting/forecasting.md).
{% endhint %}

### 2.2. Time interval mapping

When you have a date hierarchy in your rows/columns, you can use the time interval mapping to verify the formats that Inforiver auto-detects. Hover over the<img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1)  (19).png" alt="" data-size="line">icon to view all the supported date formats.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Supported date formats</p></figcaption></figure>

You can also choose whether to use Power BI sorting or Inforiver sorting. When the **Sort** toggle is enabled, any sorting changes made at Power BI level will not be reflected in the visual. In the example, notice how the Power BI sorting is not applied on the Quarter when the Sort toggle is enabled.

<figure><img src="../../.gitbook/assets/image (32).png" alt=""><figcaption><p>Sort precedence</p></figcaption></figure>

### 2.3. Dimension ID mapping

Inforiver automatically assigns a dimension ID to each row dimension to uniquely identify them. This mapping helps to track and manage them, especially during operations like writeback. Visual components such as formatting, notes, comments, and data inputs added to the rows are also linked to the dimension IDs.&#x20;

When row dimensions are renamed/changed, we might lose these visual elements added. To avoid this, Inforiver allows us to map the row dimensions to a constant dimension ID.

In the example below, we’ve applied formatting, added notes, and comments, and added data inputs to the products, _Juices_ and _Tea & Coffee_.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (2) (1).png" alt=""><figcaption><p>Sample report with formatting, comments and data input columns</p></figcaption></figure>

The visual elements were lost after the product names were renamed to _Fruit Juices_ and _Chai & Coffee_ respectively.

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (2) (1) (1).png" alt=""><figcaption><p>When the row dimension 'Product Name' is renamed</p></figcaption></figure>

To avoid this, let us map the dimension IDs to a constant dimension, such as the _Product ID_ instead of the _Product Name_. To do so, navigate to **Insert -> Manage Measures -> Settings -> Row ID mapping   -> Manage**.

<figure><img src="../../.gitbook/assets/image (5) (1) (3).png" alt=""><figcaption><p>Manage Row ID Mapping</p></figcaption></figure>

The image below shows the default row dimension ID mapping.&#x20;

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (2) (1) (1).png" alt=""><figcaption><p>Default row ID mapping</p></figcaption></figure>

Let us map the 'Product Name' to the constant dimension, 'Product ID' as shown below. Click **Apply**.

<figure><img src="../../.gitbook/assets/image (6) (1) (3).png" alt=""><figcaption><p>row dimesion ID mapped manually</p></figcaption></figure>

Note that changing the mapping removes all the initial formatting and visual elements associated with it.

Any formatting, notes, comments, and data inputs added after mapping with the constant dimension ID are retained as shown below, including during the writeback.

<figure><img src="../../.gitbook/assets/row-dimension-id-mapping.png" alt=""><figcaption><p>After manually mapping row ID dimensions</p></figcaption></figure>

**Updates due to skipped row ID dimensions reflected in writeback data**

After mapping the row IDs to a constant dimension, not only the visual formatting, data changes, notes, comments, etc., are retained in the report but also captured in the writeback data promptly.

The report below shows the default mapping, followed by the results of the writeback data.

<figure><img src="../../.gitbook/assets/1.5.1..png" alt=""><figcaption><p>Writeback data before the change</p></figcaption></figure>

After manually mapping the row dimension to a constant ID like the Product ID, any changes made in the report are also effectively captured in the writeback. In the image below, you can see the updated records in the report that are also reflected in the writeback data.

<figure><img src="../../.gitbook/assets/1.5.2. rowID-2.png" alt=""><figcaption><p>Writeback data after row ID mapping and data changes</p></figcaption></figure>

### 2.4. Schedule backup for measure

You can retain point-in-time measure values with the new scheduled backup feature. The measure values are captured as separate read-only visual columns within the same visual. With this feature, you can easily calculate historical variances and analyze fluctuations in your numbers.

Navigate to Manage Measures > Settings > Schedule Backups for Measure to create monthly, weekly, or daily schedules.

<figure><img src="../../.gitbook/assets/image (1) (1) (5).png" alt=""><figcaption><p>Creating a measure backup schedule</p></figcaption></figure>

* **Start and End date:** Specify the time frame during which the measure should be backed up.
* **Schedule Time:** The time and timezone at which the backup job should be triggered.
* **Frequency**: Opt for daily/weekly/monthly schedules.&#x20;
* For daily backups, you can specify the number of backups to create. For weekly schedules, you can select the day of the week to take a backup. For monthly schedules, you can specify which day of the month to take a backup on and additionally opt to take a backup on the last day of the month as well.

<div><figure><img src="../../.gitbook/assets/image (1103).png" alt=""><figcaption><p>Daily schedule</p></figcaption></figure> <figure><img src="../../.gitbook/assets/2025-01-02_14h26_57.png" alt=""><figcaption><p>Weekly schedule</p></figcaption></figure> <figure><img src="../../.gitbook/assets/2025-01-02_14h27_10.png" alt=""><figcaption><p>Monthly schedule</p></figcaption></figure></div>

* **Measures**: Select the measures that need to be backed up.
* **Backup name:** Enter the name of the backup field.

You can run ad-hoc backups by clicking the **Run now** icon.

<figure><img src="../../.gitbook/assets/image (1104).png" alt=""><figcaption><p>Ad hoc backups</p></figcaption></figure>

{% hint style="info" %}
Measure backups will work only after the report is saved in Power BI. The report should also be created in a common workspace.
{% endhint %}

The image below shows a report with backed-up measures:

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) ( (2).png" alt=""><figcaption><p>Measure backups</p></figcaption></figure>

Measure backup jobs have dedicated logs that show the status of the backup, milestones, and the backups that are deleted when the limit is reached. Click the **View jobs** option from the Schedule Measure Backup side pane.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>View jobs</p></figcaption></figure>

Scheduled measure backup logs:

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Scheduled measure bkp logs</p></figcaption></figure>

### 2.5. Show all periods from Infobridge

Infobridge supports forecasts and allows you to capture projections or data for future time periods. Your target reports, however, may not require future data. The **Show All Periods from Infobridge** option in the Manage Measures side pane can be used to control whether time periods that do not exist in the target visual should be imported from Infobridge:

* When the toggle is enabled, all the time periods available in the bridge will be imported into the target report, irrespective of whether they exist in the target visual.
* When disabled, only the time periods in the bridge that exist in the target visual will be imported.

This option will be enabled only after creating an integration to a bridge

<figure><img src="https://docs.inforiver.com/~gitbook/image?url=https%3A%2F%2F3062809325-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FEbkCXCUXmtUq5tcnUtZE%252Fuploads%252FTTowA2D435slJbqwvFKy%252Fimage.png%3Falt%3Dmedia%26token%3Dde312faf-ff7b-4e0e-95d1-75b0fddc1b00&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=82c486ba&#x26;sv=2" alt=""><figcaption><p><strong>Show All Periods from Infobridge option</strong></p></figcaption></figure>

In the bridge, we have the allocated budgets for 2023 and 2024 as well as the projected budgets for 2025.

<figure><img src="https://docs.inforiver.com/~gitbook/image?url=https%3A%2F%2F3062809325-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FEbkCXCUXmtUq5tcnUtZE%252Fuploads%252FVxCBjgzyogTzEQbyf3rO%252Fimage.png%3Falt%3Dmedia%26token%3De8367d4b-c819-4948-93f1-b243ff10cfc3&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=502f17d5&#x26;sv=2" alt=""><figcaption><p>Projected and allocated budgets in the bridge</p></figcaption></figure>

The target report contains the profits for 2023 and 2024. We need to integrate the budgets for 2023 and 2024 with this report. The projected budgets for 2025 are not required in this case.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Profits in the target visual</p></figcaption></figure>

Since we've disabled the **Show All Periods from Infobridge** toggl&#x65;**,** when we insert the budget from the bridge, it will be inserted only for the time periods that exist in the target report.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1).png" alt=""><figcaption><p>Inserting budgets for existing time periods</p></figcaption></figure>
