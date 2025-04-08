# Inforiver Writeback Matrix April 2025 - v4.4.

### Match date periods in Infobridge

Infobridge supports forecasts and allows you to capture projections or data for future time periods. Your target reports, however, may not require future data. We've added a new **Show All Periods from Infobridge** option in the Manage Measures side pane:&#x20;

* When the toggle is enabled, all the time periods available in the bridge will be imported into the target report.
* When disabled, only the time periods in the bridge that exist in the target report will be imported.

{% hint style="info" %}
This option will be enabled only after creating an integration to a bridge
{% endhint %}

<figure><img src="../.gitbook/assets/image (1366).png" alt=""><figcaption><p><strong>Show All Periods from Infobridge option</strong></p></figcaption></figure>

In the bridge, we have the allocated budgets for 2023 and 2024 as well as the projected budgets for 2025.

<figure><img src="../.gitbook/assets/image (1367).png" alt=""><figcaption><p>Projected and allocated budgets in the bridge</p></figcaption></figure>

The target report contains the profits for 2023 and 2024. We need to integrate the budgets for 2023 and 2024 with this report. The projected budgets for 2025 are not required in this case.

<figure><img src="../.gitbook/assets/image (1368).png" alt=""><figcaption><p>Target report </p></figcaption></figure>

Since we've disabled the **Show All Periods from Infobridge** toggl&#x65;**,** when we insert the budget from the bridge, the budget will be inserted only for the time periods which exist in the target report.

<figure><img src="../.gitbook/assets/image (1369).png" alt=""><figcaption><p>Inserting budgets for existing time periods</p></figcaption></figure>

