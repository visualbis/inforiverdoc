# Add data

The first step to using Inforiver is to add it to the Power BI canvas. You can drag it over from the visualization pane. Then, for this tutorial, resize it to fill the entire screen. There are other times when you will use it as one of many visuals.

Similar to using a pivot table, to use the visual we need to specify 3 things:

* Rows
* Columns (optional) and
* Values

If you’ve used pivot tables before, this experience should feel familiar. If you have experience with Power BI, then this process is identical to any other Power BI visual, especially a table or matrix visual.

Here we’ve dragged the Level 4 description to the rows field well, and the Actuals measure to the Values (AC) well. “AC” is the [IBCS](https://www.ibcs.com/) notation for “Actuals”. We have left the columns field well empty because we don’t need a matrix view for a P\&L statement.

We can see that while this produces a nicely formatted table, it doesn’t show all the information we want. Many accounting reports show a nested hierarchy of data, and a P\&L statement is no different. To make the most of Inforiver, we need to provide it with a structure to organize the data.

### Creating a Power BI hierarchy

When working with Power BI, there are two ways to create a hierarchy of your descriptive fields. One option is to drag and drop the different fields into the rows well, like how you would do it with a pivot table.

Alternatively, you can use use the Power BI hierarchies feature to create a combined group of fields. This can be useful when you have a nested set of fields you want to use repeatedly. Right-click on your top-level field (Level 0 Description) in the fields pane and click **Create Hierarchy**.

Next, rename the new hierarchy to the name “Accounts”. Then right-click on the next level of detail (Level 1 Description) and select **Add to Hierarchy**.

Repeat this for the rest of the levels. Now you will have an accounts hierarchy that you can drag and drop, instead of manually adding each level of detail.

### Filling out the visual

Once you have the hierarchy, the next step is to fill in the values of the report. Drag the accounts hierarchy to the Rows field well and the actuals field to the values field well. At this point, your report should look like this.

While the default settings are readable, we want to make a few formatting changes to better suit the type of report we are creating.
