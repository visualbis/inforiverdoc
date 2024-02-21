# Single Select

You can use the single select variable to choose one option from a set of choices.

### 1. Configuration

This section outlines configurations specific to single select variables.

#### **i) Orientation**

You can choose whether to display the options in a single line(horizontal) or one below the other(vertical).

<figure><img src="../../../../../.gitbook/assets/image (482).png" alt=""><figcaption><p>Orientation option for single select</p></figcaption></figure>

The example shows single select options arranged in horizontal and vertical orientations.

<figure><img src="../../../../../.gitbook/assets/image (480).png" alt=""><figcaption><p>Horizontal and vertical orientation for single select</p></figcaption></figure>

#### **ii) Options**

You can create the options in two ways - either manually enter each of the options or source the options from a dimension in your dataset.

<figure><img src="../../../../../.gitbook/assets/image (483).png" alt=""><figcaption><p>Entering options for single select</p></figcaption></figure>

* **New List**

When you click on the New List button, textboxes will be enabled to key in the options. If you have more than 3 options, you can click on the 'Add option' link to enter additional values.

<figure><img src="../../../../../.gitbook/assets/image (485).png" alt=""><figcaption><p>Manually entering options</p></figcaption></figure>

You can assign user-defined values for each of the options by enabling the 'Assign values' toggle.

<figure><img src="../../../../../.gitbook/assets/image (486).png" alt=""><figcaption><p>Assigning values to variables</p></figcaption></figure>

When you reference the variable in the formula, the assigned value will be used. In the example, the assigned value of 3 is used when Option 3 is selected.

<figure><img src="../../../../../.gitbook/assets/image (478).png" alt=""><figcaption><p>Referencing assigned values for options</p></figcaption></figure>

* **Datasets**

You can source the options for the single select widget from your datasets. You just need to select the dimension name from the dropdown - the distinct values in the chosen dimension will be displayed as options.

<figure><img src="../../../../../.gitbook/assets/image (430).png" alt=""><figcaption><p>Selecting a dimension to populate options</p></figcaption></figure>

#### **iii) Default selection**

If you want an option to be selected by default, you can choose from the list of values.

<figure><img src="../../../../../.gitbook/assets/image (431).png" alt=""><figcaption><p>Setting a default option</p></figcaption></figure>

#### **iv) Select style**

Inforiver provides the flexibility to change the look and feel of a component with several built-in styles.

<figure><img src="../../../../../.gitbook/assets/image (432).png" alt=""><figcaption><p>Set the style of the single select widget</p></figcaption></figure>

### 2. Examples

#### 2.1. Filtering data using single select

STEP 1: Create single select variables from the dataset for year and quarter - values from the dataset will be used to populate the options.

<figure><img src="../../../../../.gitbook/assets/image (434).png" alt=""><figcaption><p>Creating single select for quarter</p></figcaption></figure>

STEP 2: Create filters on year and quarter using the single select variables.

<figure><img src="../../../../../.gitbook/assets/image (435).png" alt=""><figcaption><p>Creating filters based on single select variables</p></figcaption></figure>

STEP 3: The data is dynamically filtered based on the options selected.

<figure><img src="../../../../../.gitbook/assets/image (436).png" alt=""><figcaption><p>Single select variables for data filtering</p></figcaption></figure>
