# Number

Numeric data can be entered and formatted in a variety of ways. You can either insert a blank column and start entering data or use an existing column as a base to make further updates.

Let's first look at the steps to insert a blank numeric data input column. The steps to copy another column as a data input column are covered in '[Copy as data input](insert-manual-input-columns.md#4.-copy-as-data-input)'.

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

### ii) Distribute parent value to children

When a value is entered in a subtotal or total row, the value can be distributed to the child rows.&#x20;

In the below image, 220m entered in the subtotal has been distributed equally to the subregions.

<figure><img src="../../../.gitbook/assets/4.4.1. Distribute value.png" alt=""><figcaption><p>Value in subtotal distributed to child rows</p></figcaption></figure>

There are several other ways to distribute values which will be covered in [Budgeting & allocations](../../7.-planning-budgeting-and-forecasting/budgeting-and-allocations.md).&#x20;

This distribution can be disabled if not required for certain scenarios. Uncheck the 'Distribute parent value to children' checkbox.

<figure><img src="../../../.gitbook/assets/4.4.21 number.png" alt=""><figcaption><p>Disabling distribution</p></figcaption></figure>

### iii) Min and max range

When you need to define a range for the data input values, you can use the fields highlighted in the below image. Note that these are enabled only when the 'Distribute parent value to children' checkbox is unchecked.

<figure><img src="../../../.gitbook/assets/4.4.22 number.png" alt=""><figcaption><p>Defining minimum and maximum value range</p></figcaption></figure>

In the dropdown, you can see that there are two ways of defining ranges. Click on 'Static'.&#x20;

<figure><img src="../../../.gitbook/assets/4.4.23 number.png" alt=""><figcaption><p>Static values or measures</p></figcaption></figure>

The input field gets enabled. Enter a value as shown.

<figure><img src="../../../.gitbook/assets/4.4.24 number.png" alt=""><figcaption><p>Entering a value</p></figcaption></figure>

Let's define a maximum value using a measure. Select 'Measure' and '2022 Actuals' from the dropdown list. Click 'Update'.&#x20;

<figure><img src="../../../.gitbook/assets/4.4.25 number.png" alt=""><figcaption><p>Using a measure as the maximum value range</p></figcaption></figure>

Enter a value that is not within the defined range. Double-click on a cell and type in the formula bar. Click 'Enter'.&#x20;

<figure><img src="../../../.gitbook/assets/4.4.26 number.png" alt=""><figcaption><p>Entering a value out of the defined range</p></figcaption></figure>

You can see an error message that shows the allowed range for this particular cell. The maximum is 82m as that is the value of 2022 Actuals. &#x20;

<figure><img src="../../../.gitbook/assets/4.4.27 number.png" alt=""><figcaption><p>Error message</p></figcaption></figure>

Values within the defined range are captured as shown in the below image.

<figure><img src="../../../.gitbook/assets/4.4.28 number.png" alt=""><figcaption><p>Value within range captured</p></figcaption></figure>

## 4. Copy as data input

There might be cases where you want to create a budget for the current year based on the prior year's budget and then make finer adjustments. In such cases, Inforiver provides the 'Copy as data input' option.

Click on the column gripper corresponding to the measure you want to use as the base. Select 'Copy as data input' from the 'Insert' option. &#x20;

<figure><img src="../../../.gitbook/assets/4.4.29 Number.png" alt=""><figcaption><p>Copy as data input</p></figcaption></figure>

A measure gets created with the same values. You can rename it and customize other properties such as row aggregation type or allow input using the side panel.

<figure><img src="../../../.gitbook/assets/4.4.30 Number.png" alt=""><figcaption><p>Data input column created</p></figcaption></figure>

To edit values, double-click on a cell and enter as shown in the formula bar.

<figure><img src="../../../.gitbook/assets/4.4.31 Number.png" alt=""><figcaption><p>Updating values</p></figcaption></figure>

The values get updated and are also distributed or rolled up to the child and parent cells respectively.

<figure><img src="../../../.gitbook/assets/4.4.32 Number.png" alt=""><figcaption><p>Value gets updated</p></figcaption></figure>

In the next section, we'll be looking at [dropdown input columns](dropdown.md).
