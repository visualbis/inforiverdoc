# 12. Data writeback

Inforiver writeback allows a user to export and save a report table to destinations of different types including file destinations, data warehouses, and data lake storage.&#x20;

Inforiver, unlike other BI tools, does not require IT overhead in terms of database setup and defining the structure of writeback tables in advance. Inforiver instead supports dynamic database configuration and table creation at run time and performs semi-structured, on-the-fly writeback to more than one destination at a time.

{% hint style="info" %}
Data writeback is a Writeback Matrix feature; you need to have a valid Inforiver Writeback Matrix subscription.
{% endhint %}

## 1. Overview

The Writeback screen is accessed by going to the Export tab in the toolbar. Three buttons give you access to writeback and related settings.&#x20;

**Writeback** - Export report data to a destination.&#x20;

**Settings** - Configure writeback-related settings. Navigate to the [writeback settings](settings/) chapter to learn more.&#x20;

**Logs** - Every writeback event is logged with detailed information relevant to each writeback. Navigate to the [writeback logs](logs.md) chapter to learn more.

{% hint style="info" %}
Writeback will be disabled unless a row or column dimension is added to the visual.
{% endhint %}

## 2. Writeback Modes

You can choose whether to writeback the report alone or to writeback the report along with any associated scenarios.&#x20;

Clicking on the icon below the Writeback button will show options for writeback.

<figure><img src="../../.gitbook/assets/image (14) (2) (1).png" alt=""><figcaption><p>Writeback options</p></figcaption></figure>

Selecting 'Writeback All' will open a dialogue box, which lets you choose which scenarios to writeback. If you do not want a particular scenario to be exported - uncheck the box adjacent to the name of that particular scenario.

<figure><img src="../../.gitbook/assets/image (16) (3) (1).png" alt=""><figcaption><p>Writeback all</p></figcaption></figure>

## 3. Configure Destination

Inforiver supports fast writeback setup and execution for several types of data destinations. Configuring writeback destination(s) is straightforward and involves the same procedure (picture below) for any destination.

{% hint style="info" %}
On-premise database servers need to be directly reachable from the internet for writeback. For this, on-premise servers must have a public IP address with port forwarding.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (37) (1).png" alt=""><figcaption><p>Navigating to Inforiver writeback destination setup</p></figcaption></figure>

&#x20;A list of destinations will be displayed for the users to select from.&#x20;

<figure><img src="../../.gitbook/assets/image (907).png" alt=""><figcaption></figcaption></figure>

To learn how to configure each destination in the above list, [navigate to this page](destinations/#overview).&#x20;

{% hint style="info" %}
The number of rows that can be written back is 200k rows for Excel and CSV and 250 rows for OneDrive and SharePoint
{% endhint %}

## 4. Overview of writeback steps

**STEP 1:** Navigate to the Export ribbon and click the Settings button to open the writeback settings side pane.

<figure><img src="../../.gitbook/assets/image (676).png" alt=""><figcaption><p>Writeback settings</p></figcaption></figure>

**STEP 2:** In the general tab, set the writeback type, and optionally add filters and permissions. [Learn more about General writeback options.](settings/general-settings.md)

<figure><img src="../../.gitbook/assets/image (677).png" alt=""><figcaption><p>General settings for writeback</p></figcaption></figure>

**STEP 3:** In the data tab, determine the scenarios and series to be written back and enable automatic writeback if applicable. [Learn more about Data settings for writeback.](settings/data-settings.md)

<figure><img src="../../.gitbook/assets/image (678).png" alt=""><figcaption><p>Data settings tab for writeback</p></figcaption></figure>

**STEP 4:** Configure writeback destinations from the Destinations tab. [Learn more about configuring destinations. ](settings/destination-settings.md)

<figure><img src="../../.gitbook/assets/image (679).png" alt=""><figcaption><p>Destinations tab in writeback settings</p></figcaption></figure>

**STEP 5:** In the advanced tab, you can prevent writing back if a specific column that should not be empty contains null values. You can also rename native fields and specify a different column name to be written back. [Learn more about advanced writeback settings.](settings/advanced-settings.md)

<figure><img src="../../.gitbook/assets/image (681).png" alt=""><figcaption><p>Advanced writeback settings</p></figcaption></figure>

**STEP 6:** After configuring writeback settings, close the side panel and click the Writeback button. A notification window will display the progress and status of the writeback.

<figure><img src="../../.gitbook/assets/image (682).png" alt=""><figcaption><p>Writeback initiated</p></figcaption></figure>

After performing an initial writeback, you may need to add or remove visual parameters as you build your report. Any table structure changes required in the destination due to adding or removing visual parameters will be displayed in a notification window. You can choose whether to drop the existing table and re-create it with the new structure before writing back.

<figure><img src="../../.gitbook/assets/1.5. Writeback table mismatch.png" alt=""><figcaption><p>Table mismatch notification</p></figcaption></figure>

When the number of rows being written back exceeds a threshold, you'll need to enable a temporary staging table in the destination config. Writeback will fail unless the staging table option is enabled.

<figure><img src="../../.gitbook/assets/image (1248).png" alt=""><figcaption><p>Notification to enable temporary staging table</p></figcaption></figure>

**STEP 7:** Click the logs button to navigate to the writeback log console and view details like the milestones, payload size, duration of the writeback, etc. [Learn more about writeback logs.](logs.md)

<figure><img src="../../.gitbook/assets/image (683).png" alt=""><figcaption><p>Writeback logs</p></figcaption></figure>

#### Resources

[Writeback data and comments using Inforiver](https://inforiver.com/writeback-powerbi/)

[Power BI Writeback is as easy as 1-2-3: A Step-By-Step Tutorial](https://inforiver.com/blog/writeback/power-bi-data-writeback-123-step-by-step-tutorial/)

[Write back data & comments to a database or file](https://inforiver.com/blog/writeback/write-back-data-comments-database-file-powerbi/)

[5 Reasons why Writeback is required in a Modern BI Stack](https://inforiver.com/blog/writeback/5-reasons-why-writeback-is-required-in-a-modern-bi-stack/)

[Why Writeback using Power BI + Power Apps is Not for Everyone](https://inforiver.com/blog/writeback/writeback-using-powerbi-powerapps-not-for-everyone/)

[10 Key Considerations for Choosing a Writeback Solution in Power BI](https://inforiver.com/blog/writeback/writeback-power-bi-10-key-considerations/)
