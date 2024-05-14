# Recommended practices while working with Power BI desktop

This section outlines the best practices to be followed while editing Inforiver visuals from Power BI desktop as well as from the Power BI service.&#x20;

In the previous section, we discussed [visual IDs and shared elements](safe-procedures-for-copying-writeback-matrix-visuals.md#visual-ids) in Inforiver that get synced between visuals. After you develop a report in Power BI desktop, when you subsequently publish it to the Power BI service; the desktop and the web versions will share the same Inforiver visual ID. If you directly make changes to the web version of the report after publishing it, you will need to be mindful of certain considerations:

* Any changes made from the Power BI service to **non-shared** elements like formulas will not be synced with the desktop version of the report.&#x20;
* Any changes made to **shared** elements, like comments or writeback configurations, will be synced across the desktop as well as the web versions of the report.

If a published report requires modifications, the conventional approach would be to first make changes to the desktop version and then re-publish the report. However, if changes are directly made to the web version, to ensure that the changes are smoothly integrated, you will need to follow the procedure to create a baseline.

{% hint style="warning" %}
If a baseline of the published report is not taken, certain changes made in the service will be overwritten if the desktop version is re-published.
{% endhint %}

### Creating a baseline from Power BI service

1. Take an [export of the report](https://learn.microsoft.com/en-us/power-bi/create-reports/service-export-to-pbix) from the Power BI service - this is the baseline version.
2. Import the .pbix file into Power BI desktop.
3. Use the baseline to make further changes from Power BI desktop.
4. Repeat the steps if changes are made directly in the Power BI service and the report goes out of sync with the desktop version.

Baselines need not be taken if changes are only made on Power BI desktop.
