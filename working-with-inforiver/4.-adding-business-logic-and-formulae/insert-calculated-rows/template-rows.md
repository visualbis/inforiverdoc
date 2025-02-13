# Template rows

Inforiver allows inserting calculated rows at every level in the hierarchy with the template row option.

{% embed url="https://lumel.wistia.com/medias/n67puv7p0m" %}

Let us take this example: Sales data by region and category. Let's insert a calculated row in each hierarchy which is 1.5 times the value of Beverages across quarters.

**STEP 1:** Click on the row above which to insert a template row. Create a calculated row by choosing the **Formula** option from the Insert Row menu.

<figure><img src="../../../.gitbook/assets/image (1216).png" alt=""><figcaption></figcaption></figure>

**STEP 2:** Select the Templated option. Enter the title and the desired formula in the editor. When you click Create, the row gets created across all levels of the hierarchy.

<figure><img src="../../../.gitbook/assets/image (1218).png" alt=""><figcaption><p>Creating a calculated template row</p></figcaption></figure>

**STEP 3:**  Set the row position to ‘First’, ‘Auto’, or ‘Last’ from the drop-down.

* First - the template row will be placed first at the category level, irrespective of where it is added
* Auto - the template row is placed above the selected row where it is added
* Last - the template row is placed last at the category level, irrespective of where it is added

<figure><img src="../../../.gitbook/assets/image (1219).png" alt=""><figcaption><p>Row position</p></figcaption></figure>

**STEP 4:** To include the row value in subtotals and totals, check the 'Include in total' check box.

<figure><img src="../../../.gitbook/assets/image (1220).png" alt=""><figcaption><p>include in total</p></figcaption></figure>

**STEP 5:** If charts are added to the table, the 'Include in charts' option allows you to visualize the calculated rows as well using charts.

{% hint style="info" %}
The 'Include in charts' checkbox is enabled only when the 'Include in total' option is unchecked.
{% endhint %}

**STEP 6:** You can add a description for the formula if needed.&#x20;

The below image shows another example, where the rows 'Medium-Large' are defined as the previous month's value for the size 'Medium'. To learn more about the formula used, refer to [RELATIVE\_COLUMN](../../../formula-syntax/identifiers/relative_column.md).

<figure><img src="../../../.gitbook/assets/image (1221).png" alt=""><figcaption><p>Template row</p></figcaption></figure>

Edit/delete the inserted template row by clicking on the row gripper of the selected template row and choosing the respective option from the drop-down.

<figure><img src="../../../.gitbook/assets/image (1222).png" alt=""><figcaption><p>Edit or delete template rows</p></figcaption></figure>
