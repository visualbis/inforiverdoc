# Multi Select

You can use the multi-select variable to choose multiple options simultaneously from a set of choices.

### 1. Configuration

This section outlines configurations specific to multi-select variables.

<figure><img src="../../../../../.gitbook/assets/image (443).png" alt=""><figcaption><p>Multi select configuration</p></figcaption></figure>

**i) Orientation:** You can choose whether to display the options in a single line(horizontal) or one below the other(vertical). The example shows multi-select options arranged in horizontal and vertical orientations.

<figure><img src="../../../../../.gitbook/assets/image (444).png" alt=""><figcaption><p>Multiselect orientation</p></figcaption></figure>

**ii) Options:** You can create the options in two ways - manually enter each option or source the options from a dimension in your dataset. [Refer to the configuration for single select to know more about options.](single-select.md#ii-options)

**iii) Default selection:** If you want an option to be selected by default, you can choose from the list of values.

<figure><img src="../../../../../.gitbook/assets/image (488).png" alt=""><figcaption><p>Default category selection</p></figcaption></figure>

**iv) Select style:** Inforiver provides the flexibility to change the look and feel of a component with several built-in styles.

<figure><img src="../../../../../.gitbook/assets/image (489).png" alt=""><figcaption><p>Styles for multi select</p></figcaption></figure>

### 2. Examples

#### 2.1. Filter data using multi-select

{% hint style="info" %}
To instantly create a filter driven by multi-select options, navigate to Insert Variable> Filter using Single/Multiselect. Select the dimension category to use in the filter.
{% endhint %}

**STEP 1:** Create a multi-select variable, and assign the options to use in the filter. &#x20;

<figure><img src="../../../../../.gitbook/assets/image (490).png" alt=""><figcaption><p>Creating a multi-select variable</p></figcaption></figure>

**STEP 2:** Create an Inforiver filter that references the multi-select variable.

<figure><img src="../../../../../.gitbook/assets/image (491).png" alt=""><figcaption><p>Create a filter referencing the variable</p></figcaption></figure>

**STEP 3:** Use the multi-select to easily apply filters to your data.

<figure><img src="../../../../../.gitbook/assets/image (492).png" alt=""><figcaption><p>Filter using multi-select</p></figcaption></figure>
