# Insert manual input rows

Quite often we would like to insert a row in our table/matrix reports in Power BI and enter our own data. For example, a financial statement report connecting to a database query may be able to fetch revenue & expense metrics, but it might not retrieve the number of shares outstanding. Similarly, a sales report can leave out the sales data for a newly launched product category.

To address such scenarios, Inforiver allows you to insert static rows in matrix-style reports where you can input or enter the data.

{% embed url="https://lumel.wistia.com/medias/n67puv7p0m" %}



## 1. Insert static row

The option to insert rows is available in the 'Insert' tab. Note however that the 'Insert row' option is greyed out.

<figure><img src="../../.gitbook/assets/image (306).png" alt=""><figcaption></figcaption></figure>

Select a row as shown below. The 'Insert row' option gets enabled. Click on the dropdown as shown. You can see a list of the available options. Click on 'Static row'.&#x20;

<figure><img src="../../.gitbook/assets/image (307).png" alt=""><figcaption></figcaption></figure>

Another way to insert static rows is by using the row gripper. The gripper icon is highlighted when you hover over a row. Click on it, then select the 'Add static row' option in the _insert_ section.

<figure><img src="../../.gitbook/assets/image (308).png" alt=""><figcaption></figcaption></figure>

## 2. Static row properties

A side panel opens when creating a static now, as shown below. Type in the name of the category and click 'Create'. You will see an empty record created above the row that was selected before the 'Insert Row' operation.&#x20;

<figure><img src="../../.gitbook/assets/image (318).png" alt=""><figcaption></figcaption></figure>

### **i. Scaling factor**

You can set the scaling factor for the static row depending on the data that is expected to be entered. It is set to Auto by default.

### **ii. Include in total**

When the 'Include in total' option is enabled, any values that we type in for the new row also update the parent row 'Germany'.&#x20;

### **iii. Distribute parent value to children**

The 'Distribute parent value to children' option ensures that if a value is entered at a total level, it gets distributed to the levels below it.

### **iv. Bind for cross filter/RLS**

You can enable the Bind for Cross filter/RLS option – this ensures that cross-filter selections and RLS settings apply to calculated/manual input rows that reference other rows. For example, if this option is not enabled, a manager handling Canada accounts can view a manually inserted row that references US data or an inserted region that is manually created at the visual level. [Learn more about binding rows.](insert-calculated-rows/#id-6.-bind-for-cross-filter-rls)

## 3. **Delete a static row**

To delete a static row, hover over the row and click on the row gripper. Select the 'Delete Row' option.

<figure><img src="../../.gitbook/assets/image (309).png" alt=""><figcaption></figcaption></figure>

## 4. Bulk insert static rows

### i) Multiple static row

a) You can leverage the **Multiple Static Row** option to bulk insert multiple category rows in a single stroke. The inserted rows can be used for manual data entry for categories that may not be available in your datasets.

<figure><img src="../../.gitbook/assets/image (311).png" alt=""><figcaption></figcaption></figure>

b) You can also create placeholders for hierarchical data that is not available in your datasets with this option. Click on the parent level above which you want to insert additional levels. Use tab space to indent the child rows according to the structure of the hierarchy.

<figure><img src="../../.gitbook/assets/image (312).png" alt=""><figcaption><p>Multiple static rows - hierarchical data</p></figcaption></figure>

Notice how the custom hierarchy levels for 'Malaysia' and 'Hong Kong' have been created and the corresponding rows have also been inserted.

<figure><img src="../../.gitbook/assets/image (313).png" alt=""><figcaption></figcaption></figure>

### ii) Row hierarchy

This option can be used to insert a single user-defined level for hierarchical data. Only one row is created while using this option, unlike the [multiple static row](insert-manual-input-rows.md#i-multiple-static-row) option, where you can define the hierarchy structure with multiple nested levels and rows. &#x20;

<figure><img src="../../.gitbook/assets/image (314).png" alt=""><figcaption><p>Row hierarchy</p></figcaption></figure>

After creating a custom hierarchy level, you can insert static rows, calculated rows, aggregated rows, etc as demonstrated in the example below.&#x20;

<figure><img src="../../.gitbook/assets/image (316).png" alt=""><figcaption></figcaption></figure>

In the next section, we'll be looking at [inserting manual input columns](insert-manual-input-columns.md).

#### Resources

[Insert row and manually enter data in Power BI matrix reports](https://inforiver.com/blog/feature-highlights/insert-row-manual-data-entry-powerbi/)
