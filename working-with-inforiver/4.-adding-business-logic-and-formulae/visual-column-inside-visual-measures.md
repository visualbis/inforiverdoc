# Visual column inside visual measures

We have covered the different types of manual input columns that can be inserted in the report in the previous sections. We have also learned the steps to [insert calculated columns](insert-calculated-columns.md), in the form of visual measures as well as visual columns.

In this page, we will look at a specific case where you can include a data input visual column to be referenced inside a visual measure formula.

Data fields like interest rates, discount rates, tax slabs, and foreign exchange rates might be common to all the column dimensions. Hence they would be created as visual columns and we might need to refer to them often in calculations. In such cases, you can reference those visual columns in visual measures using the **COLUMNS** prefix.

Let us consider the following example: a visual input column is included to specify a discount rate of 10%.

<figure><img src="../../.gitbook/assets/image (659).png" alt=""><figcaption><p>Visual Column - Discount%</p></figcaption></figure>

To calculate the new sale price, we can insert a formula measure.

<figure><img src="../../.gitbook/assets/image (660).png" alt=""><figcaption><p>Inserting formula measure</p></figcaption></figure>

In the formula, we need to refer to this visual column, **Discount**_**%**_ to calculate the discounted sale price. The visual column is referred to using the **COLUMNS** prefix identifier.

<figure><img src="../../.gitbook/assets/image (662).png" alt=""><figcaption><p>Visual column referred inside a visual measure</p></figcaption></figure>

Click **Create** and the result is shown below:

<figure><img src="../../.gitbook/assets/image (663).png" alt=""><figcaption><p>Discounted Price</p></figcaption></figure>

{% hint style="info" %}
In the current edition, visual measures can only refer to **data input** visual columns and not calculated visual columns (formula columns).&#x20;
{% endhint %}
