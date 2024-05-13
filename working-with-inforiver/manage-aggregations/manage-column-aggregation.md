# Manage column aggregation

In addition to configuring the row aggregation, you can also configure the column aggregation. Like row aggregation, which only applies to sub-total and grand-total rows, column aggregation applies only to the subtotal and grand-total columns.

Let us first demonstrate these aggregations for total rows with a few examples, followed by the 'Manage Aggregation' dialog box where you can perform both row and column aggregations in tandem.

## Column aggregation for a total cell

To apply column aggregation, click on the cell in the grand-total/subtotal column and select the aggregation type from the dropdown menu.

<figure><img src="../../.gitbook/assets/image (642).png" alt=""><figcaption><p>Click on the 'Aggregation' drop-down</p></figcaption></figure>

{% hint style="info" %}
The Aggregation drop-down menu gets enabled when you click on any cell that aggregates rows and/or columns.
{% endhint %}

You can see in the above example the default aggregation is the sum of column values for the _Canada_ region.

Let us now change it to 'Maximum'.&#x20;

<figure><img src="../../.gitbook/assets/image (643).png" alt=""><figcaption><p>Changing aggregation to 'Maximum'</p></figcaption></figure>

As a result, the grand total is populated with the maximum value of all the quarters.

<figure><img src="../../.gitbook/assets/image (644).png" alt=""><figcaption><p>'Maximum' aggregation type - grand total</p></figcaption></figure>

Note that for the same row, the sub-totals for each quarter are also aggregated in the same way to display the maximum value.

<figure><img src="../../.gitbook/assets/image (646).png" alt=""><figcaption><p>'Maximum' aggregation type - sub totals</p></figcaption></figure>

## Column aggregation for repetitive categories

When you have the same category repeated across all levels of the hierarchy, Inforiver will detect repeating categories and allow you to apply the same aggregation method to all the levels in a single click.

Let us assume we want to change the aggregation method for the sub-category _Amarilla_ in the _Canada_ region. Click on the total cell and select **Aggregation.**

<figure><img src="../../.gitbook/assets/image (647).png" alt=""><figcaption><p>Aggregation for repetitive sub-category</p></figcaption></figure>

Let us now change it to 'Average'.&#x20;

<figure><img src="../../.gitbook/assets/image (650).png" alt=""><figcaption><p>Click 'Average (Children)'</p></figcaption></figure>

When you click the option 'Average (Children)', a pop-up is displayed to confirm whether you want to apply the same aggregation to all the _Amarilla_ rows in all the regions.

<figure><img src="../../.gitbook/assets/image (648).png" alt=""><figcaption><p>Confirm to change for all the rows</p></figcaption></figure>

Click **Yes** to update all _Amarilla_ rows with the 'Average' aggregation method.

<figure><img src="../../.gitbook/assets/image (649).png" alt=""><figcaption><p>Average aggregation applied to repeated categories/sub-categories</p></figcaption></figure>

This ensures that the same aggregation is applied to all the repetitive categories/sub-categories in one go.

{% hint style="info" %}
Click **No** in the above confirmation pop-up to apply the aggregation only to that specific row.
{% endhint %}

## Combining Row and Column Aggregations

Inforiver lets you seamlessly track the various aggregations applied to the rows and columns with the 'Manage Aggregation' dialog box.

In the example below, both row and column aggregations are set to 'Sum' for the _Canada_ region.

<figure><img src="../../.gitbook/assets/image (629).png" alt=""><figcaption><p>Both aggregations are 'Sum'</p></figcaption></figure>

Let us now set the column aggregation to 'Maximum' while retaining the row aggregation to 'Sum'. To do this, click the required cell and select **Aggregation -> Maximum.**

<figure><img src="../../.gitbook/assets/image (631).png" alt=""><figcaption></figcaption></figure>

The column total now has the maximum value of the four quarters.

<figure><img src="../../.gitbook/assets/image (632).png" alt=""><figcaption></figcaption></figure>

You can track the same and also edit them with the 'Manage Aggregation' dialog box as illustrated below:

<figure><img src="../../.gitbook/assets/image (633).png" alt=""><figcaption><p>Manage Aggregation dialog box</p></figcaption></figure>
