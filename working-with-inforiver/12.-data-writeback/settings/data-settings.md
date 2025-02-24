# Data Settings

Under the data settings, you can view a list of all the series configurations. Here you can select the series that should be included in the writeback.

#### 1. Series allowed for writeback

This section will list all the possible series that are allowed for writeback. All the series are selected by default. You can select/unselect the series you want to write back to the destination.

<figure><img src="../../../.gitbook/assets/series-wb.png" alt=""><figcaption></figcaption></figure>

#### 2. Dimensions to be removed from writeback

Inforiver provides a [Row Dimension ID Mapping](../../4.-adding-business-logic-and-formulae/manage-inserted-rows-and-columns.md#b-row-id-mapping) feature that enables you to choose the dimensions to uniquely identify a row. For instance, you can identify a product using just the product ID instead of the product name.

<figure><img src="../../../.gitbook/assets/3.3. Writeback exclude dimension row dimension ID mapping.png" alt=""><figcaption><p>Row dimension ID mapping</p></figcaption></figure>

Since the Row Dimension ID Mapping is set up based on the Product ID, the Product Name is redundant and can be dropped from writeback. You can use the dropdown to select the dimensions to be removed.

<figure><img src="../../../.gitbook/assets/3.4. Writeback exclude dimension.png" alt=""><figcaption><p>Removing the product ID dimension from writeback</p></figcaption></figure>

The product name field is not written back. You can distinctly locate a row using the product ID field.

<figure><img src="../../../.gitbook/assets/3.5. Writeback exclude dimension target data.png" alt=""><figcaption><p>Data in the snowflake destination</p></figcaption></figure>

#### 3. Auto writeback for database destination

If you enable auto writeback, the chosen series and scenario(s) will be written back automatically without having to initiate the writeback operation manually. Writeback will be triggered periodically after specified intervals.

This option can be enabled only after configuring a destination.

{% hint style="info" %}
* Auto-writeback will be triggered only if you make adjustments to data input fields or simulations, not native values.
{% endhint %}

<figure><img src="../../../.gitbook/assets/auto-wb (1).png" alt=""><figcaption><p>Auto writeback</p></figcaption></figure>

Auto-writeback can also capture changes to dependent measures. For instance, consider that you have a data input field whose values are used to drive a formula field. In this report, we’ve derived the Rate based on the Benchmark, a data input text column.

<figure><img src="../../../.gitbook/assets/image (672).png" alt=""><figcaption><p>Dependant forumla measure</p></figcaption></figure>

The benchmark for the Furniture row was updated from LIBOR’ to ‘EURIBOR’ and captured during auto-writeback. Notice how the change in rate was also automatically written back.

Initial value of LIBOR with the corresponding rate written back to the destination:

<figure><img src="../../../.gitbook/assets/image (673).png" alt=""><figcaption><p>Initial writeback</p></figcaption></figure>

Updated benchmark value of EURIBOR with the dependent rate auto-written back to the destination:

<figure><img src="../../../.gitbook/assets/image (675).png" alt=""><figcaption><p>Autowriteback triggered when the benchmark was updated </p></figcaption></figure>

#### 3. Scenarios to be included for auto writeback

This option will be displayed only if you have created a scenario. You can read more on how to create a scenario [here](../../7.-planning-budgeting-and-forecasting/scenarios-writeback-matrix-only.md).

<figure><img src="../../../.gitbook/assets/scenario-wb.png" alt=""><figcaption></figcaption></figure>

In this section, you will find a list of all the created scenarios. You can select the scenario(s) you want to write back. Please note, if you do not have any scenarios and auto writeback is enabled, only the data input columns will be auto-written back when changes are made to the base table. Native columns will not be auto-written back even when modified.

#### 4. Advanced settings

You can set the time interval between consecutive auto-writebacks in the Advanced section. The default delay is set to 5 seconds. This time interval can be decreased, with a value of 0 resulting in the immediate triggering of writebacks.

{% hint style="info" %}
The time interval between auto-writebacks can be set for non-numeric data only.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (276).png" alt=""><figcaption><p>Auto write back debounce time</p></figcaption></figure>
