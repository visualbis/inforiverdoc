# Editing cells

Inforiver allows you to edit the contents of a cell and apply calculations. These are visual level updates and will not impact the source dataset.

### 1. Overwriting value

To overwrite an existing value, simply double-click on the cell and enter the new value. You can enter scaled values(250m, 5.6b, etc) or reference other cell values.

Double-click on a cell as shown in the image. A formula bar is enabled below the toolbar. Type in a value and click 'Enter'. Note that Inforiver allows entry of scaled values (e.g. 45.3m instead of 45,300,000).

<figure><img src="../../.gitbook/assets/image (321).png" alt=""><figcaption><p>Overwriting a value</p></figcaption></figure>

The value gets updated and the manual update can be identified by the pencil icon in the cell. The totals and subtotals are also updated to include the value entered.&#x20;

<figure><img src="../../.gitbook/assets/image (322).png" alt=""><figcaption><p>Updated value</p></figcaption></figure>

You can even reference other cells and apply formulas to them - using the cell editor, you can define simple mathematical operations such as A +/- B, etc.

<figure><img src="../../.gitbook/assets/image (320).png" alt=""><figcaption><p>Using cell references and applying formulas</p></figcaption></figure>

{% hint style="info" %}
* You can also edit cells using the 'Edit cell' icon in the toolbar. You can access it in the Insert tab > Cell section.&#x20;
* Inforiver allows you to edit values AC, PY, PL, FC, and OM measures. You can edit dates and text measures as well.
{% endhint %}

### 2. Apply formulas

&#x20; You can use the wide range of formulas and functions available in Inforiver while editing a cell. In the below example, we are using the 'Average' function. As you start typing, you can see the functions that match the entered text as a list. Click on 'Average'.

<figure><img src="../../.gitbook/assets/4.3.9 Static rows.png" alt=""><figcaption><p>Using formulas in static rows</p></figcaption></figure>

a) Click on the arrow icon, to see more information such as the arguments and examples.

<figure><img src="../../.gitbook/assets/4.3.10 Static rows.png" alt=""><figcaption><p>Formula syntax</p></figcaption></figure>

b) You can click on any cell and it gets automatically populated as shown below. You can also see the result of the operation as highlighted.

<figure><img src="../../.gitbook/assets/4.3.11 Static rows.png" alt=""><figcaption><p>Selecting a cell</p></figcaption></figure>

c) Let's calculate the average of the two selected cells.

<figure><img src="../../.gitbook/assets/4.3.12 Static rows.png" alt=""><figcaption><p>Result of the operation</p></figcaption></figure>

d) You can see the result of the operation and it also gets distributed to the child levels.&#x20;

<figure><img src="../../.gitbook/assets/4.3.13 Static rows.png" alt=""><figcaption><p>Data captured</p></figcaption></figure>

### 3. Updating multiple cells

You can also override the data in multiple cells with the same value, for instance, set a fixed budget. Select the cells and update the value in any cell, the updated value will get cascaded to all the selected cells.

<figure><img src="../../.gitbook/assets/image (310).png" alt=""><figcaption></figcaption></figure>

### 4. Renaming Row Categories

You can also rename row categories by double-clicking on them.&#x20;

The same row category may be repeated at each hierarchy level for hierarchical datasets. When you try to rename such categories at one level, Inforiver displays a prompt to confirm whether the category should be renamed across all levels or only at that level.

<figure><img src="../../.gitbook/assets/image (8) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Renaming Row Categories</p></figcaption></figure>

### 5. Bulk edit

In financial reporting, costs or revenues may need to be allocated across multiple fields, or during the budgeting/forecasting process, the same values may need to be distributed across different fields. In some cases, you may need to set the same date, such as the expiry date for a list of products, or assign the same manager to a group of locations.

Let's look at the **Bulk Edit** feature that comes in handy in such situations. We will use an example where we need to bulk edit a data input-number column.

Navigate to the Insert ribbon and click the Bulk Edit option from the Cell section.

<figure><img src="../../.gitbook/assets/image (1) (14).png" alt=""><figcaption><p>Bulk edit interface</p></figcaption></figure>

**STEP 1:** From the **Measure** dropdow&#x6E;**,** select the data input measure for which you want to perform a bulk update.

<figure><img src="../../.gitbook/assets/image (2) (13).png" alt=""><figcaption><p>Select measure</p></figcaption></figure>

**STEP 2:** Use the dimension category dropdowns to select the categories for which you need to update values. You can select multiple categories for each dimension. As you make selections, you'll notice the report getting filtered dynamically.

<figure><img src="../../.gitbook/assets/Untitled Project (1).gif" alt=""><figcaption><p>Choosing dimensions and measures</p></figcaption></figure>

**STEP 3:** Select the row hierarchy level at which the value should be updated.&#x20;

<figure><img src="../../.gitbook/assets/image (7) (12).png" alt=""><figcaption><p>Selecting the row hierarchy category</p></figcaption></figure>

**STEP 4:** Similarl&#x79;**,** select the column hierarchy level at which the value should be updated. In this case, since we do not have a column-level hierarchy, we can either update at Grand Total level or Country level.

<figure><img src="../../.gitbook/assets/image (8) (10).png" alt=""><figcaption><p>Selecting the column hierarchy category</p></figcaption></figure>

**STEP 5:** Choose the type of update to perform and enter the value. If you choose **Append**, the value will be added to the existing value. If you choose **Set Value,** the existing value will be replaced by the new value. To remove the existing value, choose **Clear Set Value.**

<figure><img src="../../.gitbook/assets/image (9) (8).png" alt=""><figcaption><p>Type of update</p></figcaption></figure>

**STEP 6:** You can choose to distribute the updated value to child rows based on the weights of another measure or distribute equally.

<figure><img src="../../.gitbook/assets/image (10) (7).png" alt=""><figcaption><p>Distribute values</p></figcaption></figure>

The cells are updated to 50k at the Segment level and distributed to the children based on the weights of the Sales measure.

<figure><img src="../../.gitbook/assets/image (11) (8).png" alt=""><figcaption><p>Edited cells highlighted in yellow. Distribution measure highlighted in violet.</p></figcaption></figure>

Similarly, we can bulk edit all other data input types, including text, date, person, single-select, and multi-select dropdowns. In the image below, the bulk edit feature has been used to set values for items in the selected categories, sub-categories, and dimensions.

<figure><img src="../../.gitbook/assets/bulk edit all data input.png" alt=""><figcaption><p>Bulk edit feature</p></figcaption></figure>

Specifically for date fields, you can either set a date from the date picker or add a duration in years, quarters, months, weeks, or days to the existing date.

<figure><img src="../../.gitbook/assets/bulk edit add duration.gif" alt=""><figcaption><p>Adding specific duration to list of items</p></figcaption></figure>

{% hint style="info" %}
When editing data in bulk:

1. If you are working with numerical data inputs, you can append and distribute values.
2. For date input type, you can specify the duration or choose a date.
3. When column headers have a hierarchy, like a region or date hierarchy, you can collectively apply changes to specific column levels.
{% endhint %}

{% hint style="info" %}
Bulk editing is available for simulation measures and scenarios so that simulations can be applied to specific categories and dimensions in one go. Refer these sections to learn more: [Bulk editing a simulation measure](what-if-analysis-and-simulations.md#id-3.-bulk-editing-a-simulation-measure) and [Bulk editing a scenario](../7.-planning-budgeting-and-forecasting/scenarios-enterprise-only.md#iv-bulk-editing-a-scenario).
{% endhint %}
