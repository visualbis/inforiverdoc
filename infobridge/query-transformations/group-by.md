---
description: >-
  Learn how to aggregate and summarize detailed reports with the Group by
  transformation.
---

# Group by

## Using the Group by transformation to aggregate your data

We often need to summarize our data to identify metrics like the 'Total number of customers by region' or the 'Average sales per quarter'. You can use the Group by transformation to aggregate measures and summarize your data based on selected dimensions.

Let's look at a classic Employee table to demonstrate how the Group by function works.&#x20;

<figure><img src="../../.gitbook/assets/image (1136).png" alt=""><figcaption><p>Sample employee table</p></figcaption></figure>

Management would want to focus on metrics like the average salary by region or the minimum experience in each department. To capture insights like these, we need to group and aggregate the employee data, as shown.

<figure><img src="../../.gitbook/assets/image (1138).png" alt=""><figcaption><p>Summarized and aggregated data</p></figcaption></figure>

Let's look at how we can aggregate your planning data with Infobridge.

<figure><img src="../../.gitbook/assets/image (1140).png" alt=""><figcaption><p>Group by in Infobridge</p></figcaption></figure>

### Group by with a single measure

Let's find the minimum interest rate for each quarter. We need to choose _Quarter_ from the **Category** dropdown, _Minimum_ from **Operations 1** dropdown, and _InterestRate_ from the **Values** dropdown.

<figure><img src="../../.gitbook/assets/image (1141).png" alt=""><figcaption><p>Group by configuration</p></figcaption></figure>

&#x20;When you click Apply, Infobridge displays the minimum interest rate for each quarter:

<figure><img src="../../.gitbook/assets/image (1142).png" alt=""><figcaption><p>Grouped data for a single measure and dimension</p></figcaption></figure>

### Group by for multiple measures

Let's also calculate the average COGS and total sales for each quarter. Click the **Add Aggregation** link to summarize your data for additional measures.&#x20;

<figure><img src="../../.gitbook/assets/image (1143).png" alt=""><figcaption><p>Group by configuration for multiple measures</p></figcaption></figure>

The summarized data after applying the group by transformation is shown below.

<figure><img src="../../.gitbook/assets/image (1144).png" alt=""><figcaption><p>Grouping multiple measures</p></figcaption></figure>

### Group by for multiple dimensions

Let's capture more insights by aggregating the same measures for each quarter and country. When you want to summarize your data based on multiple dimension categories, you can select them from the **Category** dropdown.

<figure><img src="../../.gitbook/assets/image (1145).png" alt=""><figcaption><p>Grouping data based on multiple dimensions</p></figcaption></figure>

The summarized query after applying the group by transformation is shown below.

<figure><img src="../../.gitbook/assets/image (1146).png" alt=""><figcaption><p>Summarized data</p></figcaption></figure>
