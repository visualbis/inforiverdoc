# Safe procedures for copying enterprise visuals

Report developers may often need to replicate the structure and design across multiple visuals. The fastest way to achieve this is by duplicating the visual itself. A visual can be duplicated by:

* duplicating the page.
* duplicating the report.
* publishing the same report to different workspaces from the Power BI desktop.

This section will explore the basic concepts and factors to be aware of while duplicating Inforiver visuals.

### Visual IDs

Every Inforiver visual is assigned to a specific visual ID. When a particular visual is duplicated, the new visual will also be tagged with the same visual ID as the original. Elements like forecasts, scenarios, and comments in the new visual will be a pointer to the original i.e., any changes made to these elements will be reflected in both the original and the copied visual.&#x20;

<figure><img src="../../.gitbook/assets/image (8) (1) (1).png" alt=""><figcaption><p>Visual ID</p></figcaption></figure>

Inforiver elements that are shared between visuals include:

\-> All Enterprise data such as Comments, Snapshots, Scenarios

\-> Forecasts

\-> Simulations

\-> Data Input fields such as dropdowns, checkboxes, and text/numeric input - both, the structure, and values will be synced

\-> Writeback destinations and configurations

Other elements such as Formulas, Variance columns, Formatting changes, Show/Hide columns, etc are not synced between duplicate visuals. To remove the dependencies between duplicated visuals, follow the steps outlined to detach visuals.

Inforiver generates a **notification** when a duplicate visual is detected.

<figure><img src="../../.gitbook/assets/image (9) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Detaching visuals

1. [Publish the report](https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-upload-desktop-files) to the Power BI service. Open the report in edit mode in the Power BI service, after the report has been published. A yellow warning symbol near the profile indicates that the visual is a duplicate.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1).png" alt=""><figcaption><p>Duplicate report warning</p></figcaption></figure>

2. Expand the Profile menu and navigate to **Report Details**.

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

3. Click on the **Create** button in the Report Details side pane to detach the visual.

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

4. Click on **Proceed** to confirm that the visual can be detached.

<figure><img src="../../.gitbook/assets/image (6) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

5. The warning symbol will be removed after the visual is saved.

{% hint style="info" %}
When a visual is detached, the duplicate warning symbol is removed. There will not be any other explicit changes to indicate that the visual has been detached from the original. Internally, the new visual is assigned to a separate visual ID. Any changes made in the new report will no longer affect elements from the original report.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (7) (1) (1) (1).png" alt=""><figcaption><p>Detached visual</p></figcaption></figure>

### When to detach visuals

* **Detach** visuals when the reports are mutually exclusive i.e., only the report structure needs to be identical but there are no data-level dependencies.
* **Don't detach** visuals if you need to share data between reports or create a report that sources its data from an underlying report. E.g., you may have data input fields in a base report. You may apply formulas or conditional formatting in a second report, which consumes the data from the data input fields of the first report. In such cases, when both the data and structure need to be synced across reports, do not detach the visual.

