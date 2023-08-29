# Top N + others

Top N answers questions such as _Customers_ contributing to the most revenue, _Spend Categories_ that consume most of the budget etc.&#x20;

{% embed url="https://lumel.wistia.com/medias/z9pzrtc9oy" %}
Top N + Others - Overview
{% endembed %}

In this section, let us see how the Top N feature works in Inforiver.&#x20;

Consider the example of displaying the Top 2 categories which generated maximum Revenue.

a) Select the Revenue column.

b) In the 'Home' tab of the toolbar, select 'Top n' from the 'Analyze' section. The Top N dialog box appears. Fill in the details to filter the Top 2 categories. Click 'Apply'.

{% hint style="info" %}
To show the top 2% of items, just change the selection ‘Value’ to ‘Percentage’.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (169).png" alt=""><figcaption><p>Top N dialog box</p></figcaption></figure>

c) You can see the top 2 categories with the remaining categories grouped under 'Others'_._ It also indicates how many items are a part of the 'Others' row.

<figure><img src="../../../.gitbook/assets/image (170).png" alt=""><figcaption><p>Others section</p></figcaption></figure>

d) Hover over the 'Others' row to see a preview of the items grouped under Others.  Click on the expand icon to view all the categories that have been classified as Others. This will display all the categories under 'Others' in a separate window.

<figure><img src="../../../.gitbook/assets/image (171).png" alt=""><figcaption><p>Others category details</p></figcaption></figure>

e) To remove a category from the Others group, right click on the category and select the 'Remove from others' options from the menu.

<figure><img src="../../../.gitbook/assets/image (194).png" alt=""><figcaption><p>Remove from others option</p></figcaption></figure>

Notice how the selected category has been removed from the 'Others' group.&#x20;

<figure><img src="../../../.gitbook/assets/image (195).png" alt=""><figcaption><p>Remove from others result</p></figcaption></figure>

### 1. Nested rules

a) To do a nested Top N, like the bottom 3 sub-categories in each of the top 2 categories, you can create multiple rules by clicking ‘Add rule’ and filling in the fields as shown. Click 'Apply'.

<figure><img src="../../../.gitbook/assets/Add rule (2).png" alt=""><figcaption><p>Nested rules</p></figcaption></figure>

b) The above setup displays the following output. Note that the 'Others' row is available for categories and subcategories.

<figure><img src="../../../.gitbook/assets/Nested Top N.png" alt=""><figcaption><p>Nested top N</p></figcaption></figure>

### 2. Multi-level nested rules

a) You can increase the number of hierarchy levels even beyond two (2). Add rules as below to configure the third category.

<figure><img src="../../../.gitbook/assets/Multilevel nested top n.png" alt=""><figcaption><p>Multilevel nested top N</p></figcaption></figure>

This configuration gives the following output.&#x20;

<figure><img src="../../../.gitbook/assets/Multilevel top N result.png" alt=""><figcaption><p>Multilevel top N result</p></figcaption></figure>

### 3. Suffix ‘Others’

When using the multi-level and nested Top N implementation, it may not be clear as to what a specific 'Others' row refers to.

<figure><img src="../../../.gitbook/assets/Others (1).png" alt=""><figcaption><p>Suffix others</p></figcaption></figure>

To address this, Inforiver provides an option that appends the category name to 'Others' for each instance of others, except the one at the outer-most level.

<figure><img src="../../../.gitbook/assets/Suffix with category (1).png" alt=""><figcaption><p>Suffix others with category name</p></figcaption></figure>

To delete a Top N condition, click on the 'Delete' icon. To clear all the Top N conditions, click on 'Reset all'.

<figure><img src="../../../.gitbook/assets/Reset,delete (1).png" alt=""><figcaption><p>Delete &#x26; reset</p></figcaption></figure>

A warning message gets displayed when you try to apply Top N on more than one column/measure. You need to remove the existing filter and apply a new one to the selected column by clicking on 'Remove and proceed'.

<figure><img src="../../../.gitbook/assets/Warning.png" alt=""><figcaption><p>Applying top N filter on multiple columns throws a warning</p></figcaption></figure>

In the next section, we'll be covering [sorting & reordering data](../sort-and-reorder-data.md).

#### Resources

[The Business Case for dynamic & nested Top N + Others reports](https://inforiver.com/blog/general/the-business-case-for-dynamic-nested-top-n-others-reports/)

[Dynamic and nested Top N + Others in Power BI](https://inforiver.com/blog/general/dynamic-and-nested-top-n-others-in-power-bi/)
