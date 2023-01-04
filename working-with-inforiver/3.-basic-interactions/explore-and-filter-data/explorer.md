# Explorer

KPI explorer can be used to filter rows, columns and measures, sort by name or value and highlight row hierarchies using rules or ranges. Let's take a detailed look.

<figure><img src="../../../.gitbook/assets/3.1.2.1 Explorer.png" alt=""><figcaption><p>KPI Explorer</p></figcaption></figure>

### 1. Overview

In this report, we have Region and Category hierarchies in rows, Dates in columns and Actuals and Plan as measures.&#x20;

Outline layout is used in this example, but all table and measure layouts are supported when using KPI Explorer.

a) Click on the 'Explorer' icon in the 'Analyze' section of the 'Home' tab. &#x20;

<figure><img src="../../../.gitbook/assets/3.1.2.2 Explorer.png" alt=""><figcaption><p>KPI Explorer</p></figcaption></figure>

b) KPI Explorer menu gets enabled as shown. Let's go to the full view. Click on the arrow highlighted and select the 'Explorer full view' option.

<figure><img src="../../../.gitbook/assets/3.1.2.3 Explorer.png" alt=""><figcaption><p>KPI Explorer menu</p></figcaption></figure>

c) The KPI Explorer full view is shown below. Let's minimize the toolbar to maximize real estate. Click on the highlighted arrow and select 'Unpin toolbar'.&#x20;

<figure><img src="../../../.gitbook/assets/3.1.2.4 Explorer.png" alt=""><figcaption><p>KPI Explorer full view</p></figcaption></figure>

d) The toolbar gets unpinned.&#x20;

<figure><img src="../../../.gitbook/assets/3.1.2.5 Explorer.png" alt=""><figcaption><p>KPI Explorer</p></figcaption></figure>

e) Let's take a look at filtering by the row and column hierarchies. Use the date filter slider to define a date range. Select a region and category. You can see that the sub-region and sub-category get filtered accordingly in the explorer menu.&#x20;

In the table, you can now see only United States and Beverages for Q3 2020 to Q2 2021.

<figure><img src="../../../.gitbook/assets/3.1.2.6 Explorer (1).png" alt=""><figcaption><p>Filtering rows and columns</p></figcaption></figure>

f)  Clear the selections by clicking on the highlighted arrow and then the 'Clear all' option.

<figure><img src="../../../.gitbook/assets/3.1.2.6(2) Explorer.png" alt=""><figcaption><p>Clearing selections</p></figcaption></figure>

### 2. Filtering

a) As you can see, there is a value against each hierarchy. Let's look at how the values are calculated. Since the measure selected in the dropdown is 'Actuals', you can see the actuals value for All and United States highlighted as (1) and (2).

<figure><img src="../../../.gitbook/assets/3.1.2.7(2) Explorer.png" alt=""><figcaption><p>Actuals for All and United States</p></figcaption></figure>

{% hint style="info" %}
Turn on the 'Column grand total' from the 'Totals' menu.
{% endhint %}

b) As shown in the below image, you can see the values highlighted in the case of the sub-regions.

<figure><img src="../../../.gitbook/assets/3.1.2.8 Explorer.png" alt=""><figcaption><p>Actuals for sub-regions</p></figcaption></figure>

c) To verify the values for categories and sub-categories, change the order of row and column hierarchies in the data mapping.

<figure><img src="../../../.gitbook/assets/3.1.2.10 Explorer.png" alt=""><figcaption><p>Actuals for categories and sub-categories</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/3.1.2.11 Explorer.png" alt=""><figcaption><p>Actuals for categories and sub-categories</p></figcaption></figure>

d) You can also explore other measures. Click on the dropdown highlighted and select 'Plan'.

<figure><img src="../../../.gitbook/assets/3.1.2.12 Explorer.png" alt=""><figcaption><p>Exploring different measures</p></figcaption></figure>

e) The values get updated accordingly. As you can see, the values add up to 890.60 in all four hierarchies.

<figure><img src="../../../.gitbook/assets/3.1.2.13 Explorer.png" alt=""><figcaption><p>Exploring Plan for regions</p></figcaption></figure>

f) When you apply filters, let's explore how the values are displayed.

1. International -> EMEA is 228.56 million, which is displayed as the total for all four hierarchies.
2. International and United States are 337.91 and 552.69 million as seen in earlier images.
3. EMEA is 228.56 million and the Plan values for other sub-regions are displayed accordingly.
4. International -> EMEA -> Water is 58.31 million as can be seen in the below image.
5. International -> EMEA -> Beverages -> Soda is 68.34 million.

<figure><img src="../../../.gitbook/assets/3.1.2.14 Explorer.png" alt=""><figcaption><p>Understanding the values on filtering</p></figcaption></figure>

g) The date filter slider toggle can be turned off to list the date hierarchy as filters.&#x20;

<figure><img src="../../../.gitbook/assets/3.1.2.15 Explorer.png" alt=""><figcaption><p>Date filter</p></figcaption></figure>

### 3. Customizations

a) To hide certain KPIs, click on the arrow highlighted and the 'Show KPI' option.

<figure><img src="../../../.gitbook/assets/3.1.2.16 Explorer.png" alt=""><figcaption><p>Show/hide KPIs</p></figcaption></figure>

b) KPIs can be hidden as shown.

<figure><img src="../../../.gitbook/assets/3.1.2.17 Explorer.png" alt=""><figcaption><p>Hiding sub-categories and month</p></figcaption></figure>

c) Sorting can be done based on values or names. To sort the categories by values, click on the gripper icon and 'Sort by values'. Select 'Ascending'.

<figure><img src="../../../.gitbook/assets/3.1.2.18 Explorer.png" alt=""><figcaption><p>Sorting by name or values</p></figcaption></figure>

d) Sorting gets applied. You can see an icon as shown in the image that shows the applied sorting.

<figure><img src="../../../.gitbook/assets/3.1.2.19(2) Explorer.png" alt=""><figcaption><p>Sorting by values</p></figcaption></figure>

e) You can apply highlighting rules to the KPIs. Click on the 'Flag' icon as shown. There are two options - Rules and Ranges. Let's apply based on a range. You can define ranges based on percentage values or numeric values. Let's go with the default. Click 'Apply'.

<figure><img src="../../../.gitbook/assets/3.1.2.20(2) Explorer.png" alt=""><figcaption><p>Highlighting using rules or ranges</p></figcaption></figure>

f) The values get highlighted as shown. The flag icon is also modified to indicate that highlights have been applied.

<figure><img src="../../../.gitbook/assets/3.1.2.21 Explorer.png" alt=""><figcaption><p>Highlights based on ranges</p></figcaption></figure>

g) You can add ranges, reverse the icons and colors and delete ranges using the highlighted icons.

<figure><img src="../../../.gitbook/assets/3.1.2.22 Explorer.png" alt=""><figcaption><p>Customizing the ranges</p></figcaption></figure>

h) To 'reset' the ranges to default, click on the highlighted icon.

<figure><img src="../../../.gitbook/assets/3.1.2.23 Explorer.png" alt=""><figcaption><p>Reset changes</p></figcaption></figure>

i) Ranges based on numeric values are shown below.

<figure><img src="../../../.gitbook/assets/3.1.2.24 Explorer.png" alt=""><figcaption><p>Range based on numeric values</p></figcaption></figure>

j) To apply highlights based on rules, select the 'Rules' option. Apply a rule as shown and click 'Apply'. The values are highlighted as shown.

<figure><img src="../../../.gitbook/assets/3.1.2.25 Explorer.png" alt=""><figcaption><p>Highlights based on rules</p></figcaption></figure>





