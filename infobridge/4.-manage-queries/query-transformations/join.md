---
description: >-
  Explore how to leverage joins to retrieve data from multiple tables using a
  related column.
---

# Join

Joins are widely used to fetch or lookup data from multiple tables based on a related column. Inforbridge supports 4 types of joins:

* **Inner join**: Returns the matching records between 2 tables.
* **Left join:** Returns all records from the base(left) table and matching records from the right table.
* **Right join:** Returns all records from the right table and matching records from the base table.
* **Full outer join:** Returns all records when there is a match in either table.

We'll take a simple regional sales table to demonstrate joins.&#x20;

<figure><img src="../../../.gitbook/assets/image (2) (1) (1) (1) (1).png" alt=""><figcaption><p>Regional sales</p></figcaption></figure>

We can fetch the tax and rate type for each region based on the related column - rate type ID.

<figure><img src="../../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Tax rate table</p></figcaption></figure>

The resultant joined table would look like this if we were to use an inner join. Notice how the LATAM record has been dropped as it does not have a matching rate in the second table.

<figure><img src="../../../.gitbook/assets/image (3) (1).png" alt=""><figcaption><p>Region table enriched with tax rates - inner join</p></figcaption></figure>

We can use a left outer join(or full outer join) to display the LATAM region, although it doesn't have a matching tax rate. The tax rate and rate type fields will be blank for the LATAM record when we use a left outer join.

<figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Region data with tax rates - left join</p></figcaption></figure>

Let's look at a use case in Infobridge where we can apply joins. Our base report contains the actuals and plan across various regions. We need to get the tax rates for each month.

<figure><img src="../../../.gitbook/assets/image (1333).png" alt=""><figcaption><p>Base report</p></figcaption></figure>

The monthly tax rates are in a different query that can be pulled using the common column - Month.

<figure><img src="../../../.gitbook/assets/image (1334).png" alt=""><figcaption><p>Monthly tax rates</p></figcaption></figure>

Let's select the **Join Query** option from the Data ribbon. Select "AC" as the base query and "Tax Rates" as the Query to join from the dropdowns. Choose "Month" as the Join Column. Select "Inner" as the Join Type.

<figure><img src="../../../.gitbook/assets/image (1335).png" alt=""><figcaption><p>Join query configuration</p></figcaption></figure>

The resultant join query contains the columns from both queries. You can delete the additional "Month" dimension from the Pivot Table window.

<figure><img src="../../../.gitbook/assets/image (1336).png" alt=""><figcaption><p>Joined query</p></figcaption></figure>
