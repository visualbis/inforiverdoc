# Number

Numeric data can be entered and formatted in a variety of ways. Let's look at the steps to insert a numeric data input column.&#x20;

## 1. Create a column

Select the 'Number' option in the dropdown.

<figure><img src="../../../.gitbook/assets/4.4.3 Number.png" alt=""><figcaption><p>Inserting a numeric input column/measure</p></figcaption></figure>

By default, a visual measure gets inserted as shown below. There is a side panel which provides a number of customization options.

<figure><img src="../../../.gitbook/assets/4.4.4 Number.png" alt=""><figcaption><p>Data input side panel</p></figcaption></figure>

The available properties are:

* **Insert as**: A [column or measure](../insert-manual-input-columns.md#2.-measure-vs-column) can be inserted. If there is a column hierarchy, the input column is inserted for each category. In case of no column hierarchy, a single column is inserted.
* **Input type**: The type of [data input column](../insert-manual-input-columns.md); can be changed from the initial selection before creating the column by clicking on 'Create'.&#x20;
* **Row aggregation type**: By default, totals and subtotals are defined as the sum of child rows. There are a number of other options such as average, minimum, maximum etc.&#x20;
* **Distribute parent value to children**: The values entered at a parent level are distributed to the child rows when enabled. This is very useful when creating budgets or forecasts.&#x20;
* **Allow input**: By default, inputs are enabled in both read and edit modes. But, based on your requirement, you can [allow inputs](../insert-manual-input-columns.md#3.-input-restrictions) only in edit mode or based on a formula.&#x20;
* **Description**: Option to add a note for reference

Change the title and go with the default for the other properties. Click 'Create'.

<figure><img src="../../../.gitbook/assets/4.4.6 Number.png" alt=""><figcaption><p>Inserting a numeric measure</p></figcaption></figure>

The measure gets inserted and the column grand total also gets enabled.

<figure><img src="../../../.gitbook/assets/4.4.7 Number.png" alt=""><figcaption><p>Numeric measure inserted</p></figcaption></figure>

## 2. Enter a value

To enter a value, double-click a cell and type in the formula bar that opens on the top.&#x20;

<figure><img src="../../../.gitbook/assets/4.4.8 Number.png" alt=""><figcaption><p>Entering a value</p></figcaption></figure>

The entered value is captured and is also automatically rolled up to the parent.

<figure><img src="../../../.gitbook/assets/4.4.9 Number.png" alt=""><figcaption><p>Value gets rolled up to the top</p></figcaption></figure>

## 3. Properties

To open the data input side panel, click on 'Manage' and the 'Pencil' icon as highlighted.

<figure><img src="../../../.gitbook/assets/4.4.18 number.png" alt=""><figcaption><p>Manage inserted data input column</p></figcaption></figure>

The side panel opens. The input type is greyed out. This is because once a data input column is created, the type of column cannot be changed.

### i) Row aggregation type&#x20;

Row aggregation type defines the aggregation method to be followed for the total and sub-total rows. By default, the subtotal and total rows are calculated as the sum of the child rows, as can be seen in the below image.

Click on the 'Row aggregation type' dropdown. The types of row aggregations are shown below. Click on the desired type and click 'Update'.

<figure><img src="../../../.gitbook/assets/4.4.19 number.png" alt=""><figcaption><p>Available row aggregation types</p></figcaption></figure>

In the below image, 'Maximum' has been chosen. The highlighted cells, which are the row subtotals, get updated.

<figure><img src="../../../.gitbook/assets/4.4.20 number.png" alt=""><figcaption><p>Aggregation type - Maximum</p></figcaption></figure>

### ii) Distribute parent value

When a value is entered in a subtotal or total row, the value can be distributed to the child rows. This distribution can be disabled if not required for certain scenarios.





