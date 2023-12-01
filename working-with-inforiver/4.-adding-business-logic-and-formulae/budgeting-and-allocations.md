# Budgeting & allocations

Inforiver provides an intuitive way of performing planning, budgeting & allocations through an editable table interface. You can create a new plan/budget based on an existing data series or from scratch (Zero-based Budgeting). While using hierarchies, you can spread data entered on a parent cell to its descendants (rows & columns), based on weights from other measures.&#x20;

## 1. Creating a series

Let's first look at the ways of creating a new series.

### i. From scratch (ZBB)

Let’s assume you would like to create a zero-based budget for the year 2023.&#x20;

This can be achieved by creating a data input column as mentioned in the section [create a numeric input column](insert-manual-input-columns/insert-manual-input-columns.md#1.-create-a-column). The result is shown in the below image.

<figure><img src="../../.gitbook/assets/4.4.7 Number.png" alt=""><figcaption><p>Blank measure inserted</p></figcaption></figure>

### ii. Based on an existing series&#x20;

Let’s take an example where we would like to create a 2023 Plan based on the 2022 Plan (or the most recent forecast).

This can be achieved by creating a data input column as mentioned in the section [copy as data input](insert-manual-input-columns/insert-manual-input-columns.md#4.-copy-as-data-input). The result is shown in the below image.

<figure><img src="../../.gitbook/assets/4.4.30 Number.png" alt=""><figcaption><p>Measure created based on 2022 Plan</p></figcaption></figure>

## 2. Allocate totals

In this example, let's consider a zero-based budget for 2023.

<figure><img src="../../.gitbook/assets/7.2.1 ZBB.png" alt=""><figcaption><p>Zero-based budget for 2023</p></figcaption></figure>

Enter a value of 290m as the Q1 2023 Budget in the formula bar by double-clicking on the cell.&#x20;

<figure><img src="../../.gitbook/assets/7.2.2 ZBB.png" alt=""><figcaption><p>Entering a value at the total level</p></figcaption></figure>

There are two ways to allocate a value entered in a **total or subtotal** - [equally](budgeting-and-allocations.md#i-equal) or [based on weights](budgeting-and-allocations.md#ii-weight).

{% hint style="info" %}
The equal and weight options are not shown when you click on a cell at the child level. &#x20;
{% endhint %}

### i) Equal

a) After entering the value in the formula bar, press 'Enter'. By default, the values get distributed equally across all the categories and subcategories. Inforiver automatically highlights the updated values.

Note that the values have been rolled up to the grand total (Grand total -> 2023 Budget).

<figure><img src="../../.gitbook/assets/7.2.3 ZBB (1).png" alt=""><figcaption><p>Equal distribution</p></figcaption></figure>

b) Let's consider another example where we enter a budget at the grand total level. Double-click on the highlighted cell and enter 1.2b.

<figure><img src="../../.gitbook/assets/7.2.4 Equal.png" alt=""><figcaption><p>Update grand total value </p></figcaption></figure>

c) Once you click 'Enter', you can see the value distributed equally across categories, subcategories and quarters.

<figure><img src="../../.gitbook/assets/7.2.5 Equal.png" alt=""><figcaption><p>Equal distribution at grand total level</p></figcaption></figure>

### ii) Weight

In this case, we don't need an equal distribution. We need to allocate the budget proportionally based on 2022 actuals.&#x20;

a) Click on the context menu appearing on the cell with the value 1,200.0 and choose ‘Distribute by weights of 2022 Actuals’.

<figure><img src="../../.gitbook/assets/7.2.6 Weights.png" alt=""><figcaption><p>Distribution based on prior year values</p></figcaption></figure>

b) Once this option is selected, the 2023 Budget values are updated automatically across product categories & quarters by their relative contribution to 2022 Actuals.

<figure><img src="../../.gitbook/assets/7.2.7 Weights.png" alt=""><figcaption><p>Value gets redistributed based on weights</p></figcaption></figure>

## 3. Lock values

Values in data input columns can be locked either at a cell level or including all children (at a subtotal/total level). The cells that are locked are not affected by any of the allocation methods.

{% hint style="info" %}
A child node can be locked only when [row aggregation type](insert-manual-input-columns/insert-manual-input-columns.md#i-insert-a-new-empty-series) is set to Sum or Average.
{% endhint %}

### i) Lock this cell

Let’s consider a business case – There is an overall budget for 2023 which is distributed to the categories based on 2022 Actuals. Certain categories and their sub-categories have a fixed budget, and the budget has to be reallocated once these changes are made. Budgets for Juices and Soda are 500m and 350m respectively. &#x20;

This can be easily achieved using Inforiver as shown below.&#x20;

Note that we have inserted a [numeric data input ](budgeting-and-allocations.md#i.-from-scratch-zbb)column for 2023 Budget, entered the budget 1.2b and [distributed by 2022 Actuals](budgeting-and-allocations.md#ii-weight).&#x20;

a) Double-click on the Juices -> 2023 Budget cell and update the value as shown below.

<figure><img src="../../.gitbook/assets/7.2.8 Lock cell.png" alt=""><figcaption><p>Editing a cell</p></figcaption></figure>

b) Once you press enter, click on the context menu and select 'Lock this cell'.

<figure><img src="../../.gitbook/assets/7.2.9 Lock cell.png" alt=""><figcaption><p>Locking a cell</p></figcaption></figure>

c) The cell is greyed out indicating that it is locked from further changes.

<figure><img src="../../.gitbook/assets/7.2.10 Lock cell.png" alt=""><figcaption><p>Cell locked</p></figcaption></figure>

d) Update the budgets for Soda and lock the cell. Note that the overall budget has now become 1.28b.&#x20;

<figure><img src="../../.gitbook/assets/7.2.11 Lock cell.png" alt=""><figcaption><p>Budget for soda locked</p></figcaption></figure>

e) Let’s enter 1.2b again as the overall budget. The budgets get redistributed as shown below.&#x20;

<figure><img src="../../.gitbook/assets/7.2.12 Lock cell.png" alt=""><figcaption><p>Changes to the budget doesn't affect locked cells</p></figcaption></figure>

### ii) Lock all children

In some cases, you might want to lock all the children for a particular cell. For example, all the children across rows such as sub-regions and/or across columns such as quarters might need to be locked.

{% hint style="info" %}
Lock all children option is not shown when you click on a cell at the child level.
{% endhint %}

a) Click on Beverages -> 2023 Budget, and select 'Lock all children' from the context menu.

<figure><img src="../../.gitbook/assets/7.2.13 Lock children.png" alt=""><figcaption><p>Lock all children</p></figcaption></figure>

b) All the child cells get locked as shown in the below image.

<figure><img src="../../.gitbook/assets/7.2.14 Lock children.png" alt=""><figcaption><p>Child cells are locked</p></figcaption></figure>

c) Let's update the overall budget and see the effect on the child cells.

<figure><img src="../../.gitbook/assets/7.2.15 Lock children.png" alt=""><figcaption><p>Updating the budget</p></figcaption></figure>

d) The increase gets applied to Water and its subcategories across all quarters.

<figure><img src="../../.gitbook/assets/7.2.16 Lock children.png" alt=""><figcaption><p>Changes to the budget doesn't affect locked cells</p></figcaption></figure>

e) You can also lock at the sub-category level using the lock all children option. Note that only in the case of the grand total, the lock all children option is available.

<figure><img src="../../.gitbook/assets/7.2.17 Lock children.png" alt=""><figcaption><p>Lock all children at a subcategory level</p></figcaption></figure>

f) The four quarters are locked including the grand total cell.

<figure><img src="../../.gitbook/assets/7.2.18 Lock children.png" alt=""><figcaption><p>Juices across quarters locked</p></figcaption></figure>

### iii) Lock row

You may need to lock an entire row when [measures are displayed as rows](../2.-displaying-information/layout-options.md#a.-in-rows). Consider a business case wherein you need to [add a new measure](insert-manual-input-columns/insert-manual-input-columns.md#1.-create-a-column) to set the budgets for the next year.&#x20;

After creating a new measure titled 2023 Budget, click on the row gripper and select Lock Row to lock the entire row.

<figure><img src="../../.gitbook/assets/image (11) (3).png" alt=""><figcaption><p>Lock row on Measure in Rows</p></figcaption></figure>



The entire row is now greyed out, indicating that it is locked and updates are disabled:

<figure><img src="../../.gitbook/assets/image (15) (1) (1) (1).png" alt=""><figcaption><p>Row locked for editing</p></figcaption></figure>

### iv) Lock multiple cells

In order to lock multiple cells, ctrl + click the required cells. Click on the lock icon and select Lock selected cells from the drop-down.

<figure><img src="../../.gitbook/assets/image (5) (3).png" alt=""><figcaption><p>Lock Selected Cells</p></figcaption></figure>



The cells that are locked are highlighted:

<figure><img src="../../.gitbook/assets/image (8) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Locked Cells Highlighted</p></figcaption></figure>

### v) Unlock

a) To unlock a locked cell, select 'Unlock this cell' from the context menu.

<figure><img src="../../.gitbook/assets/7.2.19 Unlock cell.png" alt=""><figcaption><p>Unlock cell</p></figcaption></figure>

b) The selected cell gets unlocked.

<figure><img src="../../.gitbook/assets/7.2.20 Unlock cell.png" alt=""><figcaption><p>Cell unlocked</p></figcaption></figure>

c) All children of a locked cell can be unlocked by selecting the 'Unlock all children' option from the context menu.

<figure><img src="../../.gitbook/assets/7.2.21 Unlock children.png" alt=""><figcaption><p>Unlock all children </p></figcaption></figure>

d) All the cells including the quarters are unlocked.

<figure><img src="../../.gitbook/assets/7.2.22 Unlock children.png" alt=""><figcaption><p>All children unlocked</p></figcaption></figure>

e) To unlock a row when measure in rows in enabled, click on the row gripper and select Unlock Row.

<figure><img src="../../.gitbook/assets/image (10) (1) (1) (1) (1).png" alt=""><figcaption><p>Unlock Row</p></figcaption></figure>

f) To unlock multiple cells, ctrl + click the cells and click on Unlock selected cells.

<figure><img src="../../.gitbook/assets/image (2) (3).png" alt=""><figcaption><p>Unlock selected cells</p></figcaption></figure>

## 4. Edit period values

On clicking a child cell, you can see that there is different context menu. There are two preset options to update cell values. You can copy the same cell value across rows or columns or apply a trend.

If these options do not satisfy your requirements, you can customize your cells manually.

<figure><img src="../../.gitbook/assets/7.2.23 Trend.png" alt=""><figcaption><p>Options to edit period values</p></figcaption></figure>

### i) Copy

You can copy the current cell value and apply it to other cells using the following options:

* Copy until the last row in the row category
* Copy to all rows in the row category
* Copy to all rows
* Copy until the last column in the column category
* Copy to all columns in the column category

{% hint style="info" %}
Note that the options shown in the below image are enabled only when there are two or more categories in the rows and columns.
{% endhint %}

<figure><img src="../../.gitbook/assets/7.2.35 Copy all category.png" alt=""><figcaption><p>Copy options</p></figcaption></figure>

Let's take a simpler example - with two categories (Product category and subcategory) in the rows and Quarters in the column.

a) On selecting 'Copy to all rows', the value for Soda is copied to all other subcategories.

<figure><img src="../../.gitbook/assets/7.2.32 Copy all.png" alt=""><figcaption><p>Copy to all rows</p></figcaption></figure>

b) If you only want to copy a particular value within the category, you can select the option highlighted below.

<figure><img src="../../.gitbook/assets/7.2.34 Copy all category.png" alt=""><figcaption><p>Copy to all rows in the category</p></figcaption></figure>

c) Value can be copied until the last column using the highlighted option.

<figure><img src="../../.gitbook/assets/7.2.33 Copy last column.png" alt=""><figcaption><p>Copy until the last column</p></figcaption></figure>



### ii) Trend

You can apply a trend based on the current cell value and apply it until the last row or column.&#x20;

a) As you click on the '>', you can see a graphical slider where you can set a trend.

<figure><img src="../../.gitbook/assets/7.2.24 Trend.png" alt=""><figcaption><p>Graphical slider</p></figcaption></figure>

b) If you want to enter a percentage precisely, you can click on the 'Input custom value' option.

<figure><img src="../../.gitbook/assets/7.2.26 Trend.png" alt=""><figcaption><p>Input custom value</p></figcaption></figure>

c) Enter a percentage and click 'Apply'.&#x20;

<figure><img src="../../.gitbook/assets/7.2.28 Trend.png" alt=""><figcaption><p>Custom value</p></figcaption></figure>

d) The values for Soda and Tea & Coffee are updated as shown in the below image.

<figure><img src="../../.gitbook/assets/7.2.29 Trend.png" alt=""><figcaption><p>Copy until last row with trend</p></figcaption></figure>

e) You can use 'Copy with trend' in combination with 'Lock this cell' to achieve different business cases. Let's consider an example where the value for Q3 is fixed and the trend needs to be applied to the other quarters. Click on the 'Lock this cell' for the cell highlighted.

<figure><img src="../../.gitbook/assets/7.2.30 Trend.png" alt=""><figcaption><p>Lock cells and copy to other columns</p></figcaption></figure>

f) On applying a trend of 20% as shown in the image, Q2 and Q4 values are updated. Q3 is greyed out as it is locked.

<figure><img src="../../.gitbook/assets/7.2.31 Trend.png" alt=""><figcaption><p>Trend applied to unlocked cells</p></figcaption></figure>

In the next section, we'll be covering [set version](set-version.md).

#### Resources

[Forecasting Multiple Items with Seasonality in Power BI](https://inforiver.com/blog/general/forecast-multiple-items-with-seasonality-power-bi/)

[5 ways to enhance your budgeting & forecasting process for better data-driven decisions](https://inforiver.com/insights/enhance-budgeting-forecasting-process-for-data-driven-decisions/)
