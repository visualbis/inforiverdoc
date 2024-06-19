# LOV from semantic models

For the Single select and Multi-select columns, a list of values (LOV) can be created from your Power BI semantic models or other dimensions like Master Data reference fields. The options are dynamically updated as the source data changes.

### 1. Creating a LOV from a semantic model

Let's create a LOV from the dataset for a multi-select column. We'll create a multi-select field to assign a subregion.

**STEP 1:** In the multi-select column side panel, click on Semantic model to open the **Add options from semantic model** dialog box.

<figure><img src="../../../../.gitbook/assets/image (712).png" alt=""><figcaption><p>Semantic model option</p></figcaption></figure>

**STEP 2:** Select the Power BI workspace from the 'Workspace' dropdown. You can also search for a specific workspace.

<figure><img src="../../../../.gitbook/assets/image (713).png" alt=""><figcaption><p>Select the workspace</p></figcaption></figure>

**STEP 3:** Select the semantic model and the table from the respective dropdowns. Click Next.&#x20;

<div>

<figure><img src="../../../../.gitbook/assets/image (710).png" alt=""><figcaption><p>Select the semantic model </p></figcaption></figure>

 

<figure><img src="../../../../.gitbook/assets/2024-04-03_15h03_16.png" alt=""><figcaption><p>Select the table - Acme Region Master</p></figcaption></figure>

</div>

**STEP 4:** From the **Label Column** dropdown, you can choose the column from the table (selected in Step 3) which will be used to populate the multi-select options.&#x20;

You can associate the options with an ID by selecting the **ID Column**. For example, if the multi-select shows a list of product names, you can tag them to a product ID field (if available in the data model). The multi-select options will not be impacted even if the product name changes, as the Product ID field remains constant.

{% hint style="info" %}
If an ID field is not available in your dataset, use the Label Column as the ID column.
{% endhint %}

<figure><img src="../../../../.gitbook/assets/image (715).png" alt=""><figcaption><p>Selecting the column to source the multi-select options</p></figcaption></figure>

You can assign regions from the multi-select dropdown after completing the steps discussed above.

<figure><img src="../../../../.gitbook/assets/image (716).png" alt=""><figcaption><p>Multi-select dropdown sourced from the dataset</p></figcaption></figure>

**STEP 5:** After configuring and creating the dropdown, to preview all the options sourced from the semantic model, click the <img src="../../../../.gitbook/assets/image (12).png" alt="" data-size="line">icon. If you need to change the configuration, click the <img src="../../../../.gitbook/assets/image (518).png" alt="" data-size="line">icon to open the semantic model configuration window.

<figure><img src="../../../../.gitbook/assets/image (11).png" alt=""><figcaption><p>Previewing options</p></figcaption></figure>

### 2. Using joins and filters

#### Joins

The base data in our visual may be from one table, but the options in the dropdown can be from a different table. The join option comes in handy in these scenarios. If you need to join your base table with another table to source dropdown options, you need to be mindful that a common column connects the two tables. In this case, the Retail-Orders and Retail-People tables are connected by Region.

<figure><img src="../../../../.gitbook/assets/image (3) (11).png" alt=""><figcaption><p>Joining tables</p></figcaption></figure>

#### Filters

There are many scenarios wherein the options in the dropdown need to change based on the row dimension category. For example, consider that we have regional data in our rows. We need to use a dropdown to assign a manager for each region. The person we assign must also be tagged to that specific region i.e. the dropdown options for the Central region should only show the people under that region. We can use filters in such scenarios.&#x20;

Let's look at a scenario where we need to use joins and filters. Please note that the filter and join features can be used independently as well.

**STEP 1:** Select the workspace, semantic model, and table as discussed in the earlier section.

**STEP 2:** You can fetch the data from another table by checking the **Join Table** checkbox. After ticking the checkbox, you will be able to specify the table to join with.

The base table used to populate rows and columns in the report is Retail - Orders. We need to fetch the person data from the Retail - People table. The Retail -Orders and Retail-People are connected by the Region field (foreign key).

<figure><img src="../../../../.gitbook/assets/image (714).png" alt=""><figcaption><p>Joining Retail-Orders with Retail-People</p></figcaption></figure>

**STEP 3:** Let's assign the field to source the multi-select options - in this case, Retail - People.Person. Since the Retail - People table does not have a unique ID column for each person, let's use the Person field as the option and the ID.

<figure><img src="../../../../.gitbook/assets/image (717).png" alt=""><figcaption><p>Soucing options from the Person in the dataset</p></figcaption></figure>

**STEP 4:** We need to filter the people based on the region they are assigned to. In the **Columns** dropdown**,** select the field based on which you need to filter the options. In this case, it is the Retail - People.Region which can be used to identify the people tagged to a region. Select the matching field from the visual from the **Visual Column** dropdown.

<figure><img src="../../../../.gitbook/assets/image (718).png" alt=""><figcaption><p>Setting a filter for dropdown options</p></figcaption></figure>

The dropdown options for people data have now been fetched from the Retail - People table. Notice how all the people are displayed in the options for the grand total row. For each region, only the person assigned to that region is shown in the dropdown.

<figure><img src="../../../../.gitbook/assets/Untitled Project (3).gif" alt=""><figcaption><p>Filtering options dynamically</p></figcaption></figure>

### 3. Refreshing data

The underlying data in the semantic model is likely to change - there may be new data added or updates to the existing data. Any updates to the underlying data should be reflected in the dropdown options too.&#x20;

* You can schedule an automatic refresh at a specific time on a daily/monthly basis.
* You can also run ad-hoc data refreshes to sync the dropdown options with the semantic model.

<figure><img src="../../../../.gitbook/assets/image (4) (1).png" alt=""><figcaption><p>Refresh dataset option</p></figcaption></figure>

#### Triggering ad-hoc refreshes

You need to check the **Require Semantic model Refresh** option to trigger manual refreshes. Click the <img src="../../../../.gitbook/assets/image (7) (1).png" alt="" data-size="line">icon in the Options section to trigger a refresh from within the Inforiver visual.

<figure><img src="../../../../.gitbook/assets/image (6) (1).png" alt=""><figcaption><p>Manual refreshes</p></figcaption></figure>

Inforiver also provides an **API endpoint** to manually sync the semantic  model from outside the visual. The API endpoint is provided in the Refresh Link section. [Learn more about working with API endpoints and authorization tokens.](../../../../admin-console/settings/api-token.md)

<figure><img src="../../../../.gitbook/assets/image (8).png" alt=""><figcaption><p>API refresh option</p></figcaption></figure>

Click on the <img src="../../../../.gitbook/assets/image (9).png" alt="" data-size="line">icon to view the semantic model refresh history. Any errors that occur during the refresh can be viewed from this screen.

<figure><img src="../../../../.gitbook/assets/image (10).png" alt=""><figcaption><p>Refresh history portal</p></figcaption></figure>
