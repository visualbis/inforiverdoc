---
description: >-
  In the module, we'll explore how to use append functions to combine data with
  the same structure from multiple tables.
---

# Append

You can have data sourced from multiple systems that need to be unified into a single table. Consider the employee bonus data from different departments:

<figure><img src="../../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>HR department</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>IT department</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (4) (1) (1) (1) (1).png" alt=""><figcaption><p>Sales and marketing department</p></figcaption></figure>

We need to combine the department-wise data to get an organizational level view of the bonus allocated to each department. The **Append** function is used in such scenarios where the structure (data type and number of columns) of all the source tables is exactly the same. The table below shows the appended data from all departments.&#x20;

<figure><img src="../../../.gitbook/assets/image (5) (1).png" alt=""><figcaption><p>Appended data</p></figcaption></figure>

We'll look at how to append data in Infobridge. The SALES bridge has regional sales from multiple countries.

<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption><p>Sales bridge with sales across different regions</p></figcaption></figure>

Click on **Append Query**. We'll be able to select the queries to combine. You may have sales and budgets in the same bridge, in which case you need to select only the queries that need to be appended.

<figure><img src="../../../.gitbook/assets/image (8).png" alt=""><figcaption><p>Selecting queries to append</p></figcaption></figure>

The selected queries will be displayed in the Append dialog box. We can click Apply.

<figure><img src="../../../.gitbook/assets/image (9).png" alt=""><figcaption><p>Append query dialog box</p></figcaption></figure>

The consolidated data is stored in a new query that can either be written back or cascaded to a target report.

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption><p>Appended data</p></figcaption></figure>
