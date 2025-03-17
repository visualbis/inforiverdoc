# Dropdown

Inforiver provides options to create single-select or multi-select lists on your own, use one of the preset options or create from your Power BI datasets.&#x20;

{% embed url="https://vimeo.com/897085316" %}
Dropdowns - overview
{% endembed %}

The single-select and multi-select columns have two main differences:

1. The obvious one is that a single-select column accepts only one option as input whereas, the multi-select column doesn't have that restriction.
2. There are presets available for creating a list of values in the case of the single-select column whereas the same is not available for multi-select columns.

In this section, we'll cover single-select columns. The same steps can be followed for multi-select except for the two points mentioned above.

{% hint style="info" %}
If you are using Inforiver Writeback Matrix, you need to [sign in](../../insert-manual-input-columns.md#1.-sign-in) to start inserting a dropdown column.
{% endhint %}

Click on the 'Single Select' option in the dropdown.

<figure><img src="../../../../.gitbook/assets/image (7) (11).png" alt=""><figcaption><p>Data Input type - Single Select</p></figcaption></figure>

{% hint style="info" %}
Some of the properties such as [Insert as Visual measure/column](../../insert-manual-input-columns.md#1.-insert-as) and [Allow input](../../insert-manual-input-columns.md#2.-allow-input) are covered in earlier sections.
{% endhint %}

## 1. Creating a list of values

There are two ways to create a list of values (LOVs) in Inforiver Reporting Matrix. The third option - Semantic model - which is greyed out is available only in Inforiver Writeback Matrix and is covered in the [next section](dropdown-options-from-semantic-models.md).

<figure><img src="../../../../.gitbook/assets/image (517) (2).png" alt=""><figcaption><p>Creating a list of values</p></figcaption></figure>

### a) List

On clicking 'List', three default options along with colors are displayed. You can rename the options as required and click **Create** to create a new list with three options.

<figure><img src="../../../../.gitbook/assets/image (518) (2).png" alt=""><figcaption><p>New list created with three options</p></figcaption></figure>

### b) Presets&#x20;

On clicking 'Presets', a pop-up screen opens. The list of values for each preset can be seen on hover. Select the required preset and Click **Apply.**&#x20;

<figure><img src="../../../../.gitbook/assets/image (519) (2).png" alt=""><figcaption><p>Using a preset list of values</p></figcaption></figure>

The list of values that gets created is shown below.

<figure><img src="../../../../.gitbook/assets/4.4.2.4 Select.png" alt=""><figcaption><p>List of values from presets</p></figcaption></figure>

### c) Text columns(For Inforiver Writeback Matrix only)

Inforiver allows you to source dropdown values from [text data input columns](../text-checkbox-and-date.md#1.-text) belonging to a different visual. The visual ID is required to reference a different visual. You can obtain the visual ID from the profile as shown in the image below.

<figure><img src="../../../../.gitbook/assets/image (286).png" alt=""><figcaption><p>Text data input column in a different visual</p></figcaption></figure>

Follow the steps below to reference the values from one visual in another visual:

**STEP 1:** Copy the visual ID from visual 1 (Regional Sales).

**STEP 2:** Create a single-select or multi-select dropdown field in visual 2 (Product Sales).

**STEP 3:** In the _Advanced_ section of the single select in visual 2 (Product Sales), enter the visual ID from step 1. Once the visual ID is entered, you will be able to select the text column(Region Entity) from the _Column_ dropdown under the _Advanced_ section.

<figure><img src="../../../../.gitbook/assets/image (287).png" alt=""><figcaption><p>Select text column from another visual</p></figcaption></figure>

Notice how the values in the single select are being populated from the Regional Sales visual.

<figure><img src="../../../../.gitbook/assets/image (288).png" alt=""><figcaption><p>Region values are sourced from the Regional Sales visual</p></figcaption></figure>

### d) Localization settings

For organizations with a global presence, Inforiver allows you to provide translation support for users in their native language. [Learn more about localization settings.](../../../../display-settings/general-settings.md#id-9.-localization-settings)

You can configure and display the dropdown options based on the current language settings in Power BI. Navigate to Display Settings > General > Localization Settings to create necessary translation entries.

<figure><img src="../../../../.gitbook/assets/image (1) (1) (1) (1) (1) (2) (1) (1) (1).png" alt=""><figcaption><p>Localization settings</p></figcaption></figure>

You can use the GETLOCALELABEL function to retrieve the dropdown options and the column title in the language that the report consumer has selected. In the example, the locale is set to French and the options automatically are translated into French.

<figure><img src="../../../../.gitbook/assets/image (1) (1) (1) (1) (1) (2) (1) (1) (1) (1).png" alt=""><figcaption><p>GETLOCALELABEL function for single select</p></figcaption></figure>

## 2. Editing the LOVs

Changes to data input columns can be achieved using the 'Manage' option in the toolbar.

<figure><img src="../../../../.gitbook/assets/4.4.2.10 Edit options.png" alt=""><figcaption><p>Manage inserted data input column</p></figcaption></figure>

The data input side panel opens up. You can make the changes as desired.

<figure><img src="../../../../.gitbook/assets/4.4.2.11 Edit options.png" alt=""><figcaption><p>Editing properties</p></figcaption></figure>

#### Editing the options

The names, order, and color of the options can be modified and they can be added or deleted as well. To edit the names, type over the existing names in the text boxes.

<figure><img src="../../../../.gitbook/assets/4.4.2.2 Edit options.png" alt=""><figcaption><p>Editing the names</p></figcaption></figure>

#### Adding new options

To create a new option, click on the 'Add option'. Type the name in the text box and click 'Enter'. The option gets created as shown below.

<div><figure><img src="../../../../.gitbook/assets/4.4.2.3 Edit options.png" alt=""><figcaption><p>Add an option</p></figcaption></figure> <figure><img src="../../../../.gitbook/assets/4.4.2.4 Edit options.png" alt=""><figcaption><p>Enter the name</p></figcaption></figure> <figure><img src="../../../../.gitbook/assets/4.4.2.5 Edit options.png" alt=""><figcaption><p>Option created</p></figcaption></figure></div>

#### Changing the color associated with each option

To change the color, click on the color dropdown. A color picker opens. Choose a color as desired.

<figure><img src="../../../../.gitbook/assets/4.4.2.6 Edit options.png" alt=""><figcaption><p>Changing the color</p></figcaption></figure>

To reorder or delete options, use the highlighted icons.

<figure><img src="../../../../.gitbook/assets/4.4.2.7 Edit options.png" alt=""><figcaption><p>Reordering or deleting options</p></figcaption></figure>

#### Icon position

This option allows you to hide or display the icon in the options to the left or right of data.

<figure><img src="../../../../.gitbook/assets/image (755).png" alt=""><figcaption><p>Icon position in the options</p></figcaption></figure>

## 3. Options Style

This option lets you choose your desired display style for single and multi-select dropdowns: Chip, Arrow, or Plain text.

<figure><img src="../../../../.gitbook/assets/image (883) (1).png" alt=""><figcaption><p>Options Style</p></figcaption></figure>

In the image below, we used the plain-text style for the multi-select dropdown, whereas, for the single-select, we’ve used the chip and arrow styles.

<figure><img src="../../../../.gitbook/assets/display style for dropdown.png" alt=""><figcaption><p>Example for chip, arrow and plain text styles</p></figcaption></figure>

## 4. Allow user to add new option

Enabling this option allows users to [create new options dynamically](./#id-5.-dynamically-adding-missing-options) while using the dropdown, without the need to open the side panel for adding options.

<figure><img src="../../../../.gitbook/assets/image (756).png" alt=""><figcaption><p>Allow user to add new option</p></figcaption></figure>

## 5. Entry in total/subtotal rows

By default, data can be entered in total/subtotal rows. To disable it, uncheck the checkbox highlighted in the below image.

<figure><img src="../../../../.gitbook/assets/4.4.2.8 Edit options.png" alt=""><figcaption><p>Disabling input in total/subtotal rows</p></figcaption></figure>

On trying to select an option in the total/subtotal row, a message as shown in the image is displayed.

<figure><img src="../../../../.gitbook/assets/4.4.2.8 Select.png" alt=""><figcaption><p>Entry disabled in total/subtotal rows</p></figcaption></figure>

## 6. Default Value

When you create a single-select data input field, you can specify a default choice to avoid blanks in your reports.

**Static**: When you use the static option, you can select the relevant default value from the Value dropdown. In this report, we’ve chosen the ‘Approval Status’ preset. Notice how the Value dropdown for default values contains options relevant to approval status. Even if you specify custom options with the Lists, Inforiver will populate the manually entered options in the default value dropdown.

<figure><img src="../../../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Static default value</p></figcaption></figure>

**Dimension**: You can choose to set a dimension category as the default value. Please be mindful that if you choose to source default values from a dimension, you will need to enable the **Allow user to add new option** checkbox.

<figure><img src="../../../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Default values from a dimension</p></figcaption></figure>

**Measure**: You can choose to set a measure as the default value. Please be mindful that if you choose to source default values from a measure, you will need to enable the **Allow user to add new option** checkbox.

<figure><img src="../../../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Default options from a measure</p></figcaption></figure>

## 7. Using the dropdown

Once the necessary changes are made to the list of values, and other properties are configured, click 'Create' in the data input side panel. Click on a cell in the data input column to enable the dropdown and choose an option.

<figure><img src="../../../../.gitbook/assets/4.4.2.5 Select.png" alt=""><figcaption><p>Selecting from the dropdown</p></figcaption></figure>

## 8. Dynamically adding missing options

Users can create a new option on the fly if a particular option is not available in LOV. In the example below, the available values are ‘Submitted’, ‘In Review’, and ‘Approved’.

<figure><img src="../../../../.gitbook/assets/image (140) (1).png" alt=""><figcaption><p>Available options in the LOV</p></figcaption></figure>

To add a new value of ‘Rejected’, type the new value in the search bar and click on the ‘Create’ button.

{% hint style="info" %}
To allow users to input custom options, the **Allow user to add new option** should be enabled in the Single-Select/Multi-Select configuration.
{% endhint %}

<figure><img src="../../../../.gitbook/assets/image (141) (1).png" alt=""><figcaption><p>Adding a new value to a LOV</p></figcaption></figure>

The new value gets added to the list.

<figure><img src="../../../../.gitbook/assets/image (142) (1).png" alt=""><figcaption><p>New value added to the LOV</p></figcaption></figure>



In the next section, we'll cover other data input types such as [text, checkbox, and date](../text-checkbox-and-date.md).
