# Context awareness

Inforiver provides built-in context awareness i.e., any comments, notes, data input, or even headers that you add will be updated dynamically based on external filter or slicer selection. You can even select writeback payload with Power BI filters.&#x20;

When users enter comments or manually input data, the visual is unaware of the context, which can be set by a filter or a slicer in the report. In the example, notice how the comment entered for 'APAC' is still visible even after changing the filter to 'EMEA'.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Context unaware</p></figcaption></figure>

With Inforiver, you can configure filter context, which ensures that Inforiver visuals are aware of context changes and responsive to changes in filters i.e. the comments, data input, writeback payload, etc are dynamically updated. Let's look at how to set up filter context.

**Step 1**: Click on the **Filter Context** button in the Insert ribbon.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Filter context navigation</p></figcaption></figure>

**Step 2**: In the popup window, enter the table and field name for which context awareness is being set up. You can enter multiple tables and categories using the Add new link. In this case, we are setting up filter context for Subregions.

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Add table and category</p></figcaption></figure>

**Step 3**: Inforiver automatically generates the DAX code based on the tables and categories entered. Click on the Generate Dax button and copy the DAX.

<figure><img src="../.gitbook/assets/image (4) (1) (1) (1) (1).png" alt=""><figcaption><p>Generate DAX</p></figcaption></figure>

**Step 4**: Create a new measure in your data model using the DAX generated in Step 3.

<figure><img src="../.gitbook/assets/image (5) (1) (1) (1) (1).png" alt=""><figcaption><p>Create new measure</p></figcaption></figure>

**Step 5**: Add the new measure to the Others (OM) visual parameter. It gets displayed in the report as well.

<figure><img src="../.gitbook/assets/image (6) (1) (1) (1) (1).png" alt=""><figcaption><p>Add measure to others parameter</p></figcaption></figure>

**Step 6**: Open the filter context configuration from the insert ribbon. You will now be able to select the new FILTERCONTEXT measure from the dropdown. You can enable/disable context awareness for notes and comments using the toggle switches. Click on save.

<figure><img src="../.gitbook/assets/image (7) (1) (1) (1).png" alt=""><figcaption><p>Filter context configuration</p></figcaption></figure>

Let's see the context awareness feature in action by adding a notes column and setting a filter on APAC subregions.

<figure><img src="../.gitbook/assets/image (8) (1) (1) (1).png" alt=""><figcaption><p>Add notes</p></figcaption></figure>

Notice how the note is removed when we change the filter from APAC to EMEA.

<figure><img src="../.gitbook/assets/image (9) (1) (1).png" alt=""><figcaption><p>Filter context in action</p></figcaption></figure>



### 1. Context awareness in report headers

Slicer selections will be reflected in header presets as well, if your report has been configured for filter context.

<figure><img src="../.gitbook/assets/7.1. Filter context header preset.png" alt=""><figcaption><p>Filter context for header presets</p></figcaption></figure>

### 2. Context awareness in writeback

The filter selections are captured in the writeback table as separate columns. In the example below, the Segment and Region selections are captured as part of the writeback.

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption><p>Writeback for Home Office + West selection</p></figcaption></figure>

When the Segment and Region selection is changed to Corporate + Central, the notes and comments are inserted as separate rows in the snowflake destination and tagged against the changed categories.

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Writeback for Corporate + Central selection</p></figcaption></figure>
