# Data Settings

Under the data settings, you can view a list of all the series configurations. Here you can select the series that should be included in the writeback.

#### i) Series allowed for writeback

This section will list all the possible series that are allowed for writeback. All the series are selected by default. You can select/unselect the series you want to write back to the destination.

<figure><img src="../../../.gitbook/assets/series-wb.png" alt=""><figcaption></figcaption></figure>

#### ii) Auto writeback for database destination

If you enable auto writeback, the chosen series and scenario(s) will be written back automatically without having to initiate the writeback operation manually. Writeback will be triggered periodically after specified intervals.

This option can be enabled only after configuring a destination.

{% hint style="info" %}
Auto-writeback can be enabled only if you make adjustments to data input fields or simulations, not native values.
{% endhint %}

<figure><img src="../../../.gitbook/assets/auto-wb (1).png" alt=""><figcaption></figcaption></figure>

#### iii) Scenarios to be included for auto writeback

This option will be displayed only if you have created a scenario. You can read more on how to create a scenario [here](../../7.-planning-budgeting-and-forecasting/scenarios-enterprise-only.md).

<figure><img src="../../../.gitbook/assets/scenario-wb.png" alt=""><figcaption></figcaption></figure>

In this section, you will find a list of all the created scenarios. You can select the scenario(s) you want to write back. Please note, if you do not have any scenarios and auto writeback is enabled, only the data input columns will be auto-written back when changes are made to the base table. Native columns will not be auto-written back even when modified.

#### iv) Advanced settings

You can set the time interval between consecutive auto-writebacks in the Advanced section. The default delay is set to 5 seconds. This time interval can be decreased, with a value of 0 resulting in the immediate triggering of writebacks.

{% hint style="info" %}
The time interval between auto-writebacks can be set for non-numeric data only.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (276).png" alt=""><figcaption><p>Auto write back debounce time</p></figcaption></figure>
