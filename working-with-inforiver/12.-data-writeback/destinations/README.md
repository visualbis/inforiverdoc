---
description: Setting up writeback destinations in Inforiver Writeback Matrix.
---

# Destinations

Inforiver supports fast writeback setup and execution for several types of data destinations

* **Database/ Data warehouses/ Data lake:** Azure SQL, SQL Server, Synapse Analytics Dedicated SQL Pool, Azure Data Lake, Fabric lakehouse, Fabric warehouse, Dataverse, Databricks, Snowflake, BigQuery, Amazon Redshift, SAP HANA, Oracle, SingleStore,  PostgreSQL, MySQL,
* **File Destinations:** OneDrive, SharePoint
* **Webhook URLs:** Can be used to trigger workflows in iPaaS such as Power Automate and Logic Apps)

Configuring writeback destination(s) is straightforward and involves the same procedure (picture below) for any destination.

<figure><img src="../../../.gitbook/assets/image (68) (1).png" alt=""><figcaption><p>Navigating to Inforiver writeback destination setup</p></figcaption></figure>

A list of destinations will be displayed for the users to select from.&#x20;

<figure><img src="../../../.gitbook/assets/image (908).png" alt=""><figcaption><p>Destinations organized by category</p></figcaption></figure>

Configuring destinations for writeback is a straightforward process that will be covered in the upcoming sections.

### Generic destination settings

#### **1. Client-managed and Inforiver-managed destination**

After configuring the destination, you can choose whether the destination should be **client-managed** or I**nforiver-managed**.  If you wish to restrict access to the database, opt for client-managed destinations.

* **Enable automatic writeback management:** For Inforiver-managed destinations, Inforiver will automatically create the writeback table. However, Inforiver needs to be provided with the required permissions on the table.

<figure><img src="../../../.gitbook/assets/image (1062).png" alt=""><figcaption><p>Inforiver managed destinations</p></figcaption></figure>

* For client-managed destinations, Inforiver will generate the scripts. You can manually execute them against the database.

<figure><img src="../../../.gitbook/assets/image (1063).png" alt=""><figcaption><p>Client managed destination</p></figcaption></figure>

#### 2. Column config

* **Decimal Precision**

Inforiver rounds off all numeric values including percentages to a specified number of decimal points as per your configuration instructions. When you create the first connection, you can specify decimal precision for all connections in that report.

{% hint style="info" %}
Inforiver supports a maximum precision of 10 digits.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (1066).png" alt=""><figcaption><p>Setting the decimal precision for destinations</p></figcaption></figure>

When you apply the decimal precision shown in the image above, Inforiver writes back values (in this example, to Snowflake) rounded off to 5 decimal places.

<figure><img src="../../../.gitbook/assets/1.4.2.WB PErcentage values output.png" alt=""><figcaption><p>Writeback percentage values</p></figcaption></figure>

* **Text length**

When you add destinations, you can restrict text fields to 512 characters or allow writeback up to the maximum limit supported by the backend.

<figure><img src="../../../.gitbook/assets/image (1067).png" alt=""><figcaption><p>Setting the text length</p></figcaption></figure>

#### 3. Batch writeback

When you configure individual writeback destinations, you'll notice an option for batched writeback wherever applicable (batched writeback is not possible for destinations like Sharepoint, Rest API, OneDrive, etc). If your writeback payload exceeds 50k records, Inforiver can split the payload into multiple chunks and write them back batch-by-batch.

You can specify whether you will use a temporary table to hold the batched data.

<figure><img src="../../../.gitbook/assets/image (928).png" alt=""><figcaption><p>Temporary staging table configuration</p></figcaption></figure>

* To use this feature, enable the checkbox as shown in the image above.
* You can specify a custom table name or use the default table created by Inforiver to store batched data.

You can analyze the writeback log, which will capture how the payload has been split into multiple chunks and processed in parallel for a performance boost.

<figure><img src="../../../.gitbook/assets/3.2. Writeback batch chunks in log.png" alt=""><figcaption><p>Writeback logs for batched data</p></figcaption></figure>
