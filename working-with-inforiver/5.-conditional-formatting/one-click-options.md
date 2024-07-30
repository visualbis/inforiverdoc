# One-click options

With Inforiver, you can perform various conditional formatting actions in a single click. Options include semantic formatting, color scales, segmentation, icons, ratings, data bars and many more.

A big benefit of the one-click setting is that you do not need to create rules from scratch. After you create a quick rule, you will have the option to customize it in a detailed manner if your report requires it.

### 1. Quick rule

Quick rule allows you to highlight the positive and negative values in the visual in a single click. Under 'Quick rule', there are two options - 'Positive' and 'Negative'.

<figure><img src="../../.gitbook/assets/5.1.2 Quick rule.png" alt=""><figcaption><p>Quick rule</p></figcaption></figure>

{% hint style="info" %}
The one-click conditional formatting options are enabled only if a cell/column is selected.
{% endhint %}

a) Select a column. You can highlight values greater than or equal to zero in green by clicking on the 'Positive' option. &#x20;

<figure><img src="../../.gitbook/assets/5.1.3 Quick rule.png" alt=""><figcaption><p>Highlight positive values</p></figcaption></figure>

b) Similarly, you can highlight values lesser than or equal to zero in red by clicking on the 'Negative' option.&#x20;

<figure><img src="../../.gitbook/assets/5.1.5 Quick rule.png" alt=""><figcaption><p>Highlight negative values</p></figcaption></figure>

### 2. Color scales

A wide variety of color scales such as sequential, qualitative, diverging, continuous and continuous-diverging can be applied in a single click.&#x20;

a) Choose any column or cell and click on Conditional Formatting -> Color scales. Choose any of the color scales shown.

<figure><img src="../../.gitbook/assets/5.1.6 Color scales.png" alt=""><figcaption><p>Color scales</p></figcaption></figure>

b) A sample heatmap using the sequential color scale is shown below. Notice that the font colors are automatically adjusted to be in contrast with their backgrounds for enhanced readability.

<figure><img src="../../.gitbook/assets/5.1.8 Color scales (1).png" alt=""><figcaption><p>Sequential color scale</p></figcaption></figure>

To learn more about customizing color scales, visit [this section](color-scale.md).

### 3. Classification

You can apply conditional formatting based on icons/ratings and even deliver ABC segmentations in a single click. As you click on 'Classification', you can see the following options.&#x20;

<figure><img src="../../.gitbook/assets/Classification (1).png" alt=""><figcaption><p>Classification</p></figcaption></figure>

Let's look at an example for the three categories - Text, Icon set, and Rating.

**3.1.** **Text**: Text-based classification is commonly used to categorize performance. A sample report with ABC classification is shown in the below image.

<figure><img src="../../.gitbook/assets/Text Classification (1).png" alt=""><figcaption><p>ABC classification</p></figcaption></figure>

**3.2.** **Icons**: You can deliver conditional formatting using icons in a few clicks. Here is an example where items that contribute the most to sales are highlighted.

<figure><img src="../../.gitbook/assets/5.1.9 Classification.png" alt=""><figcaption><p>Icon-based conditional formatting</p></figcaption></figure>

**3.3.** **Ratings**: You can use ratings such as the star-based ratings commonly seen in e-commerce sites in the product feedback section.&#x20;

<figure><img src="../../.gitbook/assets/5.1.10 Classification.png" alt=""><figcaption><p>Star-based ratings</p></figcaption></figure>

To learn more about customizing classifications, visit [this section](classification.md).

### 4. Data bars

Data bars can be used to insert colored bars inside a cell to show how a given cell value compares to others.&#x20;

a) On clicking 'Data bars', you can see the following options. Select any of the options.

<figure><img src="../../.gitbook/assets/5.6.2 Data bars.png" alt=""><figcaption><p>Data bars</p></figcaption></figure>

b) Data bars get added as shown in the image making it easy to spot the highest and lowest values at a glance.

<figure><img src="../../.gitbook/assets/5.6.3 Data bars.png" alt=""><figcaption><p>Data bars</p></figcaption></figure>

To learn more about customizing data bars, visit [this section](color-scale.md#2.-data-bars).

### 5. Action Analysis

#### a) Action dot

Action dots represent the degree to which the cell values deviate from the desired range/value in the measure. Adding them to the cells helps you assess how the quantities compare to the middle value or any desired value in the measure.&#x20;

1. Select any measure to which you want to add them. Click **Conditional Formatting -> Action Analysis -> Action Dot.**

<figure><img src="../../.gitbook/assets/image (511).png" alt=""><figcaption><p>Action Dot</p></figcaption></figure>

2. By default, Inforiver provides custom color ranges based on values or percentages. Click **Apply.** Find below a sample report with action dots applied to the _Profit_ measure.

<figure><img src="../../.gitbook/assets/image (512).png" alt=""><figcaption><p>Action dots applied to <em>Profit</em></p></figcaption></figure>

The color scale indicates a positive or negative deviation, and the number of dots represents the magnitude of the difference, with which you can focus on the values that diverge the most.

#### b) Action Color

Action colors are a variation of action dots in which the degree of divergence of cell values from the target value is expressed by color gradients. The color scale denotes a positive or negative deviation, while the gradient intensity indicates the magnitude of the deviation.

1. Select any measure to which you want to add them. Click **Conditional Formatting -> Action Analysis -> Action Color.**

<figure><img src="../../.gitbook/assets/image (513).png" alt=""><figcaption><p>Action Color</p></figcaption></figure>

2. By default, Inforiver provides custom color ranges based on values or percentages. Click **Apply.** Find below a sample report with action colors applied to the _Profit_ measure.

<figure><img src="../../.gitbook/assets/image (514).png" alt=""><figcaption><p>Action Colors applied to the <em>Profit</em></p></figcaption></figure>

The conditional formatting side panel provides options to customize the action dots and action colors. The options are similar to the color scale, data bars, and classification which are explained [here](color-scale.md#c-custom-color-scale) and [here](classification.md#classification-ranges). The **middle percentage** option is used to set the desired median percentage value from which the spread is calculated.

### 6. Bubble charts

You can use bubble charts to gauge the magnitude of a measure instantly and for quick comparative analysis.&#x20;

<figure><img src="../../.gitbook/assets/image (508).png" alt=""><figcaption><p>Bubble chart conditional formatting</p></figcaption></figure>

The bubble size can be determined by comparing values in the same column or within the same row. You can also use a different measure to determine the size of the bubble.

<figure><img src="../../.gitbook/assets/image (509).png" alt=""><figcaption><p>Bubble charts</p></figcaption></figure>



You can use the side panel to customize your rules. In the next section, we'll look at the [advanced options](create-rule-basic-settings.md).
