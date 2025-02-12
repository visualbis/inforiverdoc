# Inforiver Writeback Matrix December 2024 - v3.7 - Merge rows, new rounding functions & More

We are excited to present the new Merge Rows feature that enables you to seamlessly sync your visual-level and native row data. We've also added variations to the ROUND function along with enhancements across Infobridge, MoR layout, and data inputs to bring you a superior business reporting experience.&#x20;

Discover the new features and innovations that make Inforiver Matrix the most powerful collaborative planning solution in Power BI.

## 1. Merge rows from the semantic model

As businesses evolve, so too does the scope of their data. You may be expanding to new regions or adding new product lines - with the [Static Row](../working-with-inforiver/4.-adding-business-logic-and-formulae/insert-manual-input-rows.md#id-1.-insert-static-row), [Insert Rows(s)](../working-with-inforiver/4.-adding-business-logic-and-formulae/insert-manual-input-rows.md#id-2.-bulk-insert-static-rows), and [Row Hierarchy](../working-with-inforiver/4.-adding-business-logic-and-formulae/insert-manual-input-rows.md#id-3.-row-hierarchy) options, you can add dimension categories on the fly. When the same category exists at the visual level and in your semantic model, you will now be able to merge the rows from your dataset. &#x20;

The <img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="" data-size="line">icon that indicates a manual input row will be replaced by<img src="../.gitbook/assets/image (1061).png" alt="" data-size="line">, which indicates a merged row for a row dimension category that is available in the source system. Click the icon to merge the row.

{% hint style="info" %}
Data input fields will be locked for editing until the row is merged.
{% endhint %}

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Merging visual rows with native rows</p></figcaption></figure>

Notice how the merge icon disappears and the data input field becomes editable after merging the EURIBOR row. When you merge rows, static rows are replaced with native rows however data inputs are retained.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Merged row</p></figcaption></figure>

## 2. New rounding functions: MROUND, ROUNDUP, and ROUNDDOWN

In business intelligence reporting, accuracy and precision in handling numerical data is essential for planning, budgeting and forecasting. Inforiver gives you additional control over rounding your data with adaptable rounding options:

**Choosing the right rounding function**

* Use **ROUND** for standard rounding needs
* The **MROUND** function rounds a number to the nearest multiple of a specified value. Ideal for scenarios like rounding to the nearest 5, 10, or 100, often used in inventory management.
* The **ROUNDUP** function always rounds a number up, away from zero. Use ROUNDUP when you always need a higher estimate, such as in budgeting or safety margins.
* The **ROUNDDOWN** function always rounds a number down, toward zero. Use ROUNDDOWN for conservative estimates, like minimizing costs.

<figure><img src="../.gitbook/assets/image (9) (1) (1) (1).png" alt=""><figcaption><p>Rounding functions in Inforiver</p></figcaption></figure>

## 3. Checkboxes in MOR layout

Inforiver's popular Measure on Rows layout now supports checkboxes in addition to data input types like numeric values, text fields, dropdown menus and Last updated at/by metadata.

<figure><img src="../.gitbook/assets/image (7) (1) (1) (1) (1).png" alt=""><figcaption><p>Checkboxes in MOR layout</p></figcaption></figure>

## 4. Actionable error messages in Infobridge

Have you ever encountered data processing error messages that were too technical and left you at a loss? Infobridge has been updated with clearer, actionable error messages designed to help you quickly pinpoint and resolve the issue.

<figure><img src="../.gitbook/assets/image (10) (1).png" alt=""><figcaption><p>Simplified error messages in Infobridge</p></figcaption></figure>

## 5. Total and subtotals for non-numeric data inputs

You can input data in the total and subtotal rows for non-numeric fields without having to tweak any settings. The **Allow entry on total/subtotal rows** is pre-enabled to ensure a smooth experience. &#x20;

<figure><img src="../.gitbook/assets/image (8) (1) (1) (1) (1).png" alt=""><figcaption><p>Total and subtotal entries for non-numeric data input fields</p></figcaption></figure>
