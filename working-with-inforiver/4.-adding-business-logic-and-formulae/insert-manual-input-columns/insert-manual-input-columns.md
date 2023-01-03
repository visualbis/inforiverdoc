# Number

Let's look at the steps to insert a numeric data input column.

a) Select the 'Number' option in the dropdown.

<figure><img src="../../../.gitbook/assets/4.4.3 Number.png" alt=""><figcaption><p>Inserting a numeric input column/measure</p></figcaption></figure>

b) By default, a visual measure gets inserted as shown below. There is a side panel which provides a number of customization options.

<figure><img src="../../../.gitbook/assets/4.4.4 Number.png" alt=""><figcaption><p>Data input side panel</p></figcaption></figure>

c) The available properties are:

* **Insert as**: A [column or measure](../insert-manual-input-columns.md#2.-measure-vs-column) can be inserted. If there is a column hierarchy, the input column is inserted for each category. In case of no column hierarchy, a single column is inserted.
* **Input type**: The type of data input column; can be changed from the initial selection before creating the column by clicking on 'Create'.&#x20;
* **Row aggregation type**: By default, totals and subtotals are defined as the sum of child rows. There are a number of other options such as average, minimum, maximum etc.&#x20;
* **Distribute parent value to children**: The values entered at a parent level are distributed to the child rows when enabled. This is very useful when creating budgets or forecasts.&#x20;
* **Allow input**: By default, inputs are enabled in both read and edit modes. But, based on your requirement, you can [allow inputs](../insert-manual-input-columns.md#3.-input-restrictions) only in edit mode or based on a formula.&#x20;
* **Description**: Option to add a note for reference

d) Let's just change the title and go with the default for the other properties. Click 'Create'.

<figure><img src="../../../.gitbook/assets/4.4.6 Number.png" alt=""><figcaption><p>Inserting a numeric measure</p></figcaption></figure>

e) The measure gets inserted. You can see that the column grand total also gets enabled.

<figure><img src="../../../.gitbook/assets/4.4.7 Number.png" alt=""><figcaption><p>Numeric measure inserted</p></figcaption></figure>

f) To enter a value, double-click a cell and type in the formula bar that opens on the top.&#x20;

<figure><img src="../../../.gitbook/assets/4.4.8 Number.png" alt=""><figcaption><p>Entering a value</p></figcaption></figure>

g) The entered value is captured and is also automatically rolled up to the parent.

<figure><img src="../../../.gitbook/assets/4.4.9 Number.png" alt=""><figcaption><p>Value gets rolled up to the top</p></figcaption></figure>

h) In the below image, data has been added in a few more cells. Let's now change the aggregation type.

<figure><img src="../../../.gitbook/assets/4.4.10 Number.png" alt=""><figcaption><p>Default aggregation - Sum</p></figcaption></figure>

i) To open the data input side panel, click on 'Manage' and the 'Pencil' icon as highlighted.

<figure><img src="../../../.gitbook/assets/4.4.18 number.png" alt=""><figcaption><p>Manage inserted data input column</p></figcaption></figure>

j) Click on the 'Row aggregation type' dropdown. The available options are shown below.

<figure><img src="../../../.gitbook/assets/4.4.19 number.png" alt=""><figcaption><p>Available row aggregation types</p></figcaption></figure>

k) Select 'Maximum' and click 'Update'. The highlighted cells, which are the row subtotals, get updated.

<figure><img src="../../../.gitbook/assets/4.4.20 number.png" alt=""><figcaption><p>Aggregation type - Maximum</p></figcaption></figure>

