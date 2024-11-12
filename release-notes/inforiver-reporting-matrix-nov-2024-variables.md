# Inforiver Reporting Matrix Nov 2024: Variables,

Release notes for version v3.3

## 1.      Formatting

#### 1.1. Display skipped rows in the report

Inforiver allows you to exclude rows from total/subtotal calculations using the Skip row option. The skipped row will then be masked from the report. With the latest release, you can retain skipped rows in the report with the Skip and Show Row option in the row gripper. This feature allows you to cherry-pick the categories contributing to the subtotals and display the excluded categories.

Notice how the Bookcases row is still displayed in the report after skipping it. The subtotals for the Furniture and Central categories and the grand total have changed after excluding the Bookcases row.

<figure><img src="../.gitbook/assets/image (986).png" alt=""><figcaption><p>Skip and show row</p></figcaption></figure>

Select the **Include All Skipped Rows** option from the row gripper to include skipped rows again.&#x20;

#### **1.2. Date-based interface to show measures**&#x20;

Inforiver offers a range of time intelligence formulas to display your data for specific periods. If scripting is not your cup of tea, you can use the new **Show Measures** interface to display the data for a particular period of time. You only need to select the date range from the date picker.&#x20;

You can also hide measures for a specific time range by turning off the **Show** toggle.&#x20;

<figure><img src="../.gitbook/assets/image (987).png" alt=""><figcaption><p>Show measures setup</p></figcaption></figure>

Once defined, you can smoothly switch between different time ranges and analyze your data for specific periods.

<figure><img src="../.gitbook/assets/image (988).png" alt=""><figcaption><p>Defining multiple time periods and switching between them</p></figcaption></figure>

#### **1.3. Pie and donut – a new addition to row-level charts**&#x20;

Add a pie or donut chart to your report to visualize the proportions of different categories in your dataset. To embed pie charts, add a minimum of 2 measures.  &#x20;

<figure><img src="../.gitbook/assets/image (989).png" alt=""><figcaption><p>Embedding pie and donut charts</p></figcaption></figure>

#### **1.4. Minimum and maximum threshold for outliers**&#x20;

Inforiver can highlight outlier values for lollipop charts, and you can specify the threshold beyond which a data point will be considered an outlier. In earlier versions, we only had the option to specify a negative and positive outlier, but what if you only have positive values in your data? In the latest version, you can specify a minimum and maximum threshold or use the existing positive/negative option based on your data.&#x20;

<figure><img src="../.gitbook/assets/image (990).png" alt=""><figcaption><p>Outlier threshold</p></figcaption></figure>

#### **1.5. Display marker values for sparklines**

Inforiver enables you to visualize your numbers by embedding row-level charts. By checking the **Show Marker Label** option, you can now display markers alongside the charts, allowing you to grasp insights quickly from the charts.&#x20;

<figure><img src="../.gitbook/assets/image (991).png" alt=""><figcaption><p>Sparkline markers</p></figcaption></figure>

#### **1.6. Border box option**&#x20;

You can now create a box highlighting specific rows/columns or cells in your reports.&#x20;

<figure><img src="../.gitbook/assets/image (993).png" alt=""><figcaption><p>Border box</p></figcaption></figure>

If you have applied Power BI filters on row/column dimensions, the border box will automatically expand to accommodate the filtered categories when they are added back. &#x20;

Please remember that this will work only when you use the row/column gripper options to select data when you apply a border.&#x20;

<figure><img src="../.gitbook/assets/1.6.2. power-BI-filtered-border-box-expansion.gif" alt=""><figcaption><p>Power BI filter compatibility</p></figcaption></figure>

## 2. Analysis  <a href="#analysis" id="analysis"></a>

#### **2.1. Row groups in KPI explorer**&#x20;

With Inforiver, you can group rows and create visual-level hierarchies. In earlier releases, row groups could not be viewed or selected from the KPI explorer. From this release, row groups will be supported in the explorer view.&#x20;

<figure><img src="../.gitbook/assets/image (995).png" alt=""><figcaption><p>Row groups in KPI explorer</p></figcaption></figure>

#### **2.2. Date picker in filters**&#x20;

Inforiver makes it easier for you to apply filters for date fields. You can select the date ranges from the date picker, which is now available in the filter interface.&#x20;

Note: You need to have a date dimension in your report to enable the date picker.&#x20;

<figure><img src="../.gitbook/assets/image (996).png" alt=""><figcaption><p>Date picker in filters</p></figcaption></figure>

When you have a date dimension in your rows, you can use the new **Date Period** option to filter your row data between 2 specific dates.&#x20;

<figure><img src="../.gitbook/assets/image (997).png" alt=""><figcaption><p>Date period filter</p></figcaption></figure>

#### **2.3. Filter based on measure name**

Navigating and locating specific measures may prove time-consuming when your reports contain many measures. You can now display selected measures by creating measure-name-based filters.

<figure><img src="../.gitbook/assets/image (998).png" alt=""><figcaption><p>Measure filter</p></figcaption></figure>

You can quickly switch between different relevant measure combinations with this option.

<figure><img src="../.gitbook/assets/2.3.2. switch-measure-combinations-gif.gif" alt=""><figcaption><p>Measure filters</p></figcaption></figure>

#### **2.4. Interface change for filters**&#x20;

Is deciphering complex, multi-condition filters proving to be laborious? The filter interface has been upgraded to show the links between filter conditions, making them much easier to grasp.&#x20;

<figure><img src="../.gitbook/assets/image (999).png" alt=""><figcaption><p>New filter interface</p></figcaption></figure>

#### **2.5. Date conditions in conditional formatting**&#x20;

You can directly use date range conditions, such as the order date being in the last n days or the ship date being in the next n days, as a conditional formatting rule.&#x20;

<figure><img src="../.gitbook/assets/image (1000).png" alt=""><figcaption><p>Date-based conditional formatting</p></figcaption></figure>

#### **2.6. Hide measure values with conditional formatting**&#x20;

Business reporting may require withholding certain information to protect strategic interests. You can now use conditional formatting to mask values based on specific criteria.&#x20;

We’ve hidden the COGS values when the Discount is less than 10k.&#x20;

<figure><img src="../.gitbook/assets/image (1001).png" alt=""><figcaption><p>Hiding measure values</p></figcaption></figure>

#### **2.7. Conditional formatting for measure headers**&#x20;

Based on your data, you can highlight measure headers. For instance, you can highlight the quarters/months in which the overall sales exceed a target amount. You can select the dimensions from the **Target column** box.&#x20;

<figure><img src="../.gitbook/assets/image (1002).png" alt=""><figcaption><p>CF for measure headers</p></figcaption></figure>

## 3. Settings  <a href="#settings" id="settings"></a>

#### **3.1. Totals/subtotals for date fields**&#x20;

Aggregation may not necessarily apply to non-numeric fields. Inforiver provides the option of leaving the total and subtotal cells blank for non-numeric fields. This feature has been extended to date fields as well in this release.&#x20;

<figure><img src="../.gitbook/assets/image (1003).png" alt=""><figcaption><p>Disable totals/subtotals for non-numeric measures</p></figcaption></figure>

## **3.2. APS options moved to display settings**&#x20;

* **Absolute search:** Locate a value irrespective of its sign. This option has been added to the Misc tab.&#x20;

<figure><img src="../.gitbook/assets/image (1004).png" alt=""><figcaption><p>Absolute search</p></figcaption></figure>

* **Populate missing AC with FC:** When the AC measure is unavailable, the missing values can be substituted with the corresponding FC measure.&#x20;

<figure><img src="../.gitbook/assets/image (969).png" alt=""><figcaption><p>Replace missing AC with FC</p></figcaption></figure>

* **Customize for Indian numbering system:** This enables the lakhs and crores units that are specific to the Indian number system.&#x20;

<figure><img src="../.gitbook/assets/image (970).png" alt=""><figcaption><p>Indian number system</p></figcaption></figure>

* **Show Info logo:** The Inforiver logo will be displayed at the bottom right corner of the visual.

<figure><img src="../.gitbook/assets/image (971).png" alt=""><figcaption><p>Show info logo</p></figcaption></figure>

**3.3. Custom suffix for row subtotals split**&#x20;

Inforiver allows you to customize the row and column totals and subtotals with the Totals feature. The subtotal is displayed as a separate row when you choose the split option for row subtotals. After splitting subtotals, you can set a custom suffix for the row subtotal.

<figure><img src="../.gitbook/assets/image (972).png" alt=""><figcaption><p>Subtotal suffix</p></figcaption></figure>

**3.4. Custom labels for blank row and column categories**&#x20;

Inforiver provides numerous options for handling null data in the source. With the latest version, you can provide a default label for blank row and column dimension categories.

<figure><img src="../.gitbook/assets/image (973).png" alt=""><figcaption><p>Custom labels for blank dimensions</p></figcaption></figure>

**3.5. Show column filter**&#x20;

We’ve added a new, easily accessible column filter interface. This can be enabled by turning on the **Show Column Filter** option in the Misc tab. The **Enable Canvas Rendering** option should also be enabled from the General tab.

<figure><img src="../.gitbook/assets/image (974).png" alt=""><figcaption><p>Show column filter</p></figcaption></figure>

**3.6. Rotate the first row dimension vertically**&#x20;

You can display the dimension in the Rows parameter in a banner format with the categories rotated vertically. To turn on this option, the General settings > Enable Canvas Rendering option also needs to be enabled.&#x20;

<figure><img src="../.gitbook/assets/image (975).png" alt=""><figcaption><p>Rotate row dimension</p></figcaption></figure>

**3.7. Suppress null visual columns**&#x20;

You may have calculated fields in your report that are null for certain categories. Inforiver provides the option of suppressing such fields that do not add value to the report.

<figure><img src="../.gitbook/assets/image (976).png" alt=""><figcaption><p>Suppress null visual columns</p></figcaption></figure>

Enable the **Suppress Null Visual Columns** option to hide visual measures/columns that are entirely blank

<figure><img src="../.gitbook/assets/image (977).png" alt=""><figcaption><p>Suppress null visual columns</p></figcaption></figure>

**3.8. On data change scripts**&#x20;

You can now execute scripts on changing the data selections in an external slicer/filter. For instance, you can enhance the relevance of data by drilling up/down or mask data in response to a specific selection. The exact scripting functions used in variables or on-load can be used for data changes.

<figure><img src="../.gitbook/assets/3.8. on-data-change-scripts.gif" alt=""><figcaption><p>On data change scripts</p></figcaption></figure>

* We have introduced a new SETCOLUMNSORT scripting function to sort columns in ascending or descending order.

<figure><img src="../.gitbook/assets/image (979).png" alt=""><figcaption><p>SETCOLUMNSORT function</p></figcaption></figure>

**3.9. Reset formats for selected cells**&#x20;

Have you ever applied a series of formatting changes and found it challenging to undo them? Inforiver provides a handy **Reset Formats** option. Select the cells and click **Reset Formats** to instantly restore default formatting.

<figure><img src="../.gitbook/assets/3.9. reset-formats-selected-cells.gif" alt=""><figcaption><p>Reset formats for selected cells</p></figcaption></figure>

**3.10. Populate missing FC with PY/PL**&#x20;

If your reports contain forecast measures with missing values for certain periods, you can use either PL or PY values to replace the null forecast values.&#x20;

<figure><img src="../.gitbook/assets/image (981).png" alt=""><figcaption><p>Missing FC values</p></figcaption></figure>

Populate missing FC with PY:

<figure><img src="../.gitbook/assets/image (982).png" alt=""><figcaption><p>Populate missing FC with PY</p></figcaption></figure>

Populate missing FC values with PL:

<figure><img src="../.gitbook/assets/image (983).png" alt=""><figcaption><p>Populate missing FC with PL</p></figcaption></figure>

**3.11. Right-to-left support**&#x20;

Reports with RTL support improve the user experience for readers of RTL languages, making it easier for them to navigate, understand, and interpret the information presented. When the right-to-left option is enabled:&#x20;

* Data is arranged from right to left; notice how the months are arranged from December to January. &#x20;
* The row categories are displayed on the right-hand side.&#x20;
* Toolbar options are arranged from right to left.&#x20;
* The header is positioned at the right end of the report.

<figure><img src="../.gitbook/assets/3.11. Right to left.png" alt=""><figcaption><p>RTL support</p></figcaption></figure>

**3.12. Localization settings**&#x20;

You can configure translations in Inforiver based on the language settings in Power BI. If your report has a global audience, you can configure calculated rows/columns or column groups to display dimension categories based on pre-defined translations when the language is switched.&#x20;

Navigate to Display Settings > General > Localization Settings to create translation entries.&#x20;

<figure><img src="../.gitbook/assets/3.12.1. Localization config.png" alt=""><figcaption><p>Localization settings</p></figcaption></figure>

Use the GETLOCALELABEL function in the Title field and pass the Key specified in the translation config.

<figure><img src="../.gitbook/assets/3.12.2. Getlocalelable function.png" alt=""><figcaption><p>GETLOCALELABEL</p></figcaption></figure>

Notice how the row categories and column groups are implicitly changed to French and German.

<div>

<figure><img src="../.gitbook/assets/3.12.3. Francais.png" alt=""><figcaption><p>French</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/3.12.4. German.png" alt=""><figcaption><p>German</p></figcaption></figure>

</div>

**3.13. Hide repeating parent rows**&#x20;

Hierarchical datasets may contain categories with the same name on multiple levels.

<figure><img src="../.gitbook/assets/image (984).png" alt=""><figcaption><p>Repeating categories</p></figcaption></figure>

You can now suppress parent levels with the same name by enabling the **Hide Repeating Parent Rows** option.

<figure><img src="../.gitbook/assets/image (985).png" alt=""><figcaption><p>Hide repeating parent rows</p></figcaption></figure>
