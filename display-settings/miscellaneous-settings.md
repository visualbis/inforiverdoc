# Miscellaneous settings

### 1. View

#### i) Visual context menu

When the _Visual context menu_ option is enabled, a context menu is displayed by right-clicking a row.

<figure><img src="../.gitbook/assets/image (35).png" alt=""><figcaption><p>Visual context menu</p></figcaption></figure>

#### ii) Header word wrap

When the _Header Word Wrap_ option is enabled, the header content is wrapped according to the height of the cell. The image below shows how the headers are displayed when the header word wrap option is disabled.

<figure><img src="../.gitbook/assets/image (36).png" alt=""><figcaption><p>Header word wrap disabled</p></figcaption></figure>

You will be able to see the entire header when word wrap is enabled.

<figure><img src="../.gitbook/assets/image (37).png" alt=""><figcaption><p>Header word wrap enabled</p></figcaption></figure>

#### iii) Quick shortcuts

This option lets you add quick shortcut icons in the Actions section. The _Undo, Redo, Export as Excel_, and _Best Fit_ options are selected by default. You can select additional options including _Export PDF, Aggregation_, and _Smart Analysis_. The shortcuts for all the selected options will be displayed in the Actions section.

<figure><img src="../.gitbook/assets/image (38).png" alt=""><figcaption><p>Quick shortcuts</p></figcaption></figure>

#### iv) Show info messages

You can disable this option if you do not wish to see pop-up notifications and info messages.

<figure><img src="../.gitbook/assets/image (39).png" alt=""><figcaption><p>Show info messages</p></figcaption></figure>

#### v) Absolute sort

Enabling this option will sort measures based on the magnitude, irrespective of whether a value is positive or negative.

<figure><img src="../.gitbook/assets/image (334).png" alt=""><figcaption><p>Absolute sort disabled</p></figcaption></figure>

Notice how the values are sorted based on magnitude when absolute sort is turned on.

<figure><img src="../.gitbook/assets/image (335).png" alt=""><figcaption><p>Absolute sort enabled</p></figcaption></figure>

#### vi) Show measure header

The column or measure headers will hidden if this option is disabled.

<figure><img src="../.gitbook/assets/image (336).png" alt=""><figcaption><p>Show measure header</p></figcaption></figure>

#### vii) Fiscal year start month

Inforiver supports planning, budgeting, and forecasting for fiscal periods as well. You can set the start month of the fiscal year using this option.

<figure><img src="../.gitbook/assets/image (337).png" alt=""><figcaption><p>Fiscal year start month</p></figcaption></figure>

#### viii) Show floating toolbar

When the main toolbar has been unpinned, you will still be able to apply cell-level formatting, show/hide cell values, and add comments using the floating toolbar. Disable this option if you do not require the floating toolbar.

<figure><img src="../.gitbook/assets/image (338).png" alt=""><figcaption><p>Show floating toolbar</p></figcaption></figure>

#### ix) Diagnose

This option can be enabled if you wish to mask your data and generate random values when the data is being shared and security is a concern.

#### x) Allow native measure editing in read view

If this option is enabled, report users in the reading view can update native measures.

#### xi) Increase scroll thickness

You can increase the thickness of the horizontal and vertical scrollbars using by enabling this option.

<figure><img src="../.gitbook/assets/image (10) (1) (1).png" alt=""><figcaption><p>Increase scroll thickness</p></figcaption></figure>

#### xii) Hide pinned base rows

Inforiver’s _pin rows_ feature enables you to tag important rows in your data at the top of your report. Using this feature creates duplicate rows at the visual level (there is no change to your data). In the report below, notice how the pinned rows such as ‘Bookcases’ are repeated in the table below.&#x20;

<figure><img src="../.gitbook/assets/2.2. Settings Display hide base pinned rows.png" alt=""><figcaption><p>Hide base pinned rows disabled</p></figcaption></figure>

You can enable the _**Hide pinned base rows**_ option to hide the actual row and retain only the pinned rows.&#x20;

<figure><img src="../.gitbook/assets/2.2.1. hide pinned rows output.png" alt=""><figcaption><p>Hide pinned base rows enabled</p></figcaption></figure>

### 2. Status bar

#### i) Show status bar

You can show/hide the status bar with this option. If this option is enabled, the _Status Panel Aggregation_ option becomes available.&#x20;

#### ii) Status panel aggregation

The _Status Panel Aggregation_ option allows you to show the aggregation such as sum, average, min, max, and count for the values selected in the visual. In the below example, you can see the sum, average, and count aggregation for the selected values/measure in the status bar.

{% hint style="info" %}
Only a maximum of three aggregations are displayed in the status bar.
{% endhint %}

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Status panel aggregation</p></figcaption></figure>

### 3. Cell/row/column

#### i) Global error handling

Inforiver provides a global error handling setting that internally handles missing reference errors and converts the missing values to 0 when used in calculations.&#x20;

Consider that you are deriving the standard deviation for beverages across EMEA and APAC regions.

<figure><img src="../.gitbook/assets/7.4.1 Reference errors original data (1).png" alt=""><figcaption><p>Creating a calculated row</p></figcaption></figure>

If EMEA data is not available, the calculation will still work seamlessly in the report without throwing errors.

<figure><img src="../.gitbook/assets/7.4.2. Error handling data after removing.png" alt=""><figcaption><p>Caculation works without errors when the setting is on</p></figcaption></figure>

Notice how a missing reference error is displayed when the error handling setting is disabled.

<figure><img src="../.gitbook/assets/7.4.3. Ref error.png" alt=""><figcaption><p>Global error handling</p></figcaption></figure>

#### ii) Edit cell indicator

This option allows you to identify the edited/modified cell values in the visual. If you enable this option, the modified cell values are indicated by a pencil icon next to the corresponding values.&#x20;

<figure><img src="../.gitbook/assets/image (340).png" alt=""><figcaption><p>Edit cell indicator</p></figcaption></figure>

#### iii) Show row indicator

You can identify manually inserted rows by enabling this option. A pencil icon is displayed next to data input or calculated rows.

<figure><img src="../.gitbook/assets/image (342).png" alt=""><figcaption></figcaption></figure>

#### iv) Row label editor

This option allows you to identify if the original row labels are modified in the visual. If you enable this option, the modified row labels are indicated by an edit icon next to the corresponding label.&#x20;

<figure><img src="../.gitbook/assets/image (343).png" alt=""><figcaption><p>Row label editor</p></figcaption></figure>

#### v) Common measure width

Changing the width of one column will change the width of all other columns accordingly when this option is enabled. If this option is disabled, the width of every single column can be changed individually. In the below image, the width of the Qtr 2 column alone is modified.

<figure><img src="../.gitbook/assets/image (344).png" alt=""><figcaption><p>Common measure width</p></figcaption></figure>

#### vi) Column spacing

This option allows you to adjust the spacing between the columns. If this option is turned on, you can specify the required column spacing in the input field.

{% hint style="info" %}
The minimum and maximum values of column spacing are 0 and 20 respectively.
{% endhint %}

<figure><img src="../.gitbook/assets/image (345).png" alt=""><figcaption></figcaption></figure>

#### vii) Pin icon

You can select a custom icon for pinned rows and columns.

<figure><img src="../.gitbook/assets/image (346).png" alt=""><figcaption><p>Pin icon</p></figcaption></figure>

### 4. Reading view tooltip

Inforiver offers customizations for the tooltip in the reading view.

**i) Scaled tooltip for numbers** - Enabling this option will display the values in a scaled format in the tooltip.

**ii) Custom decimals** - Enabling this option lets you customize the decimal points to be displayed in the tooltip

**iii) Decimal places** - Field where you can enter the number of decimal places

The below image shows the values in a scaled format with one decimal point as specified.

<figure><img src="../.gitbook/assets/image (347).png" alt=""><figcaption><p>Reading view tooltip</p></figcaption></figure>
