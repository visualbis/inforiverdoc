# Template rows

Inforiver allows inserting calculated rows at every level in the hierarchy with the template row option.

{% embed url="https://lumel.wistia.com/medias/n67puv7p0m" %}

Let us take this example: Sales data by region and category. Let's insert a calculated row in each hierarchy which is 1.5 times the value of Beverages across quarters.

a) Select a row above which you would like to insert the row.

b) In the 'Insert' tab of the toolbar, click on the ‘Insert row' dropdown and select the 'Template row' option.

<figure><img src="../../../.gitbook/assets/Insert.png" alt=""><figcaption><p>Insert template row</p></figcaption></figure>

c) A new row gets inserted and the 'Template row' side panel opens.

<figure><img src="../../../.gitbook/assets/Template row panel.png" alt=""><figcaption><p>Template row side panel</p></figcaption></figure>

d) Enter the 'title' and insert the required 'formula'. Refer to [calculated rows](./) for more details on using the formula editor.

<figure><img src="../../../.gitbook/assets/Tiltle.png" alt=""><figcaption><p>Title &#x26; formula</p></figcaption></figure>

e) Select the 'Row position' as ‘First’, ‘Auto’ or ‘Last’ from the drop-down.

'First' - the template row will be placed first at the category level, irrespective of where it is added

'Auto' - the template row is placed above the selected row where it is added

'Last' - the template row is placed last at the category level, irrespective of where it is added

<figure><img src="../../../.gitbook/assets/Row pos.png" alt=""><figcaption><p>Row position</p></figcaption></figure>

f) You can select the 'Apply the same style to all rows' checkbox if you want to replicate the same formatting to all of the rows. For example, let's apply a background color for the row.

<figure><img src="../../../.gitbook/assets/Format.png" alt=""><figcaption><p>Format style applied</p></figcaption></figure>

g) To include the row value in subtotals and totals, check the 'Include in total' check box.

<figure><img src="../../../.gitbook/assets/Include total.png" alt=""><figcaption><p>Include total</p></figcaption></figure>

h) If charts are added to the table, the 'Include in charts' option allows you to visualize the calculated rows as well using charts.

{% hint style="info" %}
The 'Include in charts' checkbox is enabled only when the 'Include in total' option is unchecked.
{% endhint %}

i) If the 'Evaluate columns before rows' checkbox is enabled, the defined formula is used for calculating the column totals. If this check box is disabled, then sum aggregation is followed fo the column totals. To learn more, refer [Evaluate columns before rows](https://inforiver.gitbook.io/inforiver/working-with-inforiver/4.-adding-business-logic-and-formulae/insert-calculated-rows#4.-evaluate-column-before-rows).

j) You can add a description for the formula if needed. Click 'Create'.

<figure><img src="../../../.gitbook/assets/Formula des.png" alt=""><figcaption><p>Create template row</p></figcaption></figure>

k) The row gets created at the category level for all the subregions as shown.

<figure><img src="../../../.gitbook/assets/Template row.png" alt=""><figcaption><p>Template rows</p></figcaption></figure>

l) The below image shows another example, where the rows 'Extra Large' are defined as the previous month's value for the size 'Large'. To learn more about the formula used, refer to [RELATIVE\_COLUMN](../../../formula-syntax/identifiers/relative\_column.md).

<figure><img src="../../../.gitbook/assets/MicrosoftTeams-image (9).png" alt=""><figcaption><p>Template rows</p></figcaption></figure>

m) You can edit/delete the inserted template row by clicking on the row gripper of the selected template row and choosing the respective option from the drop-down.

<figure><img src="../../../.gitbook/assets/Edit.png" alt=""><figcaption><p>Edit &#x26; delete template row</p></figcaption></figure>
