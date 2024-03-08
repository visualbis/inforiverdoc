# Manage aggregation

While working with Power BI table/matrix reports, we would sometimes like to apply custom measure aggregations in a specific report (e.g., average quantity sold) instead of using the default aggregation used in a data model (e.g., the sum of quantity sold).&#x20;

Inforiver’s aggregation feature allows you to override the native Power BI aggregation for measures without having to make extensive model-level changes.&#x20;

### 1. Report level

Aggregations such as sum, average, standard deviation, minimum, maximum, and visible rounding can be applied globally for all the measures in the report.&#x20;

{% hint style="info" %}
Report level aggregation can be set only when there are more than 3 measures in the report.
{% endhint %}

In the 'Insert' tab of the toolbar, click the 'Aggregation' button. You can see the 'Manage Aggregation' dialog box. To set global aggregation for the report, select the aggregation method from the dropdown for the 'All' element.&#x20;

<figure><img src="../.gitbook/assets/image (199).png" alt=""><figcaption><p>Manage Aggregation dialog box</p></figcaption></figure>

#### Native

By default, the 'Native' option is applied which follows the native summarization set in Power BI.&#x20;

<figure><img src="../.gitbook/assets/image (200).png" alt=""><figcaption><p>Native aggregation at report level</p></figcaption></figure>

#### None

Choosing 'None' performs no aggregations for the selected measure or hierarchy. In the example below, the 'Discount' measure is not aggregated.

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption><p>Aggregation is 'None'</p></figcaption></figure>

#### Sum

'Sum' aggregation displays the sum of the immediate child nodes as the aggregate. In the highlighted example, the 'Computers' category is the sum of its immediate child nodes.

<figure><img src="../.gitbook/assets/image (201).png" alt=""><figcaption><p>Sum aggregation type at report level</p></figcaption></figure>

#### Minimum

'Minimum' aggregation displays the minimum value of the immediate child node as the aggregate. In the below example, the 'Computers' category displays the minimum value of its immediate child nodes which is 'Computers Accessories'.

<figure><img src="../.gitbook/assets/image (202).png" alt=""><figcaption><p>Minimum aggregation type at report level</p></figcaption></figure>

#### Maximum

'Maximum' aggregation displays the maximum value of the immediate child node as the aggregate. In the below image, the 'Computers' category displays the maximum value of its immediate child nodes which is 'Projectors and Screens'.

<figure><img src="../.gitbook/assets/image (203).png" alt=""><figcaption><p>Maximum aggregation type at report level</p></figcaption></figure>

#### Average (Children)

'Average (Children)' aggregation displays the average value of the immediate child nodes as the row aggregation. In the below example,  'Computers' category is calculated as the average of the immediate child nodes i.e. the 'SubCategory' field.

<figure><img src="../.gitbook/assets/image (204).png" alt=""><figcaption><p>Average(children) aggregation type at report level</p></figcaption></figure>

#### Average (Leaf)

'Average (Leaf)' aggregation displays the average value of all the leaf nodes of the row category as the row aggregation. In the below example, 'Computers' is calculated as the average of the leaf nodes i.e. the 'Class' field.

<figure><img src="../.gitbook/assets/image (205).png" alt=""><figcaption><p>Average(leaf) aggregation type at report level</p></figcaption></figure>

#### Standard deviation

'Standard deviation' aggregation displays the standard deviation of the child rows as the aggregate. In the below example, 'Computers' is calculated as the standard deviation of its immediate child nodes.

<figure><img src="../.gitbook/assets/image (206).png" alt=""><figcaption><p>Standard Deviation as aggregation type at report level</p></figcaption></figure>

#### Visible rounding

'Visible rounding' aggregation rounds off values in a way that the individual values add up properly to the subtotal' and grand total. This is a very common requirement in external financial statement reporting such as the income statement and balance sheet reporting.

<figure><img src="../.gitbook/assets/image (207).png" alt=""><figcaption><p>Visible Rounding as aggregation type at report level</p></figcaption></figure>

### 2. Column level

The 'Manage aggregation' option allows you to manage aggregations for specific measures.

a) In the 'Insert' tab of the toolbar, click on the 'Aggregation' button to open the 'Manage Aggregation' dialog box.

{% hint style="info" %}
Another way to access 'Manage Aggregation' is by clicking on 'Manage columns' and then the 'Settings' icon.

Alternatively, click on the column gripper and select 'Manage Aggregation' from the Aggregation section of the context menu.
{% endhint %}

b) A pop-up opens showing a list of measures under the 'Display' section. You can change the aggregation type of multiple measures here.

<figure><img src="../.gitbook/assets/Display (2).png" alt=""><figcaption><p>Manage columns pop-up</p></figcaption></figure>

c) Let's change the aggregation for '2020 Actuals' from 'Sum' to 'Maximum'. Select 'Maximum' aggregation from the dropdown.&#x20;

<figure><img src="../.gitbook/assets/Change agg.png" alt=""><figcaption><p>Column aggregation</p></figcaption></figure>

d) In the below image, you can see that East -> 2020 Actuals shows 40.18 which is the maximum of Beverages and Water, whereas East -> 2020 Plan shows 45.03 which is the sum of the two categories. &#x20;

<figure><img src="../.gitbook/assets/Sum &#x26; maximum aggregation.png" alt=""><figcaption><p>Sum &#x26; maximum aggregation</p></figcaption></figure>

{% hint style="info" %}
Report-level and column-level aggregations are applicable only for the data source rows.
{% endhint %}

e) In the below image, you can see that the aggregation field is disabled for the simulation column. Note that the [row aggregation type](../working-with-inforiver/4.-adding-business-logic-and-formulae/insert-manual-input-columns/insert-manual-input-columns.md#i-row-aggregation-type) for calculated columns and manual data input columns can be defined here in the 'Manage columns' dialog box in addition to the 'Insert formula' and 'Data input' side panels. &#x20;

<figure><img src="../.gitbook/assets/For.png" alt=""><figcaption><p>Simulation column </p></figcaption></figure>

### 3. Hierarchy level

If your data is hierarchical, Inforiver offers the flexibility to apply row aggregations on a selected branch of the hierarchy, for an entire hierarchy level and different aggregation methods for different levels simultaneously.

#### i) Selected parent row of a hierarchy

The global aggregation set at report level can be overridden and you can apply the required row aggregation method on a parent row. Click on the row gripper for the parent row, from the 'Aggregation' section of the menu, select the aggregation type.

<figure><img src="../.gitbook/assets/image (193).png" alt=""><figcaption><p>Selecting parent level aggregation</p></figcaption></figure>

Row level aggregation has been set to Minimum for the 'TV and Video' category while the other categories retain the Native Power BI aggregation.

<figure><img src="../.gitbook/assets/image (196).png" alt=""><figcaption><p>Row level aggregation set to minimum</p></figcaption></figure>

#### ii) Particular level of a hierarchy

To apply a uniform aggregation method to a given level of the hierarchy, from the Insert ribbon, select the 'Aggregation' option from the 'Customize' section. Navigate to the 'Category' tab of the Manage Aggregation dialog box . Notice that we can assign different aggregation methods for different levels of the hierarchy.

<figure><img src="../.gitbook/assets/image (197).png" alt=""><figcaption><p>Aggregation types for different levels of the hierarchy</p></figcaption></figure>

The specified aggregation method is set for a specific level of the hierarchy.

<figure><img src="../.gitbook/assets/image (198).png" alt=""><figcaption></figcaption></figure>



In the next section, we'll be covering the[ Invert sign](invert-sign.md) feature.

#### Resources

[Change & manage aggregation in Power BI matrix](https://inforiver.com/blog/feature-highlights/define-visual-aggregation-power-bi-table-matrix/)
