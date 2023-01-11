# Insert manual input rows

Quite often we would like to insert a row in our table/matrix reports in Power BI and enter our own data. For example, a financial statement report connecting to a database query may be able to fetch revenue & expense metrics. But it might not retrieve the number of shares outstanding. Similarly, a sales report can leave out the sales data for a newly launched product category.

To address such scenarios, Inforiver allows you to insert static rows in matrix-style reports where you can input or enter the data.

Let's take this example where we need to insert a new subcategory 'Specialty beverages'. The option to insert rows is available in the 'Insert' tab. Note however that the 'Insert row' option is greyed out.

<figure><img src="../../.gitbook/assets/4.3.1 Static rows (1).png" alt=""><figcaption><p>Adding a new subcategory</p></figcaption></figure>

Select a row as shown below. The 'Insert row' option gets enabled. Click on the dropdown as shown. You can see a list of the available options. Click on 'Static row'.&#x20;

<figure><img src="../../.gitbook/assets/4.3.2 Static rows.png" alt=""><figcaption><p>Insert static row</p></figcaption></figure>

A side panel opens as shown. Type in the name of the category and click 'Apply'. You will see an empty record created right beneath 'Tea and Coffee', the row that was originally selected prior to the 'Insert Row' operation.&#x20;

Note that we have left the '**Include in total**' enabled. This ensures that any values that we type in for 'Specialty beverages' also update the parent row 'Beverages'.&#x20;

The '**Distribute parent value to children**' option ensures that if a value is entered at a total level, it gets distributed to the levels below it.

<figure><img src="../../.gitbook/assets/4.3.3 Static rows.png" alt=""><figcaption><p>Static row side panel</p></figcaption></figure>

Double-click on a cell as shown in the image. A formula bar gets enabled below the toolbar. Type in a value and click 'Enter'. Note that Inforiver allows entry of scaled values (e.g. 45.3m instead of 45,300,000).

<figure><img src="../../.gitbook/assets/4.3.4 Static rows.png" alt=""><figcaption><p>Entering a value</p></figcaption></figure>

The value gets updated as highlighted in yellow. The totals and subtotals are also updated to include the value entered for speciality beverages.

<figure><img src="../../.gitbook/assets/4.3.5 Static rows.png" alt=""><figcaption><p>Totals and subtotals get updated</p></figcaption></figure>

Let's now enter a value at the total level. Double-click on the 2021 Actuals grand total, type in the value and click 'Enter'.

<figure><img src="../../.gitbook/assets/4.3.6 Static rows.png" alt=""><figcaption><p>Entering value at grand total level</p></figcaption></figure>

As shown in the below image, the 250m gets distributed equally to International and United States. The category totals and the row grand total are also updated.

<figure><img src="../../.gitbook/assets/4.3.7 Static rows.png" alt=""><figcaption><p>Value distributed to the child levels</p></figcaption></figure>

In the next section, we'll be looking at [inserting manual input columns](insert-manual-input-columns.md).
