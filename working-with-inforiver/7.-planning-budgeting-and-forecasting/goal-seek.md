# Goal Seek

In the last section, we looked into What-if analysis and simulations, which involved modifying or simulating one or more input values to obtain new output values or the totals.

Goal Seek is a also type of What-if analysis, except in this method, we specify the desired output or goal value to calculate the necessary input value to achieve the goal.

Let us take the following example where the product revenue for each region is calculated by multiplying the sale price with the number of units sold. This is accomplished by [inserting a formula measure](../4.-adding-business-logic-and-formulae/insert-calculated-columns.md#id-1.-visual-measure) as shown below.

<figure><img src="../../.gitbook/assets/image (571).png" alt=""><figcaption><p>Revenue Calculation</p></figcaption></figure>

The formula measure gets inserted and the grand total is also calculated.

<figure><img src="../../.gitbook/assets/image (580).png" alt=""><figcaption><p>Formula measure for Revenue inserted</p></figcaption></figure>

In the example above, the total revenue for the _Canada_ region is 219.40m. Let us assume we are seeking a goal of 400m as the desired revenue.&#x20;

Now, for the desired _**revenue**_ to be achieved through Goal Seek, we will choose to change one of its drivers - the _**Units Sold**_. Note that you can change only one driver at a time. Therefore, let us keep the _**Sale Price**_ fixed.

1. Input values in the native columns cannot be changed through Goal Seek. So we will create a [copy of it as a data input column](../4.-adding-business-logic-and-formulae/insert-manual-input-columns/insert-manual-input-columns.md#ii-copy-from-another-series) to change it. In this example, a data input column has been created for the _Units Sold_ driver.&#x20;

<figure><img src="../../.gitbook/assets/image (581).png" alt=""><figcaption><p>Create Data Input Column for <em>Units Sold</em></p></figcaption></figure>

2. You can also update the formula accordingly by including this data input column (Units Sold) in place of the native column.

<figure><img src="../../.gitbook/assets/image (573).png" alt=""><figcaption><p>Data input column in the formula</p></figcaption></figure>

3. Click on the required cell (Canada>Grand Total>Revenue) and select **Insert -> Goal Seek.**

<figure><img src="../../.gitbook/assets/image (574).png" alt=""><figcaption><p>Click 'Goal Seek'</p></figcaption></figure>

{% hint style="info" %}
The goal seek option gets enabled only when you click on a cell containing a formula or aggregation like sum, product, etc.
{% endhint %}

4. In the pop-up window, enter the desired goal value of 400m.

<figure><img src="../../.gitbook/assets/image (719) (2).png" alt=""><figcaption><p>Enter the goal value for revenue</p></figcaption></figure>

5. Verify the target cell and its underlying formula. Then choose which of its drivers needs to be changed from the drop-down as shown below. We will choose _Units Sold_ since we want to adjust the quantity sold to reach the desired revenu&#x65;_._&#x20;

<figure><img src="../../.gitbook/assets/image (721) (1).png" alt=""><figcaption><p>Select the driver to be changed</p></figcaption></figure>

6. You can either apply the changes to all input rows and columns or [choose which rows and column measures should be changed](goal-seek.md#applying-goal-seek-results-to-specific-rows-and-columns) to meet the desired goal value. Let us first apply changes to all the input rows and columns.
7. Click **Run** and then **Apply** to make the changes.

<figure><img src="../../.gitbook/assets/image (723) (1).png" alt=""><figcaption><p>Apply Goal Seek</p></figcaption></figure>

A new set of values is updated for the _Units Sold_ to meet the specified revenue. The new values of both measures - the units sold and the revenue are distributed to the child rows automatically.

<figure><img src="../../.gitbook/assets/image (578).png" alt=""><figcaption><p>Results of Goal Seek</p></figcaption></figure>

If you expand the column hierarchy, you can see that Inforiver also distributes the new values to the periods accordingly.

<figure><img src="../../.gitbook/assets/image (579).png" alt=""><figcaption><p>Period-wise Distribution of the results of Goal Seek</p></figcaption></figure>

**Note:** Goal Seek can also be applied to measures in rows.

<figure><img src="../../.gitbook/assets/image (582).png" alt=""><figcaption><p>Goal Seek applied on measures in rows</p></figcaption></figure>

### Applying Goal Seek Results to Specific Rows and Columns

Assume you want to meet the goal value by modifying the values of specific products or business units during a particular time of the year. In such cases, you can choose which input rows and columns should be changed to achieve the desired result.

In the example below, we set the same desired revenue of 400 million for the _Canada_ region. However, this time we intend to achieve this goal by increasing the sales of only the following products - _Amarilla_, _Carretera_, and _Montana_. We also want to change these values for the third and fourth quarters, excluding the rest.

This can be done by selecting the above-specified rows and columns as below.

<figure><img src="../../.gitbook/assets/4.1.1. filtering in goal seek.png" alt=""><figcaption><p>Applying Goal Seek to selected rows and columns</p></figcaption></figure>

In the result below, only the selected rows and columns have been modified to meet the goal.

<figure><img src="../../.gitbook/assets/4.1.2. filtering in goal seek-2.png" alt=""><figcaption><p>Results of Goal Seek</p></figcaption></figure>



**Note:** The goal seek function can also be used on formula cells referencing a column in their formulas - such as COLUMN.PARENT, COLUMN.TOTAL, etc.

In the example below, goal-seek is applied on the target cell which uses a formula with a column referencing function, [COLUMN.PARENT](../../formula-syntax/identifiers/column.parent.md).&#x20;

<figure><img src="../../.gitbook/assets/4.2.2..png" alt=""><figcaption><p>Goal Seek is applied on a target cell referencing a column</p></figcaption></figure>

### Referencing forecasts

Inforiver can adjust open forecasts to match a defined target value. Let’s consider a report that captures the projected revenue based on the quantity and sales. The report contains a forecasted quantity field as well as a projected quantity data input field. The formula uses the projected quantity for closed periods and the forecast quantity for open periods. When you set a goal for the Revenue measure, Inforiver will adjust the forecast quantity to align with the goal.

<figure><img src="../../.gitbook/assets/image (1099).png" alt=""><figcaption><p>Forecat measures in goal seek</p></figcaption></figure>
