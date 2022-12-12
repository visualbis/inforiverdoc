# Create visual hierarchies

With Inforiver, you can create visual hierarchies in rows & columns by selecting multiple items and grouping them. When you group rows, the subtotal values are calculated automatically.

You can also create row groups automatically based on Conditional formatting - Classification.

Let us look at these features in detail.  &#x20;

## 1. Group columns

In the below example, let's group the columns as shown and name them Revenue, Profitability, and Customers respectively.

<figure><img src="../../.gitbook/assets/3.7.1 Column groups.png" alt=""><figcaption><p>Columns to be grouped</p></figcaption></figure>

Select the columns to be grouped as Revenue. In the 'Insert' tab, click on 'Group' and then 'Add new group'. We'll cover the other options in the dropdown in the next section.

<figure><img src="../../.gitbook/assets/3.7.2 Column groups.png" alt=""><figcaption><p>Adding a column group</p></figcaption></figure>

Enter a label for the group as shown below and click 'Apply'.

<figure><img src="../../.gitbook/assets/3.7.3 Column groups.png" alt=""><figcaption><p>Naming the group</p></figcaption></figure>

The column group gets created and you can format it using the 'Style' and 'Alignment' options as shown below.

<figure><img src="../../.gitbook/assets/3.7.4 Column groups.png" alt=""><figcaption><p>Groups can be formatted using Style and Alignment options</p></figcaption></figure>

You can group the other columns similarly.

<figure><img src="../../.gitbook/assets/3.7.5 Column groups.png" alt=""><figcaption><p>Three column groups created</p></figcaption></figure>

## 2. Group rows

### a) Manual grouping

Let us explore row grouping. In the below example, let's group the highlighted rows and name it 'Kitchen appliances'.

<figure><img src="../../.gitbook/assets/3.7.6 Row groups.png" alt=""><figcaption><p>Rows to be grouped as Kitchen appliances</p></figcaption></figure>

Select the rows and click on 'Group' in the 'Insert' tab. A popup opens.

<figure><img src="../../.gitbook/assets/3.7.7 Row groups.png" alt=""><figcaption><p>Row grouping - label and total position</p></figcaption></figure>

Enter the row group label and set the total position. Click 'Apply'.

<figure><img src="../../.gitbook/assets/3.7.8 Row groups.png" alt=""><figcaption><p>Row grouping options configured</p></figcaption></figure>

The rows are indented to indicate that they are a part of a child hierarchy. You can see that the measures are automatically aggregated. A bar chart is displayed for the Margin column.

<figure><img src="../../.gitbook/assets/3.7.9 Row groups.png" alt=""><figcaption><p>Row grouping created</p></figcaption></figure>

Click on the expand/collapse button next to kitchen appliances.&#x20;

<figure><img src="../../.gitbook/assets/3.7.10 Row groups.png" alt=""><figcaption><p>Expand/collapse enabled row grouping</p></figcaption></figure>

### b) Auto grouping

Conditional formatting has been covered in detail in [section 5](../5.-conditional-formatting.md). For the purposes of exploring auto grouping of rows based on classification, we'll just look at the settings in brief.

In this example, classification rules are applied to Margin %. High/Medium/Low is displayed next to the Margin % values based on the applied ranges.

<figure><img src="../../.gitbook/assets/3.7.11 Auto Row groups.png" alt=""><figcaption><p>Conditional formatting - Classification</p></figcaption></figure>

In the 'Insert' tab, click on 'Group' and select the 'Margin %' option.

<figure><img src="../../.gitbook/assets/3.7.12 Auto Row groups.png" alt=""><figcaption><p>Auto grouping based on classification</p></figcaption></figure>

You can see that the rows are segmented as shown below.

<figure><img src="../../.gitbook/assets/3.7.13 Auto Row groups.png" alt=""><figcaption><p>Row groups created</p></figcaption></figure>

## 3) Ungroup&#x20;

### a) Columns

To remove a column group, click on the column group label, the 'Remove group' icon, and the 'Remove group' option.

<figure><img src="../../.gitbook/assets/3.7.16 Remove column groups.png" alt=""><figcaption><p>Removing column group</p></figcaption></figure>

### b) Rows&#x20;

1\) In case of manually grouped rows, select the group and click on the 'Remove group' icon in the 'Insert' tab.&#x20;

<figure><img src="../../.gitbook/assets/3.7.14 Remove Row groups.png" alt=""><figcaption><p>Removing row group</p></figcaption></figure>

2\) In case of auto-grouped rows, in the 'Insert' tab, 'Group' dropdown, select 'None'.

<figure><img src="../../.gitbook/assets/3.7.15 Remove auto row groups.png" alt=""><figcaption><p>Removing auto row group based on classification</p></figcaption></figure>

