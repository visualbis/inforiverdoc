# Duplicating Writeback Matrix Visuals - Best Practices

When working on a specific Inforiver visual, you might sometimes receive the following notification, warning you about a duplicate visual.

<figure><img src="../../.gitbook/assets/image (9) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Duplicate visual detected</p></figcaption></figure>

In this section, we will define duplicate visuals, discuss their causes, how to avoid them, and how to detach visuals in the event of intentional or accidental duplications.

Let us first begin with understanding visual IDs.

## Visual IDs

When you load an Inforiver visual from scratch on your desktop, it will be assigned a unique **Visual ID.** This can be seen and accessed from your user profile.

<figure><img src="../../.gitbook/assets/image (940).png" alt=""><figcaption><p>Visual ID</p></figcaption></figure>

When you save this .pbix file with a name, say, _Inforiver Datasets\_new.pbix_ and publish it to the service, this visual will retain the same Visual ID as the desktop version, as shown in the image below. Let's refer to it as _VISUAL\_ID1_.&#x20;

<figure><img src="../../.gitbook/assets/image (941).png" alt=""><figcaption><p>same Visual ID in PBI desktop and PBI service</p></figcaption></figure>

The visual ID is significant because all your input budget numbers, text, dropdowns and checkboxes, Inforiver input fields' data such as comments, snapshots, scenarios, forecasts, simulations, and other Inforiver visual metadata are stored in the backend cache with _VISUAL\_ID1_ tagged as the identifier.

If someone changes a budget number on a visual in service, you will see the same changes on the desktop report too. This is because the visuals on the desktop and the service, both have the same _VISUAL\_ID1_ as their ID which points to the same cache memory space, containing all the input data and visual metadata.

## Duplicate visuals

Report developers may often need to replicate the structure and design across multiple visuals. So they might duplicate the visuals to achieve this.

## Common ways of duplicating visuals

A visual is said to be duplicated in the following cases:

1. Publishing the same report to different workspaces in the Power BI service.

When you publish the same report to different workspaces, they share the same visual ID.

<figure><img src="../../.gitbook/assets/image (942).png" alt=""><figcaption><p>publishing the same report to different workspaces</p></figcaption></figure>

2. Saving the report with a different file name and then publishing it. For example, saving the _Inforiver Datasets\_new_.pbix file with a new name, such as _Inforiver Datasets\_new\_V2_.pbix, and then publishing it to the service, results in the same visual ID for both the visuals.&#x20;

<figure><img src="../../.gitbook/assets/image (944).png" alt=""><figcaption><p>Saving and publishing with a new name</p></figcaption></figure>

**Note that, each page in a Power BI report has a unique URL, which is a composite key of Report Name + Report Page.**

Since these two reports have the same visual IDs, their corresponding page URLs will be the same (Page 1 -> Page 1, Page 2 -> Page 2, and so on), and Inforiver flags this as a duplicate visual despite changing the .pbix file name.

<figure><img src="../../.gitbook/assets/image (945).png" alt=""><figcaption><p>Duplicate visual due to duplicated report</p></figcaption></figure>

3. Duplicating a page/tab in a report and republishing it in place of the old one: Since each page/tab in a report has a unique URL ID, when you duplicate a page or a tab within a report, these pages share the same visual IDs.

<figure><img src="../../.gitbook/assets/image (946).png" alt=""><figcaption><p>Duplicate page</p></figcaption></figure>

So, if you delete the old page/tab in your desktop and republish with the duplicated page/tab, Inforiver will flag this as duplicate.&#x20;

<figure><img src="../../.gitbook/assets/image (947).png" alt=""><figcaption><p>Duplicate visual due to duplicated page</p></figcaption></figure>

{% hint style="info" %}
Since duplicate detection works based on **Power BI report URLs**, it is obvious that Inforiver can detect duplication only on Power BI service.
{% endhint %}

## What happens with duplicate visuals?

As previously stated, when a specific visual is copied, the new visual retains the same visual ID as the old one. As a result, items such as forecasts, scenarios, comments, and other metadata from both new and old visuals share the same backend cache.

Any changes made to these items will affect both the original and the copied visuals simultaneously. These include,

-> Input fields-related data such as Comments, Snapshots, Scenarios

-> Forecasts

-> Simulations

-> Data Input fields such as dropdowns, checkboxes, and text/numeric input - both, the structure, and values

-> Inserted rows such as static rows, calculated rows and row hierarchies

-> Writeback destinations and configurations

All the above will be synced between the visuals.

**If this is not the intended use case or behavior (as is usually the case), it is ideal to detach the visuals to remove the dependencies between them. The steps to detach the visuals, after accidental duplication, are explained** [**here**](duplicating-writeback-matrix-visuals-best-practices.md#detaching-visuals)**.**

_Note: Other elements such as Formulas, Variance columns, Formatting changes, Show/Hide columns, etc. are not synced between duplicate visuals._

## How do we avoid duplicate visuals?

To prevent multiple visuals from being impacted at the same time, due to duplication, follow these best practices when copying reports or pages in Power BI:\
\
1\. When you download a visual from the Power BI service to your desktop and make changes, save the file with the same name it was downloaded with, instead of using a different name.\
\
2\. When publishing it, replace the old report with the new one. Click "Replace" when prompted by Power BI (the prompt appears because they have the same name).\
\
3\. Avoid duplicating reports or pages, as the visual IDs will also be duplicated. Instead, create new reports or pages.\
\
4\. If duplication is required to retain existing data or structure, follow these steps to detach the visuals and choose the option of retaining the data.

## Detaching visuals

Follow the steps outlined to detach visuals.

1. [Publish the report](https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-upload-desktop-files) to the Power BI service. Open the report in edit mode in the Power BI service, after the report has been published. A yellow warning symbol near the profile indicates that the visual is a duplicate.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Duplicate report warning</p></figcaption></figure>

2. Expand the Profile menu and navigate to **Report Details**.

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

3. Click on the **Create** button in the Report Details side pane to detach the visual.

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

4. Choose whether to retain existing data or enter new values for data input fields.

* To copy data input values to the new visual select the _**Yes, I do**_ option
* To enter new values, select _**No, I will start with blank cell values**_

Select the confirmation checkbox and click on **Proceed** to confirm that the visual can be detached.

<figure><img src="../../.gitbook/assets/image (413).png" alt=""><figcaption></figcaption></figure>

5. The warning symbol will be removed after the visual is saved.

{% hint style="info" %}
When a visual is detached, the duplicate warning symbol is removed. There will not be any other explicit changes to indicate that the visual has been detached from the original. Internally, the new visual is assigned to a separate visual ID. Any changes made in the new report will no longer affect elements from the original report.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (7) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Detached visual</p></figcaption></figure>

## When to detach visuals

* **Detach** visuals when the reports are mutually exclusive i.e., only the report structure needs to be identical but there are no data-level dependencies.
* **Don't detach** visuals if you need to share data between reports or create a report that sources its data from an underlying report. E.g., you may have data input fields in a base report. You may apply formulas or conditional formatting in a second report, which consumes the data from the data input fields of the first report. In such cases, when both the data and structure need to be synced across reports, do not detach the visual.

