# Hierarchy settings

The general display settings are used to customize the appearance of the report.

In the Inforiver toolbar, navigate to the Home ribbon. The _Settings_ option is available in the 'Actions' section. Click **Settings > Display Settings** to open up the Display side panel.

Click on the Hierarchy tab in this panel to view the hierarchy settings.

<figure><img src="../.gitbook/assets/image (1350).png" alt=""><figcaption><p>Hierarchy settings</p></figcaption></figure>

Let's explore the options to customize hierarchies in your reports.

## 1. Header and Column

#### 1.1. Category highlight&#x20;

This drop-down lets you show or hide the category highlight. This option is set to 'Off' by default. When this option is enabled, a color picker is displayed. You can select a color to highlight the category hierarchy.

<figure><img src="../.gitbook/assets/image (28) (1).png" alt=""><figcaption><p>Cateory highlight</p></figcaption></figure>

#### 1.2. Responsive columns&#x20;

If this option is enabled, when the report canvas is resized to a small size, only columns that fit into the canvas will be displayed and others will be hidden.

<figure><img src="../.gitbook/assets/image (43).png" alt=""><figcaption><p>Responsive columns</p></figcaption></figure>

In the image below, after resizing the canvas to a much smaller size, out of the 3 measures added in the report, only 2 measures that fit into the view are displayed. This is because the responsive columns option is enabled.

<figure><img src="../.gitbook/assets/image (46).png" alt=""><figcaption><p>Report with responsive columns enabled</p></figcaption></figure>

#### 1.3. Show totals/subtotals values for non-numeric measures

You can add non-numeric measures like dates and text fields and display them in your reports. The first value is displayed in the total/subtotal cell by default, which may be irrelevant in an aggregated row. You can choose to leave the totals and subtotals blank for non-numeric fields by enabling this property.

<div><figure><img src="../.gitbook/assets/image (4) (1) (1) (2) (1).png" alt=""><figcaption><p>Non-numeric fields displayed as totals/subtotals</p></figcaption></figure> <figure><img src="../.gitbook/assets/numeric non-numeric.png" alt=""><figcaption><p>Totals/subtotals left blank for non-numeric fields</p></figcaption></figure></div>

#### 1.4. Combine column headers&#x20;

Enabling this option will combine the column headers and measure labels to display compact headers. As you can see from the below image, when this option is turned off, the column headers and measure labels are displayed separately.

<figure><img src="../.gitbook/assets/image (47).png" alt=""><figcaption><p>Combine column headers</p></figcaption></figure>

When this option is enabled, the column headers and measure labels are combined and displayed compactly. If the _Combine Column Header_ option is enabled, you can set a custom separator using the _Column header separator_ option.

<figure><img src="../.gitbook/assets/image (48).png" alt=""><figcaption><p>Combine column headers</p></figcaption></figure>

{% hint style="warning" %}
If the 'Combine column headers' option is enabled, you won't be able to reorder the columns.
{% endhint %}

#### Column header separator&#x20;

This option lets you specify the separator that will get inserted between the column header and the measure label.

#### 1.5. Ragged hierarchy&#x20;

In the case of ragged/unbalanced hierarchies where the number of levels is uneven, you can hide the blank category rows.&#x20;

<figure><img src="../.gitbook/assets/image (49).png" alt=""><figcaption><p>Ragged hierarchy option</p></figcaption></figure>

Notice how the blank categories under 'IT Expenses' and 'Other Expenses' have been hidden after enabling the _Ragged Hierarchy_ option.

<figure><img src="../.gitbook/assets/image (50).png" alt=""><figcaption><p>Ragged hierarchy sub-options</p></figcaption></figure>

On enabling ragged hierarchy, additional options are displayed:

* **Hide blanks**

Using this option you can choose to hide the rows if the category is blank, values are blank or both value and category are blank.

If your reports contain rows that only have an Others measure but no actuals, you can choose to suppress that row. Navigate to Hierarchy Settings and set the **Hide Blanks** dropdown to ‘Visible Values’. When you select Ignore Measure in Null Suppression from the column gripper, notice how the highlighted row is hidden.

<figure><img src="../.gitbook/assets/12.9. null-suppression-gif.gif" alt=""><figcaption><p>Null suppression</p></figcaption></figure>

* #### Suppress zeros&#x20;

If you enable this option, then the rows containing zeros will be suppressed.

{% hint style="info" %}
This option becomes available only if the option chosen in the Hide Blanks is 'Value' or 'Value+Category'.
{% endhint %}

* **Suppress null columns**

Columns containing null values will be suppressed if this option is enabled.

* **Hide blank label columns**

Columns with blank labels will be suppressed if this option is enabled.

* **Hide blank dimensions in column hierarchy**

When you have hierarchical column dimensions, there may be cases where the entire dimension category is blank as shown in the report below.

<figure><img src="../.gitbook/assets/5.1.1. Hide blank category.png" alt=""><figcaption><p>Blank categories in the column dimension</p></figcaption></figure>

Since these categories do not add value to the report, you can suppress them by enabling the **Hide blank dimensions in column hierarchy** option.

<figure><img src="../.gitbook/assets/5.1.2. Hidden blank category.png" alt=""><figcaption><p>Suppress blank categories in the column dimension</p></figcaption></figure>

#### 1.6. Row hierarchy icon

You can select custom icon styles to represent the row hierarchy i.e. choose the expand/collapse icons for hierarchical categories. If 'None' is selected, an icon will not be displayed.&#x20;

<figure><img src="../.gitbook/assets/image (51).png" alt=""><figcaption><p>Row hierarchy icon</p></figcaption></figure>

#### 1.7. Column hierarchy icon

You can select custom icon styles to represent the column hierarchy as well.

<figure><img src="../.gitbook/assets/image (54).png" alt=""><figcaption><p>Change the expand and collapse icons</p></figcaption></figure>

## 2. Expand to level

If your dataset contains hierarchies with multiple levels, you can choose to expand the hierarchy to a specific level at the initial load. This setting will be retained even after applying a filter/slicer.&#x20;

<figure><img src="../.gitbook/assets/image (52).png" alt=""><figcaption><p>Expand to level</p></figcaption></figure>

## 3. Mixed layout

You can display a chosen field as a separate column similar to the stepped layout. By default, it is set to 'None'. In the below image, the 'Sub Category' field has been selected and it gets displayed as a separate column in the visual.

{% hint style="info" %}
This option is available only in the Hierarchy layout when there are 3 or more levels in the row dimensions.
{% endhint %}

<figure><img src="../.gitbook/assets/image (53).png" alt=""><figcaption><p>Mixed layout</p></figcaption></figure>

## 4. Child

#### 4.1. Indent from parent&#x20;

This option lets you set the amount of indentation that has to be applied to the child rows from the parent row.

{% hint style="info" %}
The minimum and maximum indentation values are 1 and 25 respectively.
{% endhint %}

In the image below, every child row has been indented from its parent row by the specified amount.

<figure><img src="../.gitbook/assets/image (56).png" alt=""><figcaption><p>Indent from parent</p></figcaption></figure>

#### 4.2. Single child&#x20;

Using this option you can select which nodes to display when a parent hierarchy has only one child. In this example, we have a multi-level account hierarchy with several single-child rows and blank rows.&#x20;

The sales and marketing expenses row has only one child. The personnel cost row's child rows have blank rows. Let's see how this report is displayed for each of the options.

* **All** - Displays all the rows i.e. the parent rows and the single child rows. There are blank rows at levels 5 and 6.

<figure><img src="../.gitbook/assets/Single child all.png" alt=""><figcaption><p>Single child - All</p></figcaption></figure>

* **Parent only** - Displays the parent nodes of the single child. The blank rows at level 6 have all been hidden as shown below. The blank rows at level 5 are still shown.&#x20;

<figure><img src="../.gitbook/assets/Single child parent only.png" alt=""><figcaption><p>Single child - Parent only</p></figcaption></figure>

* **Parent (Multi-level) -** Displays only the highest level row of the multi-level hierarchy. The blank rows at both levels 5 and 6 are not shown.&#x20;

<figure><img src="../.gitbook/assets/Single child parent multilevel (1).png" alt=""><figcaption><p>Single child - Parent multi-level</p></figcaption></figure>

* **Single child level as parent -** Displays the single child as the parent of its level.&#x20;

Let's take a different scenario to explain the &#x53;_&#x69;ngle Child Level As Parent_ and &#x53;_&#x69;ngle Child As Parent_ options. As you can see below, under Operating expenses we have filtered only IT expenses. You can see blanks at levels 5 and 6.

<figure><img src="../.gitbook/assets/Single child level as parent 1.png" alt=""><figcaption><p>Single child at level 4</p></figcaption></figure>

On selecting &#x53;_&#x69;ngle Child Level As Parent_, you can see that the level 6 blank row is shown as the child for the level 4 row.

<figure><img src="../.gitbook/assets/Single child level as parent.png" alt=""><figcaption><p>Single child level as parent</p></figcaption></figure>

* **Single child as parent -** Displays only the single child at the lowest level. The blank row at level 6 is shown as the child for the level 3 row.

<figure><img src="../.gitbook/assets/Single child as parent 1 (1).png" alt=""><figcaption><p>Single child as parent</p></figcaption></figure>

## 5. Data window

#### 5.1. Max columns&#x20;

Inforiver supports wide table use cases through the dynamic columns feature. You can fetch up to 1000 columns, however, the performance would be compromised. &#x20;

Every fetch from Power BI is 30,000 cells (No of rows x No of columns). This means you can load data chunks of different sizes dynamically - 500 Rows by 60 Columns (or) 30 Rows by 1000 Columns (or) 10,000 Rows by 3 Columns.

You can view the current column count by hovering over the 'i' icon and modify the column count if needed.

<figure><img src="../.gitbook/assets/image (57).png" alt=""><figcaption><p>Column count</p></figcaption></figure>

Learn more about dynamically setting data chunk size using Power BI's [fetchMoreData API](https://learn.microsoft.com/en-us/power-bi/developer/visuals/fetch-more-data).

## 6. Row totals

You can customize the totals and subtotals by adding child count, padding, border, editing titles, and more. The available options are explained below.

#### 6.1. Show child count&#x20;

Enabling this option will display the count of child rows next to the name of the parent row in brackets.

<figure><img src="../.gitbook/assets/image (58).png" alt=""><figcaption><p>Show child count</p></figcaption></figure>

#### 6.2. Show descendants count&#x20;

You can also display the total number of children including the leaf nodes under a parent category.&#x20;

{% hint style="info" %}
Prerequisite: the **Show Child Count** option should be enabled.
{% endhint %}

<figure><img src="../.gitbook/assets/image (1353).png" alt=""><figcaption><p>Show descendants count</p></figcaption></figure>

#### 6.3. Top padding&#x20;

Using this option, you can configure the spacing/padding between row hierarchies.

<figure><img src="../.gitbook/assets/image (59).png" alt=""><figcaption><p>Top padding</p></figcaption></figure>

#### 6.4. Expand/collapse&#x20;

This option lets you specify when the expand/collapse icons for the hierarchies have to be displayed.

* **Always present** - Expand/collapse icon will be always present
* **Only on hover** - The expand/collapse icons are displayed only when you hover over the rows

<figure><img src="../.gitbook/assets/image (60).png" alt=""><figcaption><p>Expand/Collapse icons</p></figcaption></figure>

#### 6.5. Hide hierarchy icon

With this option, you can specify the fields for which you want to hide the hierarchy icon. All the fields are selected by default, and unselecting any field will hide the hierarchy icon for that field. In the below image, the 'Sub Category' field has been unselected, therefore the hierarchy icon for that field has been hidden.

<figure><img src="../.gitbook/assets/image (61).png" alt=""><figcaption><p>Hide hierarchy icon</p></figcaption></figure>

#### 6.6. Grand total title&#x20;

{% hint style="info" %}
The options related to Grand total can be seen only if the Row/Column Grand Total value has not been set to ‘Off’ under the ‘Totals’ option.&#x20;
{% endhint %}

You can set a custom title for the grand total in the textbox.

<figure><img src="../.gitbook/assets/image (62).png" alt=""><figcaption><p>Grand total title</p></figcaption></figure>

#### 6.7. Grand total height&#x20;

The value that you specify here will override the default height of the grand total row.

{% hint style="info" %}
The minimum and maximum values for grand total height are 5 and 45 respectively.
{% endhint %}

<figure><img src="../.gitbook/assets/image (63).png" alt=""><figcaption><p>Grand Total Height</p></figcaption></figure>

## 7. Total API

Inforiver pre-calculates the totals and subtotals for your data while loading the report. If your dataset is large and you do not require totals in your reports, you can substantially reduce the loading time of your report and boost its performance with the Total API option.&#x20;

You can disable the total and sub-total calculations for rows and columns separately.

<figure><img src="../.gitbook/assets/image (515).png" alt=""><figcaption><p>Total API</p></figcaption></figure>

#### 7.1. Row Total/Subtotal

Disable this to stop row-level total and sub-total calculations while loading your report.

#### 7.2. Column Total/Subtotal

Disable this to stop column-level total and sub-total calculations while loading your report.

Notice the time taken when Inforiver pre-calculates the totals and subtotals:&#x20;

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>When Totals are pre-calculated</p></figcaption></figure>

When the total calculation is disabled, even large datasets can be fetched in milliseconds as shown in the screengrab below.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1)  (14).png" alt=""><figcaption><p>After Disabling the Total API</p></figcaption></figure>

**Resources**

[Implementing tables with 100+ columns (wide tables) in Power BI](https://inforiver.com/blog/general/implementing-wide-tables-with-more-than-100-columns-in-power-bi/)

In this section, we covered the hierarchy display settings. Navigate to the next section to learn more about [advanced number formatting](number-settings.md).\
