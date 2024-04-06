# Export to PDF & Excel

Inforiver allows you to export the table/matrix as either PDF or Excel. The industry-leading export capability delivers the following:

* Export with formatting, category/value structure and notes ​
* Export table/matrix along with scaled number formatting​
* Export calculated rows, columns, and edited cells​
* ​End-users in the reading view can customize export options​​
* ​Export to Excel with expand/collapse capability
* Export to multiple Excel worksheets based on category values​
* ​Pagination & page-break support for Export to PDF

You can find the export option under the 'Export' tab of the toolbar. There are two sections: 'Export to PDF' & 'Export to Excel'. Let's take a look one by one.

<figure><img src="../../.gitbook/assets/Export.png" alt=""><figcaption><p>Export options</p></figcaption></figure>

{% hint style="warning" %}
Export to PDF/Excel is supported only in Power BI Service.
{% endhint %}

### 1. Export to PDF

The first step in exporting as a PDF file is configuring the page setup.&#x20;

### i) Page setup

The page setup section provides options to customize the page size, orientation, margin etc. Click 'Page Setup', and a window opens as shown.

<figure><img src="../../.gitbook/assets/Page settings.png" alt=""><figcaption><p>Page setup</p></figcaption></figure>

a) When the number of rows/columns doesn't fit on a single page, you can define the order in which the rows/columns are exported using the '**Content order**' option.

Let's consider the below example. Based on the page scaling, only 8 columns and 20 rows can be accommodated on a single page.&#x20;

When the '**Row first**' option is chosen, the remaining rows for the first 8 columns are displayed on the second page. The third and fourth-page contents are highlighted in the image.

<figure><img src="../../.gitbook/assets/6.1.34 Export Row first.png" alt=""><figcaption><p>Row-first export</p></figcaption></figure>

When the '**Column first**' option is chosen, the remaining columns for the first 20 rows are displayed on the second page. The third and fourth-page contents are highlighted in the image.

<figure><img src="../../.gitbook/assets/6.1.35 Export Column first.png" alt=""><figcaption><p>Column-first export</p></figcaption></figure>

b) Select the '**Page size**' from the drop-down - Available sizes are Letter, A3, A4, A5. Tabloid and Legal.

c) You can select either Landscape or Portrait as page '**Orientation**'.

d) You can scale the page manually by percentages or automatically scale to fit all columns in a single page using the '**Scaling**' option.

e) You can apply a Narrow, Normal or Wide '**Margin**' as per the requirement.

f) You can select 'Font' style from the available options in the dropdown. Custom fonts can also be used when exporting.

{% hint style="info" %}
If the data is customized with different fonts, the font chosen in the Settings panel is used for PDF export.
{% endhint %}

g) You can '**Show header and footer**' either only on the First Page or on Every Page

h) You can create a cover page for your report by **First page image** toggle. Select a custom image to use as the cover page.

<figure><img src="../../.gitbook/assets/image (502).png" alt=""><figcaption><p>Cover image</p></figcaption></figure>

&#x20;i) If you want the image to fill the entire cover page, select the **Use as background image** checkbox**.**

<figure><img src="../../.gitbook/assets/image (503).png" alt=""><figcaption><p>Use as background image for PDF extracts</p></figcaption></figure>

j) You can capture comments and replies **i**n the fully formatted PDF exports. Check the **'Include comment replies'** to export the replies in the comments column.

<figure><img src="../../.gitbook/assets/image (378) (1).png" alt=""><figcaption><p>Report that has comments and replies</p></figcaption></figure>

After exporting the report to a PDF, you will be able to see formatted comments and replies in the file.

<figure><img src="../../.gitbook/assets/6.1. Comments replies (1).png" alt=""><figcaption><p>Comments and replies</p></figcaption></figure>

k)You can select the '**Include footnotes**' option to export the footnotes along with the table/matrix

l) You can set the '**Footnote position**' as

* Last Page: Footnotes get printed on the last page.
* Dynamic: Based on the available space, footnotes get printed either on the same page where they are added or on the last page.

m) Click on 'Update' to save your page setup selection. Click on 'Reset' to reset all your selections.&#x20;

### ii) Exporting

Once the page setup is complete, you need to choose whether the entire matrix needs to be exported or just selected columns.&#x20;

#### Entire matrix

a) You can export all the rows and columns by clicking 'Entire Matrix'. Click on 'PDF Report' to export the file in PDF format.

<figure><img src="../../.gitbook/assets/Entire.png" alt=""><figcaption><p>Export entire matrix PDF</p></figcaption></figure>

c) A pop-up appears as shown. The PDF file can be either saved to the computer or it can be sent by email. To save the document, choose 'Save to Computer', and click on the 'Click to export' option.&#x20;

<figure><img src="../../.gitbook/assets/6.1.1 Export pdf.png" alt=""><figcaption><p>Pop up</p></figcaption></figure>

e) A pop-up appears showing a warning, click 'Download'.

<figure><img src="../../.gitbook/assets/6.1.2 Export pdf.png" alt=""><figcaption><p>Download popup</p></figcaption></figure>

f) The entire matrix gets exported as shown.

<figure><img src="../../.gitbook/assets/Entire matrix PDF (1).png" alt=""><figcaption><p>Entire matrix PDF</p></figcaption></figure>

#### Selected columns

If you need to export only selected columns of your report, click 'Selected Columns' as highlighted in the below image.

<figure><img src="../../.gitbook/assets/ExportSelected.png" alt=""><figcaption><p>Export selected columns</p></figcaption></figure>

The selected columns 'Quarter, Q1, Q2' are downloaded as shown.

<figure><img src="../../.gitbook/assets/Selected Columns PDF.png" alt=""><figcaption><p>Selected columns PDF</p></figcaption></figure>

{% hint style="info" %}
Export to PDF does not support image columns.
{% endhint %}

### &#x20;2. Export to Excel

You can export your report as an Excel file by clicking on the 'Export report' dropdown as shown in the below image.

When there are row/column hierarchies, there are three ways to export:  'Fully Expanded', 'With Expand/Collapse', and 'Current State'.&#x20;

<figure><img src="../../.gitbook/assets/ExportReport.png" alt=""><figcaption><p>Export report</p></figcaption></figure>

{% hint style="warning" %}
Note that 'Page setup' is not applicable for export to Excel.
{% endhint %}

Let's look at the three options one by one.

### i) Fully expanded

You can export the visual with all rows fully expanded by choosing the 'Fully Expanded' option. In the Inforiver visual, you can see that 'East' and Pacific -> Beverages are collapsed.&#x20;

<figure><img src="../../.gitbook/assets/FullyExpanded1.png" alt=""><figcaption><p>Fully expanded option</p></figcaption></figure>

In the exported Excel, you can see that 'East' and Pacific -> Beverages are fully expanded.

<figure><img src="../../.gitbook/assets/FullyExpandedExcel.png" alt=""><figcaption><p>Fully expanded excel report</p></figcaption></figure>

### ii) With expand/collapse

To export as Excel with expand/collapse-enabled row hierarchies, select the 'With Expand/collapse' option.

<figure><img src="../../.gitbook/assets/Expandcollapse.png" alt=""><figcaption><p>With expand/collapse option</p></figcaption></figure>

The downloaded Excel shows the same expand/collapse state as in the report and also has the expand/collapse buttons.

<figure><img src="../../.gitbook/assets/Excel Report-with Excol.png" alt=""><figcaption><p>Excel report with expand/collapse</p></figcaption></figure>

{% hint style="info" %}
Export to Excel retains the expand/collapse state only for row hierarchy and not for column hierarchy.
{% endhint %}

### iii) Current state&#x20;

To export the current expand/collapse state without an option to expand/collapse in the Excel file, you can select the 'Current state' option.

<figure><img src="../../.gitbook/assets/CurrentStatereport.png" alt=""><figcaption><p>Current state option</p></figcaption></figure>

The downloaded Excel shows the same expand/collapse state as in the report.

<figure><img src="../../.gitbook/assets/Excel Report-currentstate.png" alt=""><figcaption><p>Current state report</p></figcaption></figure>

{% hint style="info" %}
Export to Excel does not support images and charts. Only basic icons that are available in excel, rating, and data bars are supported.
{% endhint %}

### 3. Copy to clipboard

You can copy the data from your Inforiver visual including the calculated row, columns, edits, and notes (if there are any). The copied data can be easily pasted into an Excel sheet.&#x20;

{% hint style="info" %}
The keyboard shortcut for the copy to clipboard option is **'Ctrl+C+L'**
{% endhint %}

<figure><img src="../../.gitbook/assets/copy-to-clipboard.png" alt=""><figcaption><p>Copy to clipboard</p></figcaption></figure>

The above data has been copied and pasted in an Excel sheet and it gets displayed as shown in the below image.

<figure><img src="../../.gitbook/assets/pasted-data-in-excel.png" alt=""><figcaption><p>Pasted data in Excel</p></figcaption></figure>

Another way to share reports is by sending ad-hoc emails. To learn more, refer to [Send to email](ad-hoc-emails.md).

#### Resources

[Formatted Export to PDF in Power BI](https://inforiver.com/blog/general/formatted-export-to-pdf-in-power-bi/)

[Formatted Export to Excel/Spreadsheets in Power BI](https://inforiver.com/blog/general/formatted-export-to-excel-spreadsheets-in-microsoft-power-bi/)
