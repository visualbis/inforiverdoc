# Column gripper

You can use the column gripper context menu to quickly sort or show/hide fields or insert a new field. Let's look at the various options in detail.

#### i) Sort

You can use the _Sort_ option to sort your data in ascending/descending order or apply an absolute sort.  For hierarchical datasets, sorting is applied to the child rows for each level of the hierarchy.

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption><p>Sort option</p></figcaption></figure>

In the example, the Jan > Profit measure has been sorted in ascending order.

<figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Sorted data for the Profit column</p></figcaption></figure>

#### ii) Insert

The _Insert_ option can be used for the following operations:

* **Copy as data input** - Create a new data input field. The values will be copied from the selected measure.
* **New data input** - Create a new empty data input field
* **Insert formula** - Create a new field using a built-in formula

Learn more about [data input](../../4.-adding-business-logic-and-formulae/insert-manual-input-rows.md) and [formula measures](../../4.-adding-business-logic-and-formulae/insert-calculated-columns.md).

<figure><img src="../../../.gitbook/assets/image (29) (2).png" alt=""><figcaption></figcaption></figure>

#### iii) Change to visual column

When you assign measures or dimensions to the AC/PY/PL/FC/Others parameters, the native measures and dimensions are displayed for each column dimension category. You can display them as visual columns by selecting the **Change to visual column** option.

<figure><img src="../../../.gitbook/assets/image (3).png" alt=""><figcaption><p>Change to visual column option</p></figcaption></figure>

Notice how the Profit measure has been converted into a visual column.

<figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Native measure converted into a visual column</p></figcaption></figure>

#### iv) Pin column

The pin column option allows you to tag important columns right at the beginning of your report - saving you the effort required to scroll back and forth.

<figure><img src="../../../.gitbook/assets/image (31) (3).png" alt=""><figcaption></figcaption></figure>

In the example, the Dec>Profits and Apr>Sales have been pinned to the beginning of the report.

<figure><img src="../../../.gitbook/assets/image (32) (2).png" alt=""><figcaption></figcaption></figure>

You can also choose to unpin a particular field or unpin all fields.

<figure><img src="../../../.gitbook/assets/image (33) (2).png" alt=""><figcaption></figcaption></figure>

#### iv) Stick Measure to Last

In some cases, using field measures can cause an automatic re-ordering of columns in the report. You may want a particular field, for instance, a field with an embedded chart,  to always retain its position at the end of the report. You can use the _Stick Measures to Last_ option to assign one designated measure to the last position. The last position will be retained even if new fields are added to the visual.

<figure><img src="../../../.gitbook/assets/image (41) (2).png" alt=""><figcaption><p>Stick measures to last</p></figcaption></figure>

#### v) Hide Column

You can use the _Hide Column_ option to mask a particular column in your report. In the animation below, notice how the Profit measure has been hidden in the report.&#x20;

{% hint style="info" %}
You can use the _Show All Columns_ option to display hidden columns again.
{% endhint %}

<figure><img src="../../../.gitbook/assets/Hidecolumn.gif" alt=""><figcaption></figcaption></figure>

#### vii) Aggregation

Using this option, you can directly set the aggregation method used to calculate the totals and subtotals for a particular column. Learn more about [managing aggregation](../../manage-aggregations/).

<figure><img src="../../../.gitbook/assets/image (46) (3).png" alt=""><figcaption></figcaption></figure>

#### viii) Select Measure

You may need to perform operations such as applying uniform formatting for a measure. Rather than selecting each measure and applying formatting, you can use this option to select a particular measure across the entire report and apply formatting in a single shot. In the animation below, notice how the Discount measure has been selected for all months.

<figure><img src="../../../.gitbook/assets/selectmeasure (2).gif" alt=""><figcaption></figcaption></figure>

#### ix) Number formatting

You can use this option to directly set a custom scaling factor for a particular measure.

<figure><img src="../../../.gitbook/assets/image (49) (2).png" alt=""><figcaption></figcaption></figure>

#### x) Show (-ve) Sign

Enable this option to enclose negative values in parentheses. In the report below, negative profits are displayed inside round brackets as the _Show (-ve) Sign_ option is enabled.

<figure><img src="../../../.gitbook/assets/image (50) (2).png" alt=""><figcaption></figcaption></figure>
