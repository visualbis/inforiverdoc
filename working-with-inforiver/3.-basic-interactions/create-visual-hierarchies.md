# Create visual hierarchies

With Inforiver, visual hierarchies in rows & columns can be created by selecting multiple items and grouping them. In the case of row grouping, the subtotal values are calculated automatically.

You can also create row groups automatically based on Conditional formatting - Classification.&#x20;

## 1. Group columns

In the below example, the columns are to be grouped and named Revenue, Profitability, and Customers respectively.

{% hint style="info" %}
The group icon is greyed out until a row or column is selected.
{% endhint %}

a) Select the columns to be grouped as Revenue. In the 'Insert' tab, click on '**Group**' and then '**Add new group**'. The other options in the dropdown will be covered in the next section.

<figure><img src="../../.gitbook/assets/3.7.2 Column groups.png" alt=""><figcaption><p>Adding a column group</p></figcaption></figure>

b) Enter a label for the group as shown below and click 'Apply'.

<figure><img src="../../.gitbook/assets/3.7.3 Column groups.png" alt=""><figcaption><p>Naming the group</p></figcaption></figure>

c) The column group gets created and it can be formatted using the 'Style' and 'Alignment' options as shown below.

<figure><img src="../../.gitbook/assets/3.7.4 Column groups.png" alt=""><figcaption><p>Groups can be formatted using Style and Alignment options</p></figcaption></figure>

d) The other groups can be created and formatted as shown.

<figure><img src="../../.gitbook/assets/3.7.5 Column groups.png" alt=""><figcaption><p>Three column groups created</p></figcaption></figure>

## 2. Group rows

### i) Manual grouping

a) On selecting a column or multiple columns, the 'Group' icon gets enabled. Select the rows to be grouped and click on '**Group**' in the 'Insert' tab. A popup opens.

<figure><img src="../../.gitbook/assets/3.7.7 Row groups.png" alt=""><figcaption><p>Row grouping - label and total position</p></figcaption></figure>

b) Enter the row group label and set the total position. Click 'Apply'.

<figure><img src="../../.gitbook/assets/3.7.8 Row groups.png" alt=""><figcaption><p>Row grouping options configured</p></figcaption></figure>

c) The rows are indented to indicate that they are a part of a child hierarchy. The measures are automatically aggregated. A bar chart is displayed for the Margin column.

<figure><img src="../../.gitbook/assets/3.7.9 Row groups (1).png" alt=""><figcaption><p>Row grouping created</p></figcaption></figure>

d) The row groups can be expanded/collapsed using the expand/collapse button.

<figure><img src="../../.gitbook/assets/3.7.10 Row groups.png" alt=""><figcaption><p>Expand/collapse enabled row grouping</p></figcaption></figure>

### ii) Auto grouping

Conditional formatting has been covered in detail in [section 5](../5.-conditional-formatting.md). For the purposes of exploring auto grouping of rows based on classification, we'll just look at the settings in brief.

In this example, classification rules are applied to Margin %. High/Medium/Low is displayed next to the Margin % values based on the applied ranges.

<figure><img src="../../.gitbook/assets/3.7.11 Auto Row groups.png" alt=""><figcaption><p>Conditional formatting - Classification</p></figcaption></figure>

a) In the 'Insert' tab, click on 'Group' and select the 'Margin %' option.

<figure><img src="../../.gitbook/assets/3.7.12 Auto Row groups.png" alt=""><figcaption><p>Auto grouping based on classification</p></figcaption></figure>

b) Rows are automatically grouped as shown below.

<figure><img src="../../.gitbook/assets/3.7.13 Auto Row groups.png" alt=""><figcaption><p>Row groups created</p></figcaption></figure>

## 3) Ungroup&#x20;

### i) Columns

To remove a column group, click on the column group label, the '**Remove group**' icon, and the 'Remove group' option.

<figure><img src="../../.gitbook/assets/3.7.16 Remove column groups.png" alt=""><figcaption><p>Removing column group</p></figcaption></figure>

### ii) Rows&#x20;

a) In case of manually grouped rows, select the group and click on the '**Remove group**' icon in the 'Insert' tab.&#x20;

<figure><img src="../../.gitbook/assets/3.7.14 Remove Row groups.png" alt=""><figcaption><p>Removing row group</p></figcaption></figure>

b) In case of auto-grouped rows, in the 'Insert' tab, '**Group**' dropdown, select '**None**'.

<figure><img src="../../.gitbook/assets/3.7.15 Remove auto row groups.png" alt=""><figcaption><p>Removing auto row group based on classification</p></figcaption></figure>

In the next section, we'll cover how to [pin rows and columns](pin-rows-and-columns.md).
