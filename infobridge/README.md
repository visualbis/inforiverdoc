# Infobridge

Inforiver Writeback Matrix, version 3.0 comes with Infobridge, a no-code data integration, preparation, and transformation engine, transforming it into an advanced real-time collaborative and integrated planning and business reporting suite.

Infobridge lets you connect to multiple data sources and consolidate them into a single, unified report. It has a user-friendly transformation interface to perform some common data transformations on the data sources such as append, merge, pivot, and unpivot columns, group by, etc.

## Use-cases of InfoBridge

Common use-cases of Infobridge include:

1. **Regional & Global Budgeting:** Manage regional budgets with dedicated pages for each region, consolidated into a global budget page.
2. **Operational Expense Planning:** Plan expenses at a granular level (e.g., salary plans at the employee level) and consolidate them into broader expense categories.
3. **Financial Planning and Analysis:** Import sales and COGS data from product-level reports into consolidated P & L statements. Perform planning and forecasts on the consolidated data.
4. **Planning in Pharma & Manufacturing Industries:** Plan at the material level and aggregate data to higher levels like plant or product family.
5. **Cost Center Planning:** Perform planning at detailed levels (e.g., IT maintenance costs, miscellaneous costs within specific cost centers) and aggregate the data for executive dashboards.
6. **Capacity Planning:** Convert volume forecasts from the planning sheets into headcount and resource requirements.

## Why InfoBridge?

All the above use-cases typically require composite modeling, ETL and automation tools, complex DAX & SQL scripting, extensive BI expertise and IT overheads. This is where Infobridge can help. It combines the capabilities of Power Query, Power Automate, and the Inforiver Writeback engine to enable real-time data transformations inside your existing Power BI reports.

* **No code platform:** Infobridge offers a no-code experience for use cases that would normally demand intensive DAX and composite modelling.&#x20;
* **Visual data integration:** With Infobridge, you can seamlessly access data from any Inforiver or ValQ visual in near real-time. Pulling data from different visuals would typically require ETL expertise.
* **Pivoting data**: You can pivot and unpivot dimensions and measures on the fly. Adding new dimensions or pivoting data can be done with a few clicks instead of using complex SQL and DAX scripts.&#x20;
* **Writeback**: Infobridge allows the consolidation of multiple visuals into a single WB table. Without Infobridge, users would need to writeback to separate tables and maintain each of them.

## Infobridge integration with Inforiver

In the 3.0 version of Inforiver Writeback Matrix, we have added an InfoBridge tab in the Inforiver visual. In the context of Inforiver, one of InfoBridge's capabilities is to integrate data from separate visuals and write it back to a single table. This involves creating a bridge, adding sources to it, managing the integration, and performing writeback. Hence the guide is organized as follows:

1. [**Create Bridge:**](create-bridge.md) In Infobridge, a bridge is a workspace environment with a data transformation editor that allows you to integrate multiple data sources and transform them. You can create as many bridges based on how you want to integrate or prepare your data. The process of creating a new bridge is described in this section.
2. [**Add Source to Bridge:**](add-source-to-bridge.md) Data can come from different sources in various file formats. This section explains the steps to add and connect to different data sources.
3. [**Insert Rows from the bridge:** ](insert-rows-from-bridge.md)In this section, we look at the steps to pull data from a bridge source and insert it to the Inforiver visual. Specifically, we learn to insert rows from a bridge into a target visual. This section also covers how to set up the mapping of dimensions and measures between the visuals for seamless integration.
4. [**Insert measure from the bridge:**](insert-measure-from-bridge.md) In this section, we cover the steps on how to insert a measure from the bridge to an Inforiver visual.&#x20;
5. [**Manage Integration:**](manage-integration-of-visuals.md) Integration of reports require mapping the dimensions and measures between the reports which is already explained [here](insert-rows-from-bridge.md#mapping-dimensions-between-the-reports). In this section, we explain more about managing the integration.
6. [**Manage Bridges:**](manage-bridges.md) An Inforiver visual can be a part of several bridges. This section explains about managing them easily.
7. [**Bridge Interface:**](bridge-interface.md) When you create a bridge, you will have access to the transformation editor interface for that bridge. This section walks you through the bridge interface and the different options available.
