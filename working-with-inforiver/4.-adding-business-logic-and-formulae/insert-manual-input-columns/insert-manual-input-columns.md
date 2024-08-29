# Number

Numeric data can be entered and formatted in a variety of ways. You can insert a new empty series, copy from another series, perform an advanced copy\*, or import from a file.

_\*The Advanced Copy feature will be available soon._&#x20;

Let's first look at the steps to insert a numeric data input column. The steps to copy another column as a data input column are covered in '[Copy as data input](insert-manual-input-columns.md#id-4.-copy-as-data-input)'.

{% hint style="info" %}
If you are using Inforiver Enterprise, you need to [sign in](../insert-manual-input-columns.md#1.-sign-in) to start inserting a number column.&#x20;
{% endhint %}

## 1. Create a column

Select the 'Number' option in the Data Input dropdown. You will see four different options to create a column:  Insert a new empty series, Copy from another series, Advanced copy, and Import from file. Let's go through each of these methods.

{% hint style="info" %}
Inforiver Enterprise edition has been used below to demonstrate the four ways of creating a data input column.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (594).png" alt=""><figcaption><p>Insert number options</p></figcaption></figure>

### i) Insert a new empty series

If you select this option, a visual measure gets inserted as shown below. There is a side panel that provides several customization options.

<figure><img src="../../../.gitbook/assets/image (611).png" alt=""><figcaption><p>Data input side panel</p></figcaption></figure>

#### The available properties are:

* **Insert as**: A [column or measure](../insert-manual-input-columns.md#a-insert-as) can be inserted. If there is a column hierarchy, the input column is inserted for each category. In case of no column hierarchy, a single column is inserted.
* **Input type**: The type of [data input column](../insert-manual-input-columns.md); can be changed from the initial selection before creating the column by clicking on 'Create'.&#x20;
* **Row aggregation type**: By default, totals, and subtotals are defined as the sum of child rows as shown [here](insert-manual-input-columns.md#i-row-aggregation-type). There are several other options such as average, minimum, maximum, etc. that are explained in detail [here](../../manage-aggregations/).
* **Distribute parent value to children**: The values entered at a parent level are distributed to the child rows [when enabled](insert-manual-input-columns.md#ii-distribute-parent-value-to-children). This is very useful when creating budgets or forecasts.&#x20;
* **Minimum Value**: You can optionally [specify the minimum threshold value](insert-manual-input-columns.md#iii-min-and-max-range) for the leaf-level cells, which can be a static number or value from the selected measure. When set, Inforiver ensures that both user input and the allocations to these cells are always more than this value.
* **Maximum Value**: You can optionally [specify the maximum threshold value](insert-manual-input-columns.md#iii-min-and-max-range) for the leaf-level cells, which can be a static number or value from the selected measure. When set, Inforiver ensures that both user input and the allocations to these cells are always less than this value.
* **Default Value**: In cells where the user has not entered any value, instead of displaying empty cells you can choose to display a default value. The default value can be selected from any native or formula measure as explained [here](insert-manual-input-columns.md#iv-default-value). If the underlying native or formula measure is updated, the default value will reflect the latest value.
* **Allow input**: By default, inputs are enabled in both read and edit modes. But, based on your requirement, you can [allow inputs](../insert-manual-input-columns.md#b-allow-input) only in edit mode or based on a formula.&#x20;
* **Description**: Option to add a note for reference.

Change the title and go with the default for the other properties. Click 'Create'.

<figure><img src="../../../.gitbook/assets/image (617).png" alt=""><figcaption><p>Inserting a numeric measure</p></figcaption></figure>

The measure gets inserted.

<figure><img src="../../../.gitbook/assets/image (618).png" alt=""><figcaption><p>Numeric measure inserted</p></figcaption></figure>

To learn to enter a value in an empty numeric column in the [Enter a value](insert-manual-input-columns.md#id-2.-enter-a-value) section.

### ii) Copy from another series

If you select this option, you will see a sub-option with all the measures/forecasts present in the report. You can select any series to create a numeric column with all the data copied from the chosen series. The values from the measure chosen as the source will serve as initial values only. If there are changes to the source measure, these changes will not be reflected in the data input field.

<figure><img src="../../../.gitbook/assets/image (619).png" alt=""><figcaption><p>Copy from another series</p></figcaption></figure>

A visual measure gets inserted as shown below. There is a side panel that provides several customization options. Change the title and go with the default for the other properties. Click 'Create'.

<figure><img src="../../../.gitbook/assets/image (620).png" alt=""><figcaption><p>Change the title and click 'Create'</p></figcaption></figure>

The newly created numeric measure will be pre-populated with the data of the chosen series.

In the below image, a numeric measure is created by copying the data from '2022 Actuals' and the created column is pre-populated with the copied data.

<figure><img src="../../../.gitbook/assets/image (621).png" alt=""><figcaption><p>Numeric measure created</p></figcaption></figure>

### iii) Advanced Copy\*

_\*This option will be available soon_

When you select this option, a pop-up window opens where you can create measures for multiple time frames and populate them with various series and configurations.

You can also choose this option to fill in the blank forecast measures if you have already [inserted them](../../7.-planning-budgeting-and-forecasting/forecasting.md#id-1.-generating-a-forecast) in your report.

<figure><img src="../../../.gitbook/assets/image (623).png" alt=""><figcaption><p>Advanced copy</p></figcaption></figure>

The image below demonstrates the possible configurations (copy methods) you can set for each time frame of the measure. Let us look at the options available in detail.

<figure><img src="../../../.gitbook/assets/image (609).png" alt=""><figcaption><p>Different Copy Methods</p></figcaption></figure>

**Column:** Define the end period for the column here. You will be provided with the **+Add new** option beside the Column Selection if the end period chosen is not the last one in the report. You can create multiple columns by selecting different end periods for each column.&#x20;

**Source Series:** This dropdown lists the available native /data input /forecast series from which you can choose the required one to be copied. Choose 'Blank' to leave the measures empty.

**Copy Method:** Here you can select the copy method based on which the column is populated.

* Period Range: Copies the data from a range of periods to the column, period-wise.
* Single Period: A single period's data is copied to all the periods of the column.
* Average of Period Range: The average of the data range is calculated and spread to the column periods.

**Column Selection:** This option lets you select a single period or a range of periods from the source series, based on the copy method chosen.

After setting up all the details, click **Create.** The image below is a screengrab of the result of the above configuration.

<figure><img src="../../../.gitbook/assets/image (603).png" alt=""><figcaption><p>Advanced Copy - example</p></figcaption></figure>

### iv) Import from file

You can also upload the data for the input columns by importing it through a .csv file. Choose **Import from file.**

<figure><img src="../../../.gitbook/assets/image (604).png" alt=""><figcaption><p>Import from file</p></figcaption></figure>

Download the template, save it, and enter your data in the file.

<figure><img src="../../../.gitbook/assets/image (605).png" alt=""><figcaption><p>Download the template</p></figcaption></figure>

After entering and saving the data, click **Browse** and select the saved file.&#x20;

<figure><img src="../../../.gitbook/assets/image (607).png" alt=""><figcaption><p>Select the saved file</p></figcaption></figure>

Click **Preview.**

<figure><img src="../../../.gitbook/assets/image (606).png" alt=""><figcaption><p>Click 'Preview'</p></figcaption></figure>

The measures are inserted as shown below. You can make any changes if necessary and then click **Create.**

<figure><img src="../../../.gitbook/assets/image (608).png" alt=""><figcaption><p>Measures inserted</p></figcaption></figure>

## 2. Enter a value

To enter a value, double-click a cell and type in the formula bar that opens on the top.&#x20;

<figure><img src="../../../.gitbook/assets/image (596).png" alt=""><figcaption><p>Entering a value</p></figcaption></figure>

You can also enter values directly on the cell as shown below.

<figure><img src="../../../.gitbook/assets/image (597).png" alt=""><figcaption></figcaption></figure>

The entered value is captured and it is also automatically rolled up to the parent as well as distributed to the child nodes if applicable.

<figure><img src="../../../.gitbook/assets/image (598).png" alt=""><figcaption><p>Value gets rolled up to the top and also distributed to the child levels</p></figcaption></figure>

## 3. Properties

You can modify the properties of a previously created data input column in the side panel. To open it, click on **Manage Measures** and the 'Pencil' icon as highlighted.

<figure><img src="../../../.gitbook/assets/image (599).png" alt=""><figcaption><p>Manage inserted data input column</p></figcaption></figure>

The side panel opens. The input type is greyed out. This is because once a data input column is created, you cannot change its type. You can make any necessary changes and click **Update**.

<figure><img src="../../../.gitbook/assets/image (600).png" alt=""><figcaption><p>Editing the properties of inserted Data Input column</p></figcaption></figure>

We have already discussed an overview of the properties [here](insert-manual-input-columns.md#the-available-properties-are). Here we will discuss a few properties in detail.

### i) Row aggregation type&#x20;

Row aggregation type defines the aggregation method to be applied for the total and sub-total rows. By default, the subtotal and total rows are calculated as the sum of the child rows, as can be seen in the below image.

<figure><img src="../../../.gitbook/assets/image (601).png" alt=""><figcaption><p>Default row aggregation is 'Sum'</p></figcaption></figure>

To change the aggregation method, click the **Row aggregation type** dropdown in the side panel. Choose one from the types available and click **Update**.&#x20;

<figure><img src="../../../.gitbook/assets/image (602).png" alt=""><figcaption><p>Available row aggregation types</p></figcaption></figure>

{% hint style="info" %}
To understand the different aggregations, you can refer to [this section.](../../manage-aggregations/)
{% endhint %}

In the below image, 'Maximum' has been chosen. The highlighted cells, which are the row subtotals, get updated.

<figure><img src="../../../.gitbook/assets/4.4.20 number.png" alt=""><figcaption><p>Aggregation type - Maximum</p></figcaption></figure>

### ii) Distribute parent value to children

When a value is entered in a subtotal or total row, the value can be distributed to the child rows.&#x20;

In the below image, 220m entered in the subtotal has been distributed equally to the subregions.

<figure><img src="../../../.gitbook/assets/4.4.1. Distribute value.png" alt=""><figcaption><p>Value in subtotal distributed to child rows</p></figcaption></figure>

There are several other ways to distribute values which are covered in [Budgeting & allocations](../budgeting-and-allocations.md).&#x20;

{% hint style="info" %}
**Sum** and **Weighted Average** are the only row aggregation methods that allow allocations/distributions from total cells to child rows.
{% endhint %}

This distribution can be disabled if not required for certain scenarios. Uncheck the 'Distribute parent value to children' checkbox.

<figure><img src="../../../.gitbook/assets/4.4.21 number.png" alt=""><figcaption><p>Disabling distribution</p></figcaption></figure>

### iii) Min and max range

When you need to define a range for the data input values, you can use the fields highlighted in the below image.&#x20;

<figure><img src="../../../.gitbook/assets/image (612).png" alt=""><figcaption><p>Defining minimum and maximum value range</p></figcaption></figure>

In the dropdown, you can see the two ways of defining ranges. Click on 'Static'.&#x20;

<figure><img src="../../../.gitbook/assets/image (613).png" alt=""><figcaption><p>Static values or measures</p></figcaption></figure>

The input field gets enabled. Enter a value as shown.

<figure><img src="../../../.gitbook/assets/image (614).png" alt=""><figcaption><p>Entering a value</p></figcaption></figure>

Let's define a maximum value using a measure. Select 'Measure' and '2022 Actuals' from the dropdown list. Click 'Update'.&#x20;

<figure><img src="../../../.gitbook/assets/image (615).png" alt=""><figcaption><p>Using a measure as the maximum value range</p></figcaption></figure>

Enter a value that is not within the defined range. Double-click on a cell and type in the formula bar. Click 'Enter'.&#x20;

<figure><img src="../../../.gitbook/assets/image (616).png" alt=""><figcaption><p>Entering a value out of the defined range</p></figcaption></figure>

You can see an error message that shows the allowed range for this particular cell. The maximum is 82m as that is the value of 2022 Actuals. &#x20;

<figure><img src="../../../.gitbook/assets/4.4.27 number.png" alt=""><figcaption><p>Error message</p></figcaption></figure>

Values within the defined range are captured as shown in the below image.

<figure><img src="../../../.gitbook/assets/4.4.28 number.png" alt=""><figcaption><p>Value within range captured</p></figcaption></figure>

### iv) Default Value

When you create an empty series or column, the user has to enter the values manually. Instead of having those cells blank, you can display a default value. The default value can be selected from any native or formula measure as shown in the image below. If the underlying native or formula measure is updated, the default value will reflect the latest value.

<figure><img src="../../../.gitbook/assets/image (757).png" alt=""><figcaption><p>Default Value</p></figcaption></figure>

#### Visual measures extrapolated for new categories <a href="#visual-measures" id="visual-measures"></a>

When you add new categories to your dataset, Inforiver automatically fills the data in the measure **based on the default value** configured while creating the measure. Let us look at an example where the default value is configured as a dimension from the dataset.

The report below has data for three regions – Central, East and West.&#x20;

<figure><img src="../../../.gitbook/assets/2.5.1. automatic-measure-values-for-new-data-categories.png" alt=""><figcaption><p>Sample report</p></figcaption></figure>

Now when you add data for ‘South’ region, the report automatically fills up the Sales measure based on the default values you have configured (_Sum of Sales_ dimension). You can seamlessly add new categories to your report and Inforiver will take care of populating the data. Note that this is only applicable for visual measures and not the visual columns.

<figure><img src="../../../.gitbook/assets/2.5.2. after-adding-new-measure-values-for-new-data-categories.png" alt=""><figcaption><p>Default values added for newly added categories</p></figcaption></figure>

## 4. Copy as data input

There might be cases where you want to create a budget for the current year based on the prior year's budget and then make finer adjustments. In such cases, Inforiver provides the 'Copy as data input' option.

Click on the column gripper corresponding to the measure you want to use as the base. Select 'Copy as data input' from the 'Insert' option. You need to be mindful that the values from the measure chosen as the source will serve as initial values. If there are changes in the source measure, these changes will not be reflected in the data input field.

<figure><img src="../../../.gitbook/assets/4.4.29 Number.png" alt=""><figcaption><p>Copy as data input</p></figcaption></figure>

A measure gets created with the same values. You can rename it and customize other properties such as row aggregation type or allow input using the side panel.

<figure><img src="../../../.gitbook/assets/4.4.30 Number.png" alt=""><figcaption><p>Data input column created</p></figcaption></figure>

To edit values, double-click on a cell and enter as shown in the formula bar.

<figure><img src="../../../.gitbook/assets/4.4.31 Number.png" alt=""><figcaption><p>Updating values</p></figcaption></figure>

The values get updated and are also distributed or rolled up to the child and parent cells respectively.

<figure><img src="../../../.gitbook/assets/4.4.32 Number.png" alt=""><figcaption><p>Value gets updated</p></figcaption></figure>

In the next section, we'll be looking at [dropdown input columns](dropdown/).
