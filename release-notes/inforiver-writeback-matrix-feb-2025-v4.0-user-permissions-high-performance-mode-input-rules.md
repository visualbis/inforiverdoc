# Inforiver Writeback Matrix Feb 2025 - v4.0 -  User permissions, High-performance mode, Input rules

## 1. Introducing user roles and permissions

User management in Inforiver is now more secure and streamlined with our new, role-based access control policies.

We’ve replaced the existing admin and member roles with a new set of user roles with defined access permissions. If you are an admin, you can assign roles to users (or Active Directory groups) to specify what they can or cannot do with their Inforiver reports.

For instance, an ‘input user’ can create data inputs, forecasts, scenarios, etc., while only an ‘input admin’ can change the related settings.

![](<../.gitbook/assets/0 (2).png>)

In addition to these default roles, workspace admins can create custom roles and policies on a granular level, ensuring enhanced data governance and security.

![](<../.gitbook/assets/1 (3).png>)

Note: Existing admins and members have been moved to the ‘Admin’ and ‘Contributor’ roles, respectively. Admins retain their permissions for user management and writeback settings, while contributors can access all report-level settings.

You can refer to the documentation for the detailed roles and permissions matrix.

## 2. Data Input

### 2.1. Input rules for data input and forecast measures

While adding input and forecast columns to your report, you may need to set minimum and maximum limits to the column values. You can configure these limits and the distribution settings in the ‘Data Input’ and ‘Forecast’ side panels.

Additionally, we have introduced a centralized menu option, ‘**Input Rules’**.

![Input rules for Data Input and Forecast
](<../.gitbook/assets/2 (2).png>)

With this, you can:

* Configure input and distribution rules for measures and columns in one place.
* Set global rules for all data input and forecast measures or apply them to specific measures.
* Choose the rows, columns, and period range to which the rules should apply.
* View additional details such as who set the rules, when they were configured, and the applicable rows, columns, and measures.

**Locking rule:** Configure which cells should be locked and restricted from changes during distribution and forecasting to ensure key values remain unchanged.

![](<../.gitbook/assets/3 (2).png>)

**Min-Max rule:** Set limits on the minimum and maximum values users can enter in these measures. These constraints ensure that the measure values do not fall below or exceed your specified limits during forecasting and distribution.

![](<../.gitbook/assets/4 (2).png>)

**Distribution rule:** Choose whether to distribute the total equally or to use a weighted distribution. You can also define the period range from which the weights will be derived, as well as the target rows and columns where they will be applied.

![](<../.gitbook/assets/5 (2).png>)

## 3. Data streaming to Analytics+

Want to create Analytics+ charts for your Inforiver reports? We have the solution with our new **Data Streamer** feature. With this, you can quickly stream your report’s dimension data, as well as native and custom input measures to an Analytics+ visual.

Create a sample Analytics+ visual with some measure added to it, as displayed below, side by side. Then, go to **Settings > Global Settings > Data Streamer**.

![Data streamer in Global settings](<../.gitbook/assets/6 (2).png>)

Create a new data source in the Data Streamer by configuring the necessary fields and values for your visualization. Add filters, if needed. In the Analytics+ visual, customize your chart with options such as Chart Type, Pivot Data, etc., and you’re all set.

![Creating Analytics+ charts with data streamer](<../.gitbook/assets/7 (2).png>)

## 4. Optimized performance for large datasets

Inforiver now supports faster and seamless working with large datasets, up to 1 million records with our new, high-performance mode.

This mode transforms the way the data input values are stored, retrieved, and updated. When enabled, you’ll notice improved performance and reduced processing times, especially with larger datasets.

![High performance mode](<../.gitbook/assets/8 (1).png>)

Please remember to **enable this mode before creating any data input measures** or columns in your report. Switching between modes is not possible after data input columns are created and updated unless you delete them.

## 5. Infobridge

### 5.1. Faster writeback up to 30 million records

Experience **three times faster writebacks** in Infobridge, with enhanced efficiency and scalability. We have improved the Infobridge writeback process to accommodate larger datasets, now supporting up to 10 million records. For Azure SQL destinations, Infobridge writebacks can handle up to 30 million records.

### 5.2. OneLake as data source

You can now add data sources from OneLake to Infobridge. Ensure that you’re connected to your Fabric Lakehouse and Azure Data Lake Storage from the ‘My Integrations’ page in the console, and you are good to go.

![](../.gitbook/assets/9.gif)

### 5.3. Support for EDITABLE data source

Infobridge can fetch data from EDITable.

[**EDITable**](https://inforiver.com/editable/) supports a wide range of cloud-based and on-premises databases, including Fabric Warehouse, Fabric SQL, Azure SQL, Snowflake, Amazon Redshift, BigQuery, Databricks, and PostgreSQL. The data tables from these destinations can now be imported into Infobridge via EDITable for real-time, integrated and connected planning.

![](../.gitbook/assets/10.gif)

## 6. Writeback:

### 6.1. Seamless Auto-writeback

No more distracting notifications and pauses during the auto-writeback process. The auto-writeback process is now seamless, with the event notifications displayed at the bottom of the visual.



## 7. Forecast

The 'Forecast' tab now has an input rules menu where users can set up locking rules, the minimum and maximum values users can enter, and the distribution method for forecast measures and columns. To know more, click [here](inforiver-writeback-matrix-feb-2025-v4.0-user-permissions-high-performance-mode-input-rules.md#id-2.1.-input-rules-for-data-input-and-forecast-measures).

<figure><img src="../.gitbook/assets/image (1262).png" alt=""><figcaption><p>Input rules for forecast measures</p></figcaption></figure>

## 8. Audit log – enhanced

The audit log now displays a complete and comprehensive overview of all changes made to the report. This includes changes to data input measures, forecast measures, scenarios, snapshots, writeback settings, comments settings, conditional formatting, and more.

You can filter the logs by type, date range, the user who made the changes, and logs that include comments.

<figure><img src="../.gitbook/assets/11 (1).png" alt=""><figcaption><p>Enhanced audit log</p></figcaption></figure>

## 8. Scheduler:

### 8.1. Filter child jobs

Search and filter options have been added to the scheduler summary, allowing users to select child jobs based on table name, category, sub-category, job status, and recipients for email destinations.

<figure><img src="../.gitbook/assets/12 (1).png" alt=""><figcaption><p>Filter child jobs</p></figcaption></figure>

## 9. Visual Formulas

The latest version supports statistical formulas for calculating standard deviation, variance, mean, median, mode, percentiles, and much more.

## 10. Commenting and Collaboration

The comment panel now features simple and detailed views, allowing users to edit comments inline on the panel, resize the panel to view longer comments, and manage who can add starred comments.

<figure><img src="../.gitbook/assets/image (1263).png" alt=""><figcaption><p>simple and detailed views</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (1264).png" alt=""><figcaption><p>Manage permissions for starred comments</p></figcaption></figure>

## 11. Other Enhancements

* This release adds Bulgarian language translation support within the Localization Settings.
* Granular forecast controls are included in the ‘Allowed User Controls’ window to manage permissions for closing periods, reforecasting, and distributing deficits in the Reading view.
* You can now writeback your snapshot data to the configured destinations using the Writeback option available in the Snapshots tab.
* The staging table is enabled by default in supported destinations, with an option to disable it if required.
* The author's name and date in comments will now be included in exports only if the corresponding option is checked in the Page Setup settings.
* The ‘Metrics’ page in the admin console now shows detailed information about the health of all worker services for better monitoring.
* Security/Active Directory groups without their emails enabled can also be included in the writeback settings user list, allowing them to use admin connections and add writeback destinations.
* The pivot explorer window is now bigger for improved readability.
* Issue with the 'LOOKUP' function for Infobridge query measures has been fixed.
