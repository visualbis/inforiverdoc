# Enterprise features

As mentioned in [manual input columns](../insert-manual-input-columns.md), Inforiver Enterprise provides additional features compared to Inforiver Premium Matrix.

1. Data type - Person
2. Track changes at row level using the last updated at/by columns
3. List of values (LOV) from dimensions or other Power BI datasets

{% hint style="info" %}
You need to [sign in](../insert-manual-input-columns.md#1.-sign-in) to access the Enterprise features.
{% endhint %}

Let's take a detailed look.

## 1. Person

In the 'Data input' dropdown, you can now see an additional type called Person. Once a data input column is added in Inforiver Enterprise, two columns – Last updated at and last updated by get enabled. These are covered in [track changes at the row level](enterprise-features.md#2.-track-changes-at-row-level).

<figure><img src="../../../.gitbook/assets/4.4.4.2 Person.png" alt=""><figcaption><p>Data input column type - Person</p></figcaption></figure>

a) Click on 'Person'. The person column side panel is shown in the below image.&#x20;

You can choose to [insert as a visual measure or column](../insert-manual-input-columns.md#1.-insert-as). Entry can be enabled or disabled in the total/subtotal rows using the '[Allow entry on total/subtotal rows](dropdown.md#iii-entry-in-total-subtotal-rows)' checkbox. Input access can be configured using the '[Allow input](../insert-manual-input-columns.md#2.-allow-input)' option.&#x20;

Click 'Create'.

<figure><img src="../../../.gitbook/assets/4.4.4.4 Person.png" alt=""><figcaption><p>Person column properties</p></figcaption></figure>

b) The person column gets inserted. Double-click on any of the cells. You can see a list of the users within the organization. Select any of the users.

<figure><img src="../../../.gitbook/assets/4.4.4.5 Person.png" alt=""><figcaption><p>List of users</p></figcaption></figure>

c) Start typing a name or scroll to find the desired user. Click on the username.

<figure><img src="../../../.gitbook/assets/4.4.4.6 Person.png" alt=""><figcaption><p>Selecting a username</p></figcaption></figure>

d) You can also select multiple users if required.

<figure><img src="../../../.gitbook/assets/4.4.4.7 Person.png" alt=""><figcaption><p>Selecting multiple users</p></figcaption></figure>

e) Click 'Enter' to save the data. You can see the user's name displayed as shown below.

<figure><img src="../../../.gitbook/assets/4.4.4.8 Person.png" alt=""><figcaption><p>Person name captured</p></figcaption></figure>

## 2. Last updated at/by&#x20;

You can track changes at the row level using the two columns – 'Last updated at' and 'Last updated by' which capture metadata for changes in the data input columns.&#x20;

These are enabled once you add a data input column and can be found in the data input dropdown. Select/deselect to show/hide columns. They can also be enabled/disabled from the ‘Manage columns’ dropdown.

<figure><img src="../../../.gitbook/assets/4.4.4.1 Person.png" alt=""><figcaption><p>Last updated at/by columns</p></figcaption></figure>

## 3. List of values (LOV)

For the Single select and Multi-select columns, a list of values (LOV) can be created from your Power BI semantic models or other dimensions like Master Data reference fields. The options are dynamically updated as the source data changes.

Note: The video is from an older version, the interface and options have changed in the later versions.

{% embed url="https://lumel.wistia.com/medias/bppuqp940h" %}
List of values from Power BI datasets
{% endembed %}

Let's create a LOV from the dataset for a multi-select column. We'll create a multi-select field to assign a subregion.

**STEP 1:** In the multi-select column side panel, click on Semantic model to open the **Add options from semantic model** dialog box.

<figure><img src="../../../.gitbook/assets/image (712).png" alt=""><figcaption><p>Semantic model option</p></figcaption></figure>

**STEP 2:** Select the Power BI workspace from the 'Workspace' dropdown. You can also search for a specific workspace.

<figure><img src="../../../.gitbook/assets/image (713).png" alt=""><figcaption><p>Select the workspace</p></figcaption></figure>

**STEP 3:** Select the semantic model and the table from the respective dropdowns. Click Next.&#x20;

<div>

<figure><img src="../../../.gitbook/assets/image (710).png" alt=""><figcaption><p>Select the semantic model </p></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/2024-04-03_15h03_16.png" alt=""><figcaption><p>Select the table - Acme Region Master</p></figcaption></figure>

</div>

**STEP 4:** From the **Label Column** dropdown, you can choose the column from the table (selected in Step 3) which will be used to populate the multi-select options.&#x20;

You can associate the options with an ID by selecting the **ID Column**. For example, if the multi-select shows a list of product names, you can tag them to a product ID field (if available in the data model). The multi-select options will not be impacted even if the product name changes, as the Product ID field remains constant.

{% hint style="info" %}
If an ID field is not available in your dataset, use the Label Column as the ID column.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (715).png" alt=""><figcaption><p>Selecting the column to source the multi-select options</p></figcaption></figure>

You can assign regions from the multi-select dropdown after completing the steps discussed above.

<figure><img src="../../../.gitbook/assets/image (716).png" alt=""><figcaption><p>Multi-select dropdown sourced from the dataset</p></figcaption></figure>

#### Applying filters on dropdown options

There are many scenarios wherein the options in the dropdown need to change based on the row dimension category. For example, consider that we have regional data in our rows. We need to use a dropdown to assign a manager for each region. The person that we assign must also be tagged to that specific region i.e. the dropdown options for the Central region should only show the people under that region. We can use filters in such scenarios, let's see how.

**STEP 1:** Select the workspace, semantic model, and table as discussed in the earlier section.

**STEP 2:** You can fetch the data from another table by checking the **Join Table** checkbox. After ticking the checkbox, you will be able to specify the table to join with.

The base table used to populate rows and columns in the report is Retail - Orders. We need to fetch the person data from the Retail - People table. The Retail -Orders and Retail-People are connected by the Region field (foreign key).

<figure><img src="../../../.gitbook/assets/image (714).png" alt=""><figcaption><p>Joining Retail-Orders with Retail-People</p></figcaption></figure>

**STEP 3:** Let's assign the field to source the multi-select options - in this case, Retail - People.Person. Since the Retail - People table does not have a unique ID column for each person, let's use the Person field as the option and the ID.

<figure><img src="../../../.gitbook/assets/image (717).png" alt=""><figcaption><p>Soucing options from the Person in the dataset</p></figcaption></figure>

**STEP 4:** We need to filter the people based on the region they are assigned to. In the **Columns** dropdown**,** select the field based on which you need to filter the options. In this case, it is the Retail - People.Region which can be used to identify the people tagged to a region. Select the corresponding field from the visual from the **Visual Column** dropdown.

<figure><img src="../../../.gitbook/assets/image (718).png" alt=""><figcaption><p>Setting a filter for dropdown options</p></figcaption></figure>

The dropdown options for people data have been fetched from the Retail - People table. Notice how all the people are displayed in the options for the grand total row. For each region, only the person assigned to that region is displayed in the dropdown.

<figure><img src="../../../.gitbook/assets/Untitled Project (2).gif" alt=""><figcaption><p>Fetching options</p></figcaption></figure>

In the next section, we'll be covering [quick formulas](../quick-formula.md).
