---
description: Setting up writeback destinations in Inforiver Enterprise
---

# Destinations

Inforiver supports fast writeback setup and execution for several types of data destinations

* **Database/ Data warehouses/ Data lake:** Azure SQL, SQL Server, Synapse Analytics Dedicated SQL Pool, Azure Data Lake, Fabric lakehouse, Fabric warehouse, Dataverse, Databricks, Snowflake, BigQuery, Amazon Redshift, SAP HANA, Oracle, SingleStore,  PostgreSQL, MySQL,
* **File Destinations:** OneDrive, SharePoint
* **Webhook URLs:** Can be used to trigger workflows in iPaaS such as Power Automate and Logic Apps)

Configuring writeback destination(s) is straightforward and involves the same procedure (picture below) for any destination.

<figure><img src="../../../.gitbook/assets/image (68) (1).png" alt=""><figcaption><p>Navigating to Inforiver writeback destination setup</p></figcaption></figure>

A list of destinations will be displayed for the users to select from.&#x20;

<figure><img src="../../../.gitbook/assets/image (365).png" alt=""><figcaption></figcaption></figure>

Configuring destinations for writeback is a straightforward process that will be covered in the upcoming sections.

### Generic destination settings

#### **1. Client-managed and Inforiver-managed destination**

After configuring the destination, you can choose whether the destination should be **client-managed** or **inforiver-managed**.  If you wish to restrict access to the database, opt for client-managed destinations.

* For Inforiver-managed destinations, creating the writeback table will be done automatically by Inforiver. Requisite permissions on the table need to be provided to Inforiver.
* For client-managed destinations, Inforiver will generate the scripts. You can manually execute them against the database.

<figure><img src="../../../.gitbook/assets/image (236).png" alt=""><figcaption><p>Destination management</p></figcaption></figure>

#### 2. Decimal Precision

Inforiver rounds off all numeric values including percentages to a specified number of decimal points as per your configuration instructions. When you create the first connection, you can specify decimal precision for all connections in that report.

<figure><img src="../../../.gitbook/assets/1.4.1.WB PErcentage values.png" alt=""><figcaption><p>Decimal precision</p></figcaption></figure>

When you apply the decimal precision shown in the image above, Inforiver writes back values (in this example, to Snowflake) rounded off to 5 decimal places.

<figure><img src="../../../.gitbook/assets/1.4.2.WB PErcentage values output.png" alt=""><figcaption><p>Writeback percentage values</p></figcaption></figure>

#### 3. Batch writeback

When you configure individual writeback destinations, you'll notice a Btach Writeback option wherever applicable (batched writeback is not possible for destinations like Sharepoint, Rest API, OneDrive, etc). If your writeback payload exceeds 50k records, Inforiver can split the payload into multiple chunks and write them back batch-by-batch.

<figure><img src="../../../.gitbook/assets/image (760).png" alt=""><figcaption><p>Batched writeback configuration</p></figcaption></figure>

* Enable the Batched Write checkbox to use this feature.
* You can specify a custom table name or use the default table created by Inforiver to store batched data.

You can analyze the writeback log, which will capture how the payload has been split into multiple chunks and processed in parallel for a performance boost.

<figure><img src="../../../.gitbook/assets/3.2. Writeback batch chunks in log.png" alt=""><figcaption><p>Writeback logs for batched data</p></figcaption></figure>
