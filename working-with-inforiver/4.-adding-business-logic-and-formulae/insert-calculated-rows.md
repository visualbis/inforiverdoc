# Insert calculated rows

Inforiver provides an option to insert calculated rows using an intuitive formula editor. The Excel-like formula engine supports 50+ functions (logical, boolean, math functions and more). The formula editor provides syntax, examples and features such as autocomplete, multi-line support and more to help users create, and troubleshoot formulas.

{% embed url="https://lumel.wistia.com/medias/n67puv7p0m" %}

{% hint style="info" %}
Refer to [formula syntax](../../formula-syntax/) for a detailed list of functions, operators, and identifiers that can be used for calculations.
{% endhint %}

Let us take this example, where we have sales data by category and subcategory. Let's insert a row for Specialty Beverages which is calculated as the minimum of the other subcategories in Beverages across quarters.

<figure><img src="../../.gitbook/assets/4.1.1 Calculated row.png" alt=""><figcaption><p>Sales report</p></figcaption></figure>

a) Select the Tea & Coffee row above which we need to insert the row. In the 'Insert' tab, click on the 'Insert row' dropdown. Click on 'Calculated row'.

<figure><img src="../../.gitbook/assets/4.1.2 Calculated row.png" alt=""><figcaption><p>Inserting a calculated row</p></figcaption></figure>

b) A blank row gets inserted and a side panel opens up as shown.

<figure><img src="../../.gitbook/assets/4.1.3 Calculated row.png" alt=""><figcaption><p>Calculated row side panel</p></figcaption></figure>

### 1. Formula editor

a) Rename the title and click on the formula editor. In the 'Functions' tab, you can see a list of available functions.

<figure><img src="../../.gitbook/assets/4.1.4 Calculated row.png" alt=""><figcaption><p>Using functions</p></figcaption></figure>

b) As you start typing, the list of functions narrows down to match the entered text. Click on 'Min'.

<figure><img src="../../.gitbook/assets/4.1.5(2) Calculated row.png" alt=""><figcaption><p>Formula editor</p></figcaption></figure>

c) You can see the syntax for the function. Click on the arrow highlighted.

<figure><img src="../../.gitbook/assets/4.1.6 Calculated row.png" alt=""><figcaption><p>Formula syntax</p></figcaption></figure>

d) You can see an explanation of the arguments and examples.

<figure><img src="../../.gitbook/assets/4.1.7 Calculated row.png" alt=""><figcaption><p>Formula syntax and examples</p></figcaption></figure>

e) To insert a particular row, you can simply click on it when the cursor is placed in the formula editor.&#x20;

<figure><img src="../../.gitbook/assets/4.1.8 Calculated row.png" alt=""><figcaption><p>Inserting references by clicking a row</p></figcaption></figure>

f) The other way is to use the 'References' tab. To access Soda, you need to type Beverages.Soda. As you start typing, the references get narrowed down. Select 'Beverages'.

<figure><img src="../../.gitbook/assets/4.1.9 Calculated row.png" alt=""><figcaption><p>Inserting a reference from the dropdown</p></figcaption></figure>

g) Type a '.' after Beverages and select 'Soda' from the dropdown.

<figure><img src="../../.gitbook/assets/4.1.10 Calculated row.png" alt=""><figcaption><p>Traversing a hierarchy</p></figcaption></figure>

h) Finish typing the formula as shown below.

<figure><img src="../../.gitbook/assets/4.1.11 Calculated row.png" alt=""><figcaption><p>Formula entered</p></figcaption></figure>

{% hint style="info" %}
To see the underlying logic for calculated data, you can click on the cell to preview the formulae applied in the formula bar.
{% endhint %}

**Note:** While you can use the [SUM](../../formula-syntax/math-functions/sum.md) and [AVERAGE](../../formula-syntax/math-functions/average.md) functions to calculate the sum and average of rows respectively, you can also use the **Insert Sum of rows** and **Insert Avg of rows** options from the 'Insert Row' menu for the same.

Select the desired rows first holding down the Ctrl key and then select **Insert Sum of rows.**

<figure><img src="../../.gitbook/assets/image (517).png" alt=""><figcaption><p>Choose <strong>Insert Sum of rows</strong></p></figcaption></figure>

A new row containing the sum of the selected rows is created as shown below. You can use the side panel to make any additional changes. Observe how the formula editor has been automatically populated with the selected rows.

<figure><img src="../../.gitbook/assets/image (518).png" alt=""><figcaption><p>New Calculated Row - Sum</p></figcaption></figure>

Similarly, for calculating and inserting the average of rows, use **Insert Avg of rows.**

### 2. Include in total

a) Check the 'Include in total' checkbox as we need the Specialty Beverages value to be included in the Beverages total and the grand total. Click 'Create'.&#x20;

<figure><img src="../../.gitbook/assets/4.1.12 Calculated row.png" alt=""><figcaption><p>Including calculated row in total</p></figcaption></figure>

b) You can see that the row is renamed and the values are populated. There is also a formula bar on the top which shows the formula defined.&#x20;

Note that the grand total is now updated to 255m.

<figure><img src="../../.gitbook/assets/4.1.13 Calculated row.png" alt=""><figcaption><p>Calculated row inserted</p></figcaption></figure>

c) Let's uncheck the 'Include in total' checkbox and click 'Update'.

<figure><img src="../../.gitbook/assets/4.1.14 Calculated row.png" alt=""><figcaption><p>Excluding Specialty Beverages from total</p></figcaption></figure>

d) You can see that the grand total has now reverted back to the original value of 239m.

<figure><img src="../../.gitbook/assets/4.1.15 Calculated row.png" alt=""><figcaption><p>Specialty Beverages excluded from total</p></figcaption></figure>

### 3. Include in charts

a) Check the 'Include in charts' checkbox and click 'Update'.

{% hint style="info" %}
The 'Include in charts' checkbox is enabled only when the 'Include in total' option is unchecked.
{% endhint %}

<figure><img src="../../.gitbook/assets/4.1.16 Calculated row.png" alt=""><figcaption><p>Include in charts</p></figcaption></figure>

b) Let's now add a bar chart to 2022 Actuals. Click on the column and select the highlighted bar chart from the 'Home' tab.

<figure><img src="../../.gitbook/assets/4.1.17 Calculated row.png" alt=""><figcaption><p>Adding a bar chart</p></figcaption></figure>

c) Notice that the Specialty Beverages row is also visualized using the bar chart.

<figure><img src="../../.gitbook/assets/4.1.18 Calculated row.png" alt=""><figcaption><p>Bar chart shown for calculated row</p></figcaption></figure>

d) On unchecking the 'Include in charts' checkbox and clicking 'Update', you can see that the calculated row is no longer shown as charts.

<figure><img src="../../.gitbook/assets/4.1.19 Calculated row.png" alt=""><figcaption><p>Calculated row shown as numbers</p></figcaption></figure>

### 4. Evaluate column before rows

When inserting calculated rows, in some cases you might want the total to be the sum of the child columns whereas in other cases, it needs to follow the defined formula. This behaviour can be configured using the 'Evaluate column before rows' option.&#x20;

Let's consider an example where we are inserting the relative variance between two of the rows. In the below image, with 'Evaluate columns before rows' enabled, you can see that the variance for the grand total is calculated based on the grand total values of Pacific and Central.

<figure><img src="../../.gitbook/assets/4.1.20 Calculated row.png" alt=""><figcaption><p>Total value calculated based on formula</p></figcaption></figure>

When 'Evaluate columns before rows' is disabled, the grand total variance is calculated as the sum of Beverages and Water which is not the expected behaviour in this case.

<figure><img src="../../.gitbook/assets/4.1.21 Calculated row.png" alt=""><figcaption><p>Total value calculated as sum of category values</p></figcaption></figure>

### 5. Custom scaling

In certain cases, the values in calculated rows may not conform to the number scaling set at the report level. You can apply a custom scaling factor based on the nature of the calculation applied.

<figure><img src="../../.gitbook/assets/7.3. Custom scaling for calculated rows.png" alt=""><figcaption><p>Scaling Factor</p></figcaption></figure>

### 6. Bind for Cross filter/RLS

Select this option to enable RLS (Row-level Security) to the inserted rows. You can bind the inserted row to any existing row or a dimension member for secure bi-directional cross filtering.&#x20;

For example, the image below shows the newly inserted row being bound to the member _'Technology'_ in the dimension _'Category'._ This is done by choosing 'Dimension Member' in the Selection Type and then selecting the required dimension and member.&#x20;

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption><p>Binding for Cross filtering/RLS</p></figcaption></figure>

Note: You can also choose 'Row' as the Selection Type and select any existing row in the report.

Only the users with permission to access the 'Technology' category can view the newly added row as shown below. This way, you can bind the inserted rows to their respective categories.

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption><p>RLS added to the new row</p></figcaption></figure>

#### Resources

[Insert Formulas, Columns and Aggregation](https://www.youtube.com/watch?v=hjPAbuYJUSc)

[Visual calculations using Inforiver](https://inforiver.com/webinars/visual-level-formula-calculations-powerbi/)

[Implement SUM measure totals in Power BI (without using DAX)](https://inforiver.com/blog/general/sum-measure-totals-powerbi-no-dax/)

[Excel-like MoM, QoQ, YoY % Calculations in Rows in Power BI](https://inforiver.com/blog/general/excel-like-mom-qoq-yoy-calculations-power-bi/)
