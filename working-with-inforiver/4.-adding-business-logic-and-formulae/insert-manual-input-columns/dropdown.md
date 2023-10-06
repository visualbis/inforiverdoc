# Dropdown

Inforiver provides options to create single-select or multi-select lists on your own, use one of the preset options or create from your Power BI datasets.&#x20;

The single-select and multi-select columns have two main differences:

1. The obvious one is that a single-select column accepts only one option as input whereas, the multi-select column doesn't have that restriction.
2. There are presets available for creating a list of values in the case of the single-select column whereas the same is not available for multi-select columns.

In this section, we'll cover single-select columns. The same steps can be followed for multi-select except for the two points mentioned above.

{% hint style="info" %}
If you are using Inforiver Enterprise, you need to [sign in](../insert-manual-input-columns.md#1.-sign-in) to start inserting a dropdown column.
{% endhint %}

Click on the 'Select' option in the dropdown.

<figure><img src="../../../.gitbook/assets/4.4.2.1 Select.png" alt=""><figcaption><p>Input type - Select</p></figcaption></figure>

{% hint style="info" %}
Some of the properties such as [Insert as Visual measure/column](../insert-manual-input-columns.md#1.-insert-as) and [Allow input](../insert-manual-input-columns.md#2.-allow-input) are covered in earlier sections.
{% endhint %}

## i) Creating a list of values

There are two ways to create a list of values (LOVs) in Inforiver Matrix. The third option - Datasets - which is greyed out is available only in Inforiver Enterprise and is covered in a [later section](enterprise-features.md).

<figure><img src="../../../.gitbook/assets/4.4.2.2 Select.png" alt=""><figcaption><p>Creating list of values</p></figcaption></figure>

### a) New list

On clicking a 'New list', three default options along with colors are displayed.

<figure><img src="../../../.gitbook/assets/4.4.2.1 New list.png" alt=""><figcaption><p>New list created</p></figcaption></figure>

### b) Presets&#x20;

On clicking 'Presets', a pop-up screen opens. The list of values for each preset can be seen on hover. Select the required preset and Click 'Apply'.

<figure><img src="../../../.gitbook/assets/4.4.2.3(2) Select.png" alt=""><figcaption><p>Using a preset</p></figcaption></figure>

The list of values that gets created is shown below.

<figure><img src="../../../.gitbook/assets/4.4.2.4 Select.png" alt=""><figcaption><p>List of values from presets</p></figcaption></figure>

### c) Text columns(Enterprise only)

Inforiver allows you to source dropdown values from [text data input columns](text-checkbox-and-date.md#1.-text) belonging to a different visual. The visual ID is required to reference a different visual. You can obtain the visual ID from the profile as shown in the image below.

<figure><img src="../../../.gitbook/assets/image (286).png" alt=""><figcaption></figcaption></figure>

Follow the steps below to reference the values from one visual in another visual:

1. Copy the visual ID from visual 1 (Regional Sales).
2. Create a single-select or multi-select dropdown field in visual 2 (Product Sales).
3. In the _Advanced_ section of the single select in visual 2 (Product Sales), enter the visual ID from step 1. Once the visual ID is entered, you will be able to select the text column(Region Entity) from the _Column_ dropdown under the _Advanced_ section.

<figure><img src="../../../.gitbook/assets/image (287).png" alt=""><figcaption></figcaption></figure>

Notice how the values in the single select are being populated from the Regional Sales visual.

<figure><img src="../../../.gitbook/assets/image (288).png" alt=""><figcaption></figcaption></figure>

## ii) Editing the LOVs

The names, order, and color of the options can be modified and they can be added or deleted as well. To edit the names, type over the existing names in the text boxes.

<figure><img src="../../../.gitbook/assets/4.4.2.2 Edit options.png" alt=""><figcaption><p>Editing the names</p></figcaption></figure>

To create a new option, click on the 'Add option'. Type the name in the text box and click 'Enter'. The option gets created as shown below.

<div>

<figure><img src="../../../.gitbook/assets/4.4.2.3 Edit options.png" alt=""><figcaption><p>Add an option</p></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/4.4.2.4 Edit options.png" alt=""><figcaption><p>Enter the name</p></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/4.4.2.5 Edit options.png" alt=""><figcaption><p>Option created</p></figcaption></figure>

</div>

To change the color, click on the color dropdown. A color picker opens. Choose a color as desired.

<figure><img src="../../../.gitbook/assets/4.4.2.6 Edit options.png" alt=""><figcaption><p>Changing the color</p></figcaption></figure>

To reorder or delete options, use the highlighted icons.

<figure><img src="../../../.gitbook/assets/4.4.2.7 Edit options.png" alt=""><figcaption><p>Reordering or deleting options</p></figcaption></figure>

## iii) Entry in total/subtotal rows

By default, data can be entered in total/subtotal rows. To disable it, uncheck the checkbox highlighted in the below image.

<figure><img src="../../../.gitbook/assets/4.4.2.8 Edit options.png" alt=""><figcaption><p>Disabling input in total/subtotal rows</p></figcaption></figure>

On trying to select an option in the total/subtotal row, a message as shown in the image is displayed.

<figure><img src="../../../.gitbook/assets/4.4.2.8 Select.png" alt=""><figcaption><p>Entry disabled in total/subtotal rows</p></figcaption></figure>

## iv) Using the dropdown

Once the necessary changes are made to the list of values, and other properties are configured, click 'Create' in the data input side panel. Click on a cell in the data input column to enable the dropdown and choose an option.

<figure><img src="../../../.gitbook/assets/4.4.2.5 Select.png" alt=""><figcaption><p>Selecting from the dropdown</p></figcaption></figure>

## v) Editing the properties

Changes to data input columns can be achieved using the 'Manage' option in the toolbar.

<figure><img src="../../../.gitbook/assets/4.4.2.10 Edit options.png" alt=""><figcaption><p>Manage inserted data input column</p></figcaption></figure>

The data input side panel opens up. You can make the changes as desired.

<figure><img src="../../../.gitbook/assets/4.4.2.11 Edit options.png" alt=""><figcaption><p>Editing properties</p></figcaption></figure>

If a particular item is not available in the presets or data source, you can create a new option while configuring a list of values. In the example below, the available values are ‘Submitted’, ‘In Review’, and ‘Approved’.

<figure><img src="../../../.gitbook/assets/image (140) (1).png" alt=""><figcaption></figcaption></figure>

To add a new value of ‘Rejected’, type the new value in the search bar and click on the ‘Create’ button.

<figure><img src="../../../.gitbook/assets/image (141) (1).png" alt=""><figcaption><p>Adding a new value to a LOV</p></figcaption></figure>

The new value gets added to the list.

<figure><img src="../../../.gitbook/assets/image (142) (1).png" alt=""><figcaption><p>New value added to the LOV</p></figcaption></figure>



In the next section, we'll be covering other data input types such as [text, checkbox, and date](text-checkbox-and-date.md).
