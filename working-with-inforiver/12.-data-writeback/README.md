# 12. Data writeback

Inforiver writeback allows a user to export and save a report table to destinations of different types including file destinations, data warehouses, and data lake storage.&#x20;

Inforiver, unlike other BI tools, does not require IT overhead in terms of database setup and defining the structure of writeback tables in advance. Inforiver instead supports dynamic database configuration and table creation at run time and performs semi-structured, on-the-fly writeback to more than one destination at a time.

{% hint style="info" %}
Data writeback is an enterprise feature; you need to have a valid Inforiver Enterprise subscription.
{% endhint %}

## 1. Overview

The Writeback screen is accessed by going to the Export tab in the toolbar. Three buttons give you access to writeback and related settings.&#x20;

**Writeback** - Export report data to a destination.&#x20;

**Settings** - Configure writeback-related settings. Navigate to the [writeback settings](settings/) chapter to learn more.&#x20;

**Logs** - Every writeback event is logged with detailed information relevant to each writeback. Navigate to the [writeback logs](logs.md) chapter to learn more.



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

<figure><img src="../../.gitbook/assets/image (364).png" alt=""><figcaption></figcaption></figure>

To learn how to configure each destination in the above list, [navigate to this page](destinations/#overview).&#x20;

{% hint style="info" %}
The number of rows that can be written back is 200k rows for Excel and CSV and 250 rows for OneDrive and SharePoint
{% endhint %}

#### Resources

[Writeback data and comments using Inforiver](https://inforiver.com/writeback-powerbi/)

[Power BI Writeback is as easy as 1-2-3: A Step-By-Step Tutorial](https://inforiver.com/blog/writeback/power-bi-data-writeback-123-step-by-step-tutorial/)

[Write back data & comments to a database or file](https://inforiver.com/blog/writeback/write-back-data-comments-database-file-powerbi/)

[5 Reasons why Writeback is required in a Modern BI Stack](https://inforiver.com/blog/writeback/5-reasons-why-writeback-is-required-in-a-modern-bi-stack/)

[Why Writeback using Power BI + Power Apps is Not for Everyone](https://inforiver.com/blog/writeback/writeback-using-powerbi-powerapps-not-for-everyone/)

[10 Key Considerations for Choosing a Writeback Solution in Power BI](https://inforiver.com/blog/writeback/writeback-power-bi-10-key-considerations/)
