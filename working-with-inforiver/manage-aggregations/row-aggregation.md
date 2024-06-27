# Row aggregation

If your data is hierarchical, Inforiver offers the flexibility to apply row aggregations for all branches on a selected level of the hierarchy. You can set different aggregation methods for different levels simultaneously.

To apply a uniform aggregation method to a given level of the hierarchy, navigate to the **Hierarchy** tab in the Manage Aggregation dialog box. Notice that we can assign different aggregation methods for different levels of the hierarchy.

{% hint style="warning" %}
The aggregation type set in the Hierarchy tab will not be applied to formula measures or quick measures created in Inforiver.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (779) (1).png" alt=""><figcaption><p>Aggregation set for hierarchy levels</p></figcaption></figure>

The specified aggregation method is set for a specific level of the hierarchy.

<figure><img src="../../.gitbook/assets/image (198).png" alt=""><figcaption><p>Hierarchy-level aggregation</p></figcaption></figure>

### Other methods to set row aggregation

#### 1. Setting aggregation from manage columns

Another way to set row aggregation for measures is by clicking on **Manage Columns** and then the <img src="../../.gitbook/assets/image (1) (1) (3).png" alt="" data-size="line"> icon. This allows you to manage row aggregations for specific measures.

<figure><img src="../../.gitbook/assets/image (651).png" alt=""><figcaption><p>Settings in 'Manage Columns' dropdown</p></figcaption></figure>

A pop-up displays a list of measures under the **Display** section. You can change the aggregation type of multiple measures here.

<figure><img src="../../.gitbook/assets/Display (2).png" alt=""><figcaption><p>Manage columns pop-up</p></figcaption></figure>

Let's change the aggregation for '2020 Actuals' from 'Sum' to 'Maximum'. Select 'Maximum' aggregation from the dropdown.&#x20;

<figure><img src="../../.gitbook/assets/Change agg.png" alt=""><figcaption><p>Column aggregation</p></figcaption></figure>

In the image below, you can see that East -> 2020 Actuals shows 40.18 which is the maximum of Beverages and Water, whereas East -> 2020 Plan shows 45.03 which is the sum of the two categories. &#x20;

<figure><img src="../../.gitbook/assets/Sum &#x26; maximum aggregation.png" alt=""><figcaption><p>Sum &#x26; maximum aggregation</p></figcaption></figure>

{% hint style="info" %}
You cannot set aggregation for a simulation measure. In the below image, you can see that the aggregation field is disabled for the simulation column.
{% endhint %}

Note that the [row aggregation type](../4.-adding-business-logic-and-formulae/insert-manual-input-columns/insert-manual-input-columns.md#i-row-aggregation-type) for calculated columns and manual data input columns can also be defined here in the **Manage Columns** dialog box in addition to the **Insert formula** and **Data input** [side panels](../4.-adding-business-logic-and-formulae/insert-manual-input-columns/insert-manual-input-columns.md#id-3.-properties). &#x20;

<figure><img src="../../.gitbook/assets/For.png" alt=""><figcaption><p>Simulation column disabled</p></figcaption></figure>

#### 2. Setting aggregation from column gripper

To set aggregation for a specific measure, you can also click on that column's gripper and choose 'Aggregation' from the context menu as shown below. Click on the required aggregation type to apply it to that measure.

<figure><img src="../../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Set aggregation from the column gripper</p></figcaption></figure>

In the example below, the 'Forecast' measure has been aggregated to display the maximum value of the child rows using the aggregation method 'Maximum'.

<figure><img src="../../.gitbook/assets/image (628).png" alt=""><figcaption><p>'Maximum' aggregation method in 'Forecast'</p></figcaption></figure>

In the next section, we will learn how to manage column aggregations.
