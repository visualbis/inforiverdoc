# Row gripper

In this section, let's explore the various options in Inforiver to customize rows in your reports.&#x20;

#### i) Freeze grand total

If you have set a multi-page layout with scrolling,  use this option to ensure the grand total row is fixed to the top of the page.

<figure><img src="../../../../.gitbook/assets/image (331).png" alt=""><figcaption></figcaption></figure>

#### ii) Expand/Collapse

Inforiver makes it effortless for you to handle large hierarchical datasets. Instead of manually expanding or collapsing each level of the hierarchy, you have various options in the row gripper. [Learn more about managing hierarchies.](../../manage-hierarchies.md)

<figure><img src="../../../../.gitbook/assets/image (39) (2).png" alt=""><figcaption></figcaption></figure>

#### iii) Insert

You can easily insert rows from the row gripper menu. Let's explore the different types of rows that can be inserted using this option.

<figure><img src="../../../../.gitbook/assets/image (3) (7).png" alt=""><figcaption></figcaption></figure>

a) Calculated row

You can create a new row using Inforiver's built-in formulas or write a custom calculation. [Learn more about calculated rows](../../../4.-adding-business-logic-and-formulae/insert-calculated-rows.md).

b) Static row

You can insert a row and manually enter data using the static row option. [Learn more about static rows.](../../../4.-adding-business-logic-and-formulae/insert-manual-input-rows.md)

c) Row hierarchy

Use this option to insert a user-defined level into hierarchical data. [Learn more about row hierarchies](../../../4.-adding-business-logic-and-formulae/insert-manual-input-rows.md#ii-row-hierarchy).

d) Multiple static row

You can insert an entire hierarchy or bulk insert multiple rows using this option. [Learn more about multiple static rows.](../../../4.-adding-business-logic-and-formulae/insert-manual-input-rows.md#i-multiple-static-row)

e) Contribution row

_Contribution rows_ can be used to calculate the contribution of a particular row to its parent. Select a particular row to create a contribution row for it. [Learn more about contribution rows.](../../../4.-adding-business-logic-and-formulae/quick-formula.md#3.-contribution-rows)

f) Template row

Use template rows to insert a calculated row in every level of the hierarchy. Rather than repeatedly creating a calculated row for each level, you can use the _Template row_ option to insert rows in a single shot. [Learn more about template rows.](../../../../advanced-topics/template-rows.md)

g) Empty row

Financial statements and reports often require options to add white spaces for formatting. Inforiver provides the insert 'empty row' option to achieve this in a single click.  [Learn more about empty rows](../../../2.-displaying-information/basic-formatting/insert-blank-rows.md).

#### iv) Aggregation

Inforiver enables you to set custom aggregation to calculate the sub-totals at the parent node level for hierarchical data. This option is available in the row gripper for parent nodes only.

<figure><img src="../../../../.gitbook/assets/image (4) (5).png" alt=""><figcaption></figcaption></figure>

In the report below, the 'Technology' category has an aggregation of **sum**, the 'Furniture' category has an aggregation of **minimum**, and the 'Office Supplies' category has an aggregation of **average**. [Learn more about managing aggregation in Inforiver.](../../../../advanced-topics/manage-aggregations.md)

<figure><img src="../../../../.gitbook/assets/image (5) (7).png" alt=""><figcaption></figcaption></figure>

#### v) Add aggregated row

In addition to the default aggregation at the parent node level, Inforiver allows you to add multiple totals/sub-total rows with different aggregation types. This option is available in the row gripper for parent nodes only.

<figure><img src="../../../../.gitbook/assets/image (6) (8).png" alt=""><figcaption></figcaption></figure>

In the report below, notice how minimum, standard deviation and average rows have been created, in addition to the default total/sub-total aggregation.

<figure><img src="../../../../.gitbook/assets/image (7) (8).png" alt=""><figcaption></figcaption></figure>

#### vi) Actions

The actions section has various formatting and customization options for rows. Let's take a detailed look.

a) Add row break

You can use this option to set pagination based on the category i.e. your report will have one page per category. This option is available in the row gripper for parent nodes only.

<figure><img src="../../../../.gitbook/assets/image (8) (7).png" alt=""><figcaption></figcaption></figure>

We have used the _Add Row Break_ option to create one page corresponding to each category - Technology, Furnishings, and Office Supplies.

<figure><img src="../../../../.gitbook/assets/image (9) (6).png" alt=""><figcaption></figcaption></figure>

b) Hide Icon for level

You can use this option to disable the expand/collapse icon for a particular level of the hierarchy. The hierarchy will always be in an expanded state for that level.

<figure><img src="../../../../.gitbook/assets/image (11) (7).png" alt=""><figcaption></figcaption></figure>

Notice how the expand/collapse icon has been removed for the category level i.e. Furniture, Office Supplies, and Technology.

<figure><img src="../../../../.gitbook/assets/image (12) (3).png" alt=""><figcaption></figcaption></figure>

c) Hide icon and children

This option removes the expand collapse icon and hides all the child rows, retaining only the parent row.

<figure><img src="../../../../.gitbook/assets/image (13) (6).png" alt=""><figcaption></figcaption></figure>

Notice how all the children under the Furniture category have been hidden and the expand/collapse icon has been removed.

<figure><img src="../../../../.gitbook/assets/image (14) (4).png" alt=""><figcaption></figcaption></figure>

d) Hide row

This option can be used to mask rows in the report. Note that hidden rows will still be included in total and sub-total calculations.

<figure><img src="../../../../.gitbook/assets/image (16) (5).png" alt=""><figcaption></figcaption></figure>

The 'Bookcases' row has been masked using this option. Use the _Show All Rows_ option from the row gripper to display the hidden rows.

<figure><img src="../../../../.gitbook/assets/image (17) (6).png" alt=""><figcaption></figcaption></figure>

e) Skip row

The _Skip row_ option performs a soft delete - the row is removed from the report and excluded from total and sub-total calculations.

<figure><img src="../../../../.gitbook/assets/image (18) (4).png" alt=""><figcaption></figcaption></figure>

The 'Furnishings' row has been removed using the _Skip row_ option and the totals and sub-totals have been adjusted accordingly.

<figure><img src="../../../../.gitbook/assets/image (20) (2).png" alt=""><figcaption></figcaption></figure>

f) Disable Subtotal

Use this option to remove all the sub-total aggregations for parent nodes in the hierarchy. This option is available in the row gripper for parent nodes only. In the animation below, notice how all the subtotal calculations have been removed using this option.

<figure><img src="../../../../.gitbook/assets/Disable subtotal (1).gif" alt=""><figcaption></figcaption></figure>



g) Set Subtotal below

This option will position the parent sub-total rows below the child rows. In the animation below, notice how the subtotal rows have been moved to the bottom, below all the child rows.

<figure><img src="../../../../.gitbook/assets/Setsubtotalbelow.gif" alt=""><figcaption></figcaption></figure>

