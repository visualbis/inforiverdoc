# Pivot table

### Pivoting dimensions and measures

Use the **Pivot Table** option to easily re-structure your dimensions and measures and select the aggregation for totals and subtotals.

<figure><img src="../../.gitbook/assets/2024-12-23_08h54_18.png" alt=""><figcaption><p>Pivot table interface</p></figcaption></figure>

### 1. Converting rows into columns

You can pivot row and column dimensions by dragging them into the respective buckets. Let's look at how to convert the Region column dimension into a row dimension.

<figure><img src="../../.gitbook/assets/2024-12-23_08h57_48.png" alt=""><figcaption><p>Region column dimension</p></figcaption></figure>

Drag the Region dimension from the Columns bucket to the Rows bucket to pivot the columns into rows.

<figure><img src="../../.gitbook/assets/Untitled Project (7).gif" alt=""><figcaption><p>Column to row conversion</p></figcaption></figure>

### 2. Aggregating numeric measures

When you enable totals and subtotals, you can also specify the type of aggregation to apply: sum/average/minimum/maximum.

<figure><img src="../../.gitbook/assets/2024-12-23_09h10_25.png" alt=""><figcaption><p>Aggregation type</p></figcaption></figure>

In this query, we've applied summation for the Profit measure and average for the Sales measure.

<figure><img src="../../.gitbook/assets/2024-12-23_09h12_56.png" alt=""><figcaption><p>Aggregated measures</p></figcaption></figure>

### 3. Converting text dimensions into measures

You can convert text dimensions into measures and vice versa. Drag the dimension into the Values bucket to convert it into a measure.

### 4. Concatenating text measures

Use the **Concat** option to aggregate strings from multiple rows into a single string, with a delimiter of your choice. For instance, you can concatenate all the accounts under a particular segment and analyze data at a higher granularity, without losing any information.

<figure><img src="../../.gitbook/assets/2024-12-23_10h33_12.png" alt=""><figcaption><p>Concatenating text measures with a delimiter</p></figcaption></figure>

Individual accounts are rolled up at Account type level, providing a concise summary of the dataset. The aggregated rows can then be consumed in other destination visuals.

<figure><img src="../../.gitbook/assets/2024-12-23_10h37_34.png" alt=""><figcaption><p>Aggregated text measure</p></figcaption></figure>
