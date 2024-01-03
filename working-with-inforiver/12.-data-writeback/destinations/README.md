---
description: Setting up writeback destinations in Inforiver Enterprise
---

# Destinations

Inforiver supports fast writeback setup and execution for several types of data destinations

* **Database/ Data warehouses/ Data lake:** Azure SQL, SQL Server, Synapse Analytics Dedicated SQL Pool, Azure Data Lake, Fabric lakehouse, Fabric warehouse, Dataverse, Databricks, Snowflake, BigQuery, Amazon Redshift, SAP HANA, Oracle, SingleStore,  PostgreSQL, MySQL,
* **File Destinations:** OneDrive, SharePoint
* **Webhook URLs:** Can be used to trigger workflows in iPaaS such as Power Automate and Logic Apps)

Configuring writeback destination(s) is straightforward and involves the same procedure (picture below) for any destination.

<figure><img src="../../../.gitbook/assets/image (68).png" alt=""><figcaption><p>Navigating to Inforiver writeback destination setup</p></figcaption></figure>

A list of destinations will be displayed for the users to select from.&#x20;

<figure><img src="../../../.gitbook/assets/image (365).png" alt=""><figcaption></figcaption></figure>

Configuring destinations for writeback is a straightforward process that will be covered in the upcoming sections.

After configuring the destination, you can choose whether the destination should be **client-managed** or **inforiver-managed**.  If you wish to restrict access to the database, opt for client-managed destinations.

* For Inforiver-managed destinations, creating the writeback table will be done automatically by Inforiver. Requisite permissions on the table need to be provided to Inforiver.
* For client-managed destinations, Inforiver will generate the scripts. You can manually execute them against the database.

<figure><img src="../../../.gitbook/assets/image (236).png" alt=""><figcaption><p>Destination management</p></figcaption></figure>

You can also set the decimal precision i.e. the number of digits after the decimal point to be written back to the destination.

<figure><img src="../../../.gitbook/assets/image (359).png" alt=""><figcaption></figcaption></figure>
