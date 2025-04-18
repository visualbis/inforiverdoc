# 14. Manage aggregation

While working with Power BI table/matrix reports, we would sometimes like to apply custom aggregations for the measures in a specific report (e.g., average quantity sold) instead of using the default aggregation used in a data model (e.g., the sum of quantity sold).&#x20;

Inforiver’s aggregation feature allows you to override the native Power BI aggregation for measures without having to make extensive model-level changes. You can set aggregation at measure/column-level, hierarchy-level, and specify aggregation for the row and column subtotals/grand totals.

**Row aggregation:** You can specify the aggregation to be applied on row subtotals and grand total.

<figure><img src="../../.gitbook/assets/image (776) (1).png" alt=""><figcaption><p>Row aggregation</p></figcaption></figure>

**Column aggregation: Y**ou can specify the aggregation to be applied on the column grand total and subtotals.

<figure><img src="../../.gitbook/assets/image (777) (1).png" alt=""><figcaption><p>Column aggregation</p></figcaption></figure>

Click the **Aggregation** button in the **Insert** ribbon to open the **Manage Aggregation** interface.

### 1. Measure level aggregation

You can specify the row and column aggregation for individual measures and columns from the **Measure** tab. Select the aggregation type from the dropdown against the measure name.

<figure><img src="../../.gitbook/assets/image (778) (1).png" alt=""><figcaption><p>Measure level row and column aggregation</p></figcaption></figure>

* **Sum** set as row aggregation for 2024 Plan: The sum of the child rows will be used to populate the row subtotal and grand total.
* **Maximum** set as row aggregation for 2024 Actuals: The maximum value in the child rows will be used to populate the row subtotal and grand total.
* **Minimum** set as column aggregation for 2024 Actuals and Plan: The minimum values in the columns will be used as the column grand total and subtotal.

### 2. Aggregation types

{% hint style="info" %}
The interface shown in the screenshots in this section has changed slightly in newer versions but the functionality remains the same.
{% endhint %}

#### Native

By default, the 'Native' option is applied which follows the native summarization set in Power BI.&#x20;

<figure><img src="../../.gitbook/assets/image (200).png" alt=""><figcaption><p>Native aggregation at report level</p></figcaption></figure>

#### None

Choosing 'None' performs no aggregations for the selected measure or hierarchy. In the example below, the 'Discount' measure is not aggregated.

<figure><img src="../../.gitbook/assets/image (7) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Aggregation is 'None'</p></figcaption></figure>

#### Sum

'Sum' aggregation displays the sum of the immediate child nodes as the aggregate. In the highlighted example, the 'Computers' category is the sum of its immediate child nodes.

<figure><img src="../../.gitbook/assets/image (201).png" alt=""><figcaption><p>Sum aggregation type at report level</p></figcaption></figure>

#### Minimum

'Minimum' aggregation displays the minimum value of the immediate child nodes as the aggregate. In the below example, the 'Computers' category displays the minimum value of its immediate child nodes which is 'Computers Accessories'.

<figure><img src="../../.gitbook/assets/image (202).png" alt=""><figcaption><p>Minimum aggregation type at report level</p></figcaption></figure>

#### Maximum

'Maximum' aggregation displays the maximum value of the immediate child nodes as the aggregate. In the below image, the 'Computers' category displays the maximum value of its immediate child nodes which is 'Projectors and Screens'.

<figure><img src="../../.gitbook/assets/image (203).png" alt=""><figcaption><p>Maximum aggregation type at report level</p></figcaption></figure>

#### Average (Children)

'Average (Children)' aggregation displays the average value of the immediate child nodes as the row aggregation. In the below example,  'Computers' category is calculated as the average of the immediate child nodes i.e. the 'SubCategory' field.

<figure><img src="../../.gitbook/assets/image (204).png" alt=""><figcaption><p>Average(children) aggregation type at report level</p></figcaption></figure>

#### Average (Leaf)

'Average (Leaf)' aggregation displays the average value of all the leaf nodes of the row category as the row aggregation. In the below example, 'Computers' is calculated as the average of the leaf nodes i.e. the 'Class' field.

<figure><img src="../../.gitbook/assets/image (205).png" alt=""><figcaption><p>Average(leaf) aggregation type at report level</p></figcaption></figure>

#### Standard deviation

'Standard deviation' aggregation displays the standard deviation of the child rows as the aggregate. In the below example, 'Computers' is calculated as the standard deviation of its immediate child nodes.

<figure><img src="../../.gitbook/assets/image (206).png" alt=""><figcaption><p>Standard Deviation as aggregation type at report level</p></figcaption></figure>

#### Visible rounding

'Visible rounding' aggregation rounds off values in a way that the individual values add up properly to the subtotal' and grand total. This is a very common requirement in external financial statement reporting such as the income statement and balance sheet reporting.

<figure><img src="../../.gitbook/assets/image (207).png" alt=""><figcaption><p>Visible Rounding as aggregation type at report level</p></figcaption></figure>

#### Weighted Average

In weighted average aggregation, each child value in a row category is multiplied with weights taken from another measure which are then summed and divided by the total weight.&#x20;

Weighted moving average = (w1\*a1 + w2\*a2 +...+wn\*an) / (w1+w2+...+wn),

where

n= number of child rows in the row category

w1,w2,w3,....wn = weights (data from measure 1)

a1,a2,a3,........an = data from measure 2

This type of averaging is sometimes more accurate than simple averaging as it considers the varying importance of the data points. This also smoothens any price point fluctuations and is commonly used for inventory accounting, portfolio analysis, statistical research, planning, and forecasting.&#x20;

The example below calculates the weighted average using the costs and quantities in each region.

i.e., Average Cost for _**Paseo**_ = \[(Quantity\*Cost) _in Canada_  + (Quantity\*Cost) _in_ _France_ + (Quantity\*Cost) _in United States_ + (Quantity\*Cost) _in Mexico_ + (Quantity\*Cost) _in Germany_ ] / Total Quantity&#x20;

Note that weighted average is a row aggregation method – only the total and subtotal rows will reflect the calculation.

<figure><img src="../../.gitbook/assets/image (626).png" alt=""><figcaption><p>Weighted Average as the row aggregation type for data input measure</p></figcaption></figure>

{% hint style="info" %}
'Weighted Average' aggregation can be applied only to data input, formula, and forecast measures.&#x20;
{% endhint %}

#### First

This aggregation type is often used in time-series data or any sequential dataset. The 'First' aggregation type displays the first value from the set of immediate child nodes. This is especially useful when we need to record the dataset's initial state or value.&#x20;

In the example below, we have captured the first month's value in a year.

<figure><img src="../../.gitbook/assets/image (1111) (1).png" alt=""><figcaption><p>'First' aggregation type </p></figcaption></figure>

#### Last

This aggregation type is used in time-series data or any sequential dataset. The 'Last' aggregation type displays the last value or the latest value from the set of immediate child nodes. This is useful when we need the most recent value in a dataset, especially when budgeting for the following year by carrying over the previous year's value.&#x20;

In the example below, we have captured the value from the last month of the year.

<figure><img src="../../.gitbook/assets/image (1112) (1).png" alt=""><figcaption><p>'Last' aggregation type</p></figcaption></figure>

#### Resources

[Change & manage aggregation in Power BI matrix](https://inforiver.com/blog/feature-highlights/define-visual-aggregation-power-bi-table-matrix/)
