# Top N

In this section, let us see how the Top N feature works in Inforiver. Top N answers questions such as _Customers_ contributing to the most revenue, _Spend Categories_ that consume most of the budget etc.

Consider the example of displaying the Top 5 Cities by Sales for each Subcategory.

a) Select the Sales (2016 Sales) column.

b) In the 'Home' tab of the toolbar, select 'Top N' from the 'Analyze' section.

<figure><img src="../../../.gitbook/assets/Top N.png" alt=""><figcaption><p>Top n</p></figcaption></figure>

c) In the Top N dialog box that appears, input the following fields:

* Top/Bottom/Both: Both displays Top and Bottom values (Both)
* Number of items (5)
* Condition-based on Value or Percentage (Value)
* Field to which condition to be applied (Sub-Category)

<figure><img src="../../../.gitbook/assets/Choose from Top, Bottom or Both.png" alt=""><figcaption><p>Choose from Top, Bottom or Both</p></figcaption></figure>

d) To display the remaining categories as Others, check the respective checkbox. Inorder to customize the name “Others”, click on the Pen icon.

e) Check “Suffix Others with category name”, to display the category label along with Others.

<figure><img src="../../../.gitbook/assets/Aggregate the Rest as Others.png" alt=""><figcaption><p>Aggregate &#x26; Suffix Others</p></figcaption></figure>

f) Click Apply, the result is shown below.

<figure><img src="../../../.gitbook/assets/Top 5 Subcategory based on the Value.png" alt=""><figcaption><p>Top 5 Subcategory based on the Value</p></figcaption></figure>

g) To apply another Top n condition, follow the same procedure as illustrated above.

* In the Top n dialog box, click on Add rule.
* Select the fields as shown in the below image:

<figure><img src="../../../.gitbook/assets/Add Rule.png" alt=""><figcaption><p>Add rule</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/Showing result with added rule (1).png" alt=""><figcaption><p>Showing result with added rule</p></figcaption></figure>

h) To delete a Top n condition, click on the respective Delete icon.

i) To clear all the Top n conditions, click on Reset All Button.

<figure><img src="../../../.gitbook/assets/Reset,delete.png" alt=""><figcaption><p>Delete &#x26; reset</p></figcaption></figure>

{% hint style="info" %}
A warning message gets displayed when you try to apply Top n on more than one column/measure.
{% endhint %}

<figure><img src="../../../.gitbook/assets/warning.png" alt=""><figcaption><p>Warning message</p></figcaption></figure>

In the next section, we'll look at&#x20;
