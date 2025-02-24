# Text, checkbox & date

In addition to [number](insert-manual-input-columns.md) and [dropdown](dropdown/) input columns, you can also use columns of types text, checkbox and date to capture manual data.

Let's cover them one by one.

{% hint style="info" %}
If you are using Inforiver Enterprise, you need to [sign in](../insert-manual-input-columns.md#1.-sign-in) to start inserting a number column.&#x20;
{% endhint %}

## 1. Text

Text columns or measures can be inserted to capture text.&#x20;

a) Select 'Text' from the _Data Input_ dropdown.

<figure><img src="../../../.gitbook/assets/image (255).png" alt=""><figcaption><p>Data input - text</p></figcaption></figure>

b) The text column side panel is shown in the image below.&#x20;

You can choose to [insert as a visual measure or column](../insert-manual-input-columns.md#1.-insert-as). Text entry can be enabled or disabled in the total/subtotal rows using the 'Allow entry on total/subtotal rows' checkbox. Input access can be configured using the '[Allow input](../insert-manual-input-columns.md#2.-allow-input)' option. You can also set field validations which will be discussed later in this section.

Click 'Create'.

<figure><img src="../../../.gitbook/assets/image (256).png" alt=""><figcaption></figcaption></figure>

c) The text column gets inserted. Double-click on any of the cells and start typing the text in the editor. Press Enter to commit the text entry.

<figure><img src="../../../.gitbook/assets/image (257).png" alt=""><figcaption></figcaption></figure>

#### 1.1. Word wrap

Inforiver provides an option to wrap the text for long entries that get truncated.

<figure><img src="../../../.gitbook/assets/image (258).png" alt=""><figcaption><p>Text entry truncated</p></figcaption></figure>

Click on the word wrap icon in the Home ribbon to wrap text as per the width of the field.

<figure><img src="../../../.gitbook/assets/image (259).png" alt=""><figcaption><p>Word wrap</p></figcaption></figure>

#### 1.2. Text validations

Inforiver provides the ability to add data validations for text inputs. You can add validations to check the length, and data type (numeric/text/alphanumeric).&#x20;

<figure><img src="../../../.gitbook/assets/image (264).png" alt=""><figcaption><p>Text validations</p></figcaption></figure>

You can also enforce that a text entry should be an email or URL or even provide a regular expression using the Custom option.

<figure><img src="../../../.gitbook/assets/image (265).png" alt=""><figcaption></figcaption></figure>

For example, if you choose email as _Field Validation_ and the data entered is not a valid email ID, Inforiver will generate a pop-up error notification.

<figure><img src="../../../.gitbook/assets/image (266).png" alt=""><figcaption><p>Error notification when validation fails</p></figcaption></figure>

#### 1.3. Default values

Blank fields do not add value and are likely to reduce the appeal of a report. You can choose to use default values instead of displaying blank text data input fields. You can either enter a static default value or assign a dimension.

<div><figure><img src="../../../.gitbook/assets/image (909).png" alt=""><figcaption><p>Static default value</p></figcaption></figure> <figure><img src="../../../.gitbook/assets/2024-08-12_11h51_11.png" alt=""><figcaption><p>Dimension as a default value</p></figcaption></figure></div>



## 2. Checkbox

Checkbox columns or measures can be inserted to capture binary inputs. Click on 'Checkbox' in the 'Data input' dropdown.

<figure><img src="../../../.gitbook/assets/4.4.3.8 Checkbox.png" alt=""><figcaption><p>Data input column - Checkbox</p></figcaption></figure>

The checkbox column side panel is shown in the below image.&#x20;

You can choose to [insert as a visual measure or column](../insert-manual-input-columns.md#1.-insert-as). Entry can be enabled or disabled in the total/subtotal rows using the '[Allow entry on total/subtotal rows](dropdown/#iii-entry-in-total-subtotal-rows)' checkbox. Input access can be configured using the '[Allow input](../insert-manual-input-columns.md#2.-allow-input)' option.&#x20;

Click 'Create'.

<figure><img src="../../../.gitbook/assets/4.4.3.9 Checkbox.png" alt=""><figcaption><p>Checkbox column</p></figcaption></figure>

Click on any of the cells to check the checkbox.

<figure><img src="../../../.gitbook/assets/4.4.3.10 Checkbox.png" alt=""><figcaption><p>Making a selection</p></figcaption></figure>

## 3. Date

Date columns or measures can be inserted by clicking on 'Date' in the 'Data input' dropdown. You can insert an empty column or copy the dates from the rows in the report.

<figure><img src="../../../.gitbook/assets/image (727) (1).png" alt=""><figcaption><p>Data input column - Date</p></figcaption></figure>

### i) Create an empty series&#x20;

When you select this option, an empty date column is created and the side panel opens as shown in the image.

<figure><img src="../../../.gitbook/assets/image (728) (1).png" alt=""><figcaption><p>Date column type properties</p></figcaption></figure>

You can choose to [insert it as a visual measure or column](../insert-manual-input-columns.md#1.-insert-as). Entry can be enabled or disabled in the total/subtotal rows using the '[Allow entry on total/subtotal rows](dropdown/#iii-entry-in-total-subtotal-rows)' checkbox. Input access can be configured using the '[Allow input](../insert-manual-input-columns.md#2.-allow-input)' option.&#x20;

You can also configure other optional fields as below:

#### Format

The date format can be changed by clicking the 'Format' dropdown. Choose the desired format.

<figure><img src="../../../.gitbook/assets/image (729) (1).png" alt=""><figcaption><p>Date format</p></figcaption></figure>

#### Minimum and Maximum Date

You can set the minimum and maximum date ranges for the date input. Users will not be able to enter any dates that fall outside this range. You can enter both dates to specify a range, or just the minimum or the maximum date. To select a date, click the calendar icon.

<figure><img src="../../../.gitbook/assets/image (730) (1).png" alt=""><figcaption><p>Minimum and maximum date ranges</p></figcaption></figure>

#### Default value

In a report that has thousands of rows, manually entering or copying dates in a data input-date field can be a tedious task. In such cases, you can set a default date. All rows will be filled with the configured default date as soon as you click **Create**.

There are multiple options to set a default date:

* **Static value**: Use the date picker to set a common date for all the rows. In the image below, the created date column is pre-filled with the default date - 07/01/2024.

<figure><img src="../../../.gitbook/assets/3.1.1. Static Value.png" alt=""><figcaption><p>Static value as default date</p></figcaption></figure>

* **Measure**: Select the measure (native measure/formula measure/date input column) from which the default date should be sourced. In the example below, the default value is sourced from a formula measure that is available within the same report.

<figure><img src="../../../.gitbook/assets/3.1.3. Measure default date.png" alt=""><figcaption><p>Setting a measure value as default date</p></figcaption></figure>

* **Dimension**: When you have a date dimension in your row, you can select the row dimension from which the default date must be picked. The default date in the example below is picked from the row dimension, 'Order Date'.

<figure><img src="../../../.gitbook/assets/3.1.2. Dimension default date.png" alt=""><figcaption><p>Setting a dimension value as default date</p></figcaption></figure>

{% hint style="info" %}
The default date option is available for both visual measures and visual columns. Invalid date format errors are implicitly handled as blanks for a clean export and writeback.
{% endhint %}

After configuring the required settings, click **Create.**

<figure><img src="../../../.gitbook/assets/image (731) (1).png" alt=""><figcaption><p>Create date column</p></figcaption></figure>

The date column gets inserted.

#### Entering a date

To enter data, double-click on a cell. Select a date from the calendar/date picker.&#x20;

<figure><img src="../../../.gitbook/assets/image (732).png" alt=""><figcaption><p>Choosing a date as input</p></figcaption></figure>

The date gets captured in the chosen format.

<figure><img src="../../../.gitbook/assets/image (733).png" alt=""><figcaption><p>Date gets captured</p></figcaption></figure>

### ii) Copy from rows

If your report has a list of calendar dates in the row dimension, and you want to replicate the same dates in an input column, you can use the **‘copy from rows’** option, instead of manually entering it for each record.

<figure><img src="../../../.gitbook/assets/image (736).png" alt=""><figcaption><p>Copy from rows </p></figcaption></figure>

Inforiver automatically detects the date format which can be verified from the pop-up.

<figure><img src="../../../.gitbook/assets/image (737).png" alt=""><figcaption><p>Automatic date format detection </p></figcaption></figure>

In rare cases when the format mapping is not as expected, you can map them manually using the help suggestions and click **Submit.**&#x20;

<figure><img src="../../../.gitbook/assets/image (775).png" alt="" width="563"><figcaption><p>Suggestions for manual mapping</p></figcaption></figure>

The date column is inserted as shown, which follows the dates in the rows. By default, the first of January is the fiscal year's start.

<figure><img src="../../../.gitbook/assets/image (738).png" alt=""><figcaption><p>Date column inserted</p></figcaption></figure>



**Note:** Inforiver accepts both hierarchical and non-hierarchical date formats. For example, the visual below has date formats such as half-years, quarters, and months assigned as individual fields instead of using a date hierarchy. Inforiver automatically maps them using the custom formats.

<figure><img src="../../../.gitbook/assets/image (772).png" alt=""><figcaption><p>Mapping non-hierarchical date format</p></figcaption></figure>

The inserted date column is shown below after setting the required fiscal year.

<figure><img src="../../../.gitbook/assets/image (773).png" alt=""><figcaption><p>Date column inserted</p></figcaption></figure>

Unconventional date formats are also accepted and automatically mapped.

<figure><img src="../../../.gitbook/assets/image (774).png" alt=""><figcaption><p>Unconventional date formats mapped</p></figcaption></figure>

#### Setting the start of the fiscal year

You also have the option to select the start of the fiscal year while copying the dates. Click 'Change fiscal year start' to choose.

<figure><img src="../../../.gitbook/assets/image (739).png" alt=""><figcaption><p>Change fiscal year start</p></figcaption></figure>

In the below example, the fiscal year start is set to April 5th. Click **Submit** to insert.

<figure><img src="../../../.gitbook/assets/image (740).png" alt=""><figcaption><p>Fiscal year starting date is changed</p></figcaption></figure>

The date column is inserted with the specified fiscal month and date.

<figure><img src="../../../.gitbook/assets/image (741).png" alt=""><figcaption><p>Date column inserted</p></figcaption></figure>

In the next section, we'll cover the [data input features available only in Inforiver Enterprise](writeback-matrix-features.md).
