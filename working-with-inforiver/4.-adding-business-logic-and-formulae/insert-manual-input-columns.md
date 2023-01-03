# Insert manual input columns

Inforiver provides six (6) different options to manually enter data in your Power BI report which are listed below.

| Input type                                                           | Description                                                                                               |
| -------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| [Number](insert-manual-input-columns/insert-manual-input-columns.md) | Double-click and start typing values in directly into a cell                                              |
| [Text](formula-syntax/text-formatting-functions/text.md)             | Enter text with multi-line support and word wrap                                                          |
| [Dropdown](insert-manual-input-columns/dropdown.md)                  | Use the available presets or create your own list of values; supports both single-select and multi-select |
| [Date](insert-manual-input-columns/text-checkbox-and-date.md)        | Add a date from the calendar / date picker                                                                |
| [Checkbox](insert-manual-input-columns/text-checkbox-and-date.md)    |                                                                                                           |
| [Person](insert-manual-input-columns/enterprise-features.md)         | Input users from your organization (only available in Inforiver Enterprise)                               |

{% hint style="warning" %}
Inforiver Matrix offers only the first five types. Input types and features specific to Inforiver Enterprise are covered in a later [section](insert-manual-input-columns/enterprise-features.md).&#x20;
{% endhint %}

### 1. Sign-in

a) If you are using the Enterprise version, you need to sign in as shown below.

{% hint style="info" %}
Sign-in is optional. Unless specified, all these features are available in Inforiver Matrix as well.
{% endhint %}

<figure><img src="../../.gitbook/assets/4.4.0 Login.png" alt=""><figcaption><p>Sign in with Office 365 account</p></figcaption></figure>

b) Once you sign in successfully, your profile picture will be displayed as seen in the image.

<figure><img src="../../.gitbook/assets/4.4.1 Login.png" alt=""><figcaption><p>Sign in successful</p></figcaption></figure>

c) You can now start inserting a column to capture your data inputs by clicking on Insert --> Data Input.&#x20;

<figure><img src="../../.gitbook/assets/4.4.1 Data input.png" alt=""><figcaption><p>Data input columns</p></figcaption></figure>

Before we look at inserting data input columns, let's look at some common properties available for all the input types.

### 2. Measure vs column

Data input columns can be inserted as a measure or a column.&#x20;

**Visual measure:** If there is a column hierarchy, the input column is inserted for each category. In case of no column hierarchy, a single column is inserted.&#x20;

In the below image, a text column has been inserted as a measure by selecting 'Insert as' -> 'Visual measure'.

<figure><img src="../../.gitbook/assets/4.4.10 Insert as.png" alt=""><figcaption><p>Visual measure</p></figcaption></figure>

**Visual column:** Irrespective of whether there is a column hierarchy or not, a single column gets inserted.

In the below image, a text column has been inserted as a column by selecting 'Insert as' -> 'Visual column'.

<figure><img src="../../.gitbook/assets/4.4.11 Insert as.png" alt=""><figcaption><p>Visual column</p></figcaption></figure>

### 3. Input restrictions

By default, inputs are enabled in both read and edit modes in Power BI. But, based on your requirement, you can allow inputs only in edit mode or based on a formula.

<figure><img src="../../.gitbook/assets/4.4.12 allow input.png" alt=""><figcaption><p>Restrictions on input</p></figcaption></figure>

a) Only in edit mode:

When the 'Only in edit mode' option is chosen, the text editor is disabled.

<figure><img src="../../.gitbook/assets/4.4.15 only edit mode.png" alt=""><figcaption><p>Data input disabled in reading mode</p></figcaption></figure>

b) In both Power BI read and edit modes:

When the option 'In both Power BI read and edit modes' is selected, you can enter data in the reading view as shown below.

<figure><img src="../../.gitbook/assets/4.4.16 read and edit modes.png" alt=""><figcaption><p>Data input in reading mode</p></figcaption></figure>

c) Based on a formula:

You can allow data input only if a certain condition is met. The formula entered should return a boolean.

In the below image, data input is allowed only if (2022 Actuals - 2022 Plan)% < 0. You can see that the text fields for Central and Midwest are greyed out.

<figure><img src="../../.gitbook/assets/4.4.14(2) formula.png" alt=""><figcaption><p>Allow input based on formula</p></figcaption></figure>
