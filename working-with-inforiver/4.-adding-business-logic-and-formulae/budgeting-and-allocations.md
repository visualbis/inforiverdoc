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

There are two ways to allocate a value entered in a total or subtotal - [equally](budgeting-and-allocations.md#i-equal) or [based on weights](budgeting-and-allocations.md#ii-weight).

### i) Equal

After entering the value in the formula bar, press 'Enter'. By default, the values get distributed equally across all the categories and subcategories. Inforiver automatically highlights the updated values.

Note that the values have been rolled up to the grand total (Grand total -> 2023 Budget).

<figure><img src="../../.gitbook/assets/7.2.3 ZBB.png" alt=""><figcaption><p>Equal distribution</p></figcaption></figure>

Let's consider another example where we enter a budget at the grand total level. Double-click on the highlighted cell and enter 1.2b.

<figure><img src="../../.gitbook/assets/7.2.4 Equal.png" alt=""><figcaption><p>Update grand total value </p></figcaption></figure>

Once you click 'Enter', you can see the value distributed equally across categories, subcategories and quarters.

<figure><img src="../../.gitbook/assets/7.2.5 Equal.png" alt=""><figcaption><p>Equal distribution at grand total level</p></figcaption></figure>

### ii) Weight

In this case, we don't need an equal distribution. We need to allocate the budget proportionally based on 2022 actuals. Click on the context menu appearing on the cell with the value 1,200.0 and choose ‘Distribute by weights of 2022 Actuals’.

<figure><img src="../../.gitbook/assets/7.2.6 Weights.png" alt=""><figcaption><p>Distribution based on prior year values</p></figcaption></figure>

Once this option is selected, the 2023 Budget values are updated automatically across product categories & quarters by their relative contribution to 2022 Actuals.

<figure><img src="../../.gitbook/assets/7.2.7 Weights.png" alt=""><figcaption><p>Value gets redistributed based on weights</p></figcaption></figure>

## 3. Lock values

Values in data input columns can be locked either at a cell level or including all children (at a subtotal/total level). The cells that are locked are not affected by any of the allocation methods.

### i) Lock this cell

Let’s consider a scenario – There is an overall budget for 2023 which is distributed to the categories based on 2022 Actuals. Certain categories and their sub-categories have a fixed budget, and the budget has to be reallocated once these changes are made. Budgets for Juices and Soda are 500m and 350m respectively. &#x20;

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

### iii) Unlock

a) To unlock a locked cell, select 'Unlock this cell' from the context menu.

<figure><img src="../../.gitbook/assets/7.2.19 Unlock cell.png" alt=""><figcaption><p>Unlock cell</p></figcaption></figure>

b) The selected cell gets unlocked.

<figure><img src="../../.gitbook/assets/7.2.20 Unlock cell.png" alt=""><figcaption><p>Cell unlocked</p></figcaption></figure>

c) All children of a locked cell can be unlocked by selecting the 'Unlock all children' option from the context menu.

<figure><img src="../../.gitbook/assets/7.2.21 Unlock children.png" alt=""><figcaption><p>Unlock all children </p></figcaption></figure>

d) All the cells including the quarters are unlocked.

<figure><img src="../../.gitbook/assets/7.2.22 Unlock children.png" alt=""><figcaption><p>All children unlocked</p></figcaption></figure>

## 4. Edit period values



### i) Trend





### ii) Copy





