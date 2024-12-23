# Query transformations

Infobridge provides a wide range of transformations to pivot, aggregate, join, merge, and append queries. Let's dive in!&#x20;

<figure><img src="../.gitbook/assets/2024-12-23_08h31_43.png" alt=""><figcaption><p>Query transformations</p></figcaption></figure>

### 1. Duplicating queries

You can create a copy or take a backup of your query before applying transformations. You can either hover over the query name and select **Duplicate** from the context menu or you can click the **Duplicate Query** option from the Home ribbon.

<figure><img src="../.gitbook/assets/2024-12-23_08h40_52.png" alt=""><figcaption><p>Duplicating queries</p></figcaption></figure>

### 2. Pivoting dimensions and measures

Use the **Pivot Table** option to easily re-structure your dimensions and measures and select the aggregation for totals and subtotals.

<figure><img src="../.gitbook/assets/2024-12-23_08h54_18.png" alt=""><figcaption><p>Pivot table interface</p></figcaption></figure>

#### 2.1. Converting rows into columns

You can pivot row and column dimensions by dragging them into the respective buckets. Let's look at how to convert the Region column dimension into a row dimension.

<figure><img src="../.gitbook/assets/2024-12-23_08h57_48.png" alt=""><figcaption><p>Region column dimension</p></figcaption></figure>

Drag the Region dimension from the Columns bucket to the Rows bucket to pivot the columns into rows.

<figure><img src="../.gitbook/assets/Untitled Project (7).gif" alt=""><figcaption><p>Column to row conversion</p></figcaption></figure>

#### 2.2. Aggregating numeric measures

When you enable totals and subtotals, you can also specify the type of aggregation to apply: sum/average/minimum/maximum.

<figure><img src="../.gitbook/assets/2024-12-23_09h10_25.png" alt=""><figcaption><p>Aggregation type</p></figcaption></figure>

In this query, we've applied summation for the Profit measure and average for the Sales measure.

<figure><img src="../.gitbook/assets/2024-12-23_09h12_56.png" alt=""><figcaption><p>Aggregated measures</p></figcaption></figure>

#### 2.3. Converting text dimensions into measures

You can convert text dimensions into measures and vice versa. Drag the dimension into the Values bucket to convert it into a measure.





