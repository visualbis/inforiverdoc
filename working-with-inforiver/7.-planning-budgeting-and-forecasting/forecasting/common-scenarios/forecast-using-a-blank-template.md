# Forecast using a Blank Template

A common requirement for organizations is to forecast using a blank template in Power BI, just as we would do with Microsoft Excel. Data may be entered by a single individual, or by many individuals across the organization.&#x20;

Let us explore how we can set this up quickly in Power BI using Inforiver.&#x20;

In our case, ACME Inc. wants to create sales forecasts for all four quarters of the year 2024 for each geography. These are the steps involved.&#x20;

1. Launch Inforiver Matrix visual.&#x20;

<figure><img src="../../../../.gitbook/assets/launch-inforiver-matrix-visual.png" alt=""><figcaption><p>Launch Inforiver</p></figcaption></figure>

2. Assign _Region_ & _Sub Region_ categories to rows and _Quarters_ to columns. You will have a blank table structure.

<figure><img src="../../../../.gitbook/assets/create-blank-table-structure.png" alt=""><figcaption><p>Creating a blank report</p></figcaption></figure>

3. We will now create a data input field (a forecast measure) so that users can type in their values. To do this, click on **Insert -> Data Input -> Number** (since it is a numeric field type) **-> Insert a new empty series.**&#x20;

<figure><img src="../../../../.gitbook/assets/create-a-data-input-field.png" alt=""><figcaption><p>Create Data Input fields</p></figcaption></figure>

4. Name the column _2024 Forecast_ and click on **Create**.&#x20;

<figure><img src="../../../../.gitbook/assets/name-forecast-column.png" alt=""><figcaption><p>Name the forecast columns</p></figcaption></figure>

5. You will get a blank template with four columns. You can also add additional fields of other types (text, multi-select, date, etc.) using the same Data Input menu shown earlier.

<figure><img src="../../../../.gitbook/assets/add-fields-with-data-input-menu.png" alt=""><figcaption><p>Blank Template with 4 forecast columns</p></figcaption></figure>

6. Let us go ahead & add these fields:

* a 'Person' column for inputting users' names from the organization. The list of names comes from the Office365 directory.
* a 'Status' text drop-down field, and
* a 'Remark' column for entering multi-line comments.&#x20;

<figure><img src="../../../../.gitbook/assets/remark-column-for-entering-comments.png" alt=""><figcaption><p>Add other fields</p></figcaption></figure>

7. Let us start entering our forecasts now. Double-click the value for _Q1_ for the _APAC_ region. A formula bar appears above the table. Type in ‘10m’ in the formula bar.

<figure><img src="../../../../.gitbook/assets/start-entering-forecasts-value-now.png" alt=""><figcaption><p>Enter forecast values</p></figcaption></figure>

8. Press Enter, and the _APAC_ values automatically roll up to the _International_ region and _All_ (company-level total). This makes hierarchical budgeting easier without having to write formulas at each parent level.

<figure><img src="../../../../.gitbook/assets/auto-roll-up-without writing formula-at-each-level.png" alt=""><figcaption><p>Automatic roll-up to the top levels</p></figcaption></figure>

9. Similarly, you can go ahead by filling out values for the other granular regions. Assign the people & status fields to each row.

<figure><img src="../../../../.gitbook/assets/final-sales-forecast-with-blank-template-using-power-bi.png" alt=""><figcaption><p>Assign people and status</p></figcaption></figure>

Just like we entered the values, other users in the organization also can enter the values for their respective regions.&#x20;

This is how a sales forecast can be done using Inforiver with a blank template in Power BI.

&#x20;
