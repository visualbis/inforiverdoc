# Color scale & data bars

Another commonly used type of conditional formatting is the 'color scale,' which applies a gradient fill to a range of cells based on their values. This is a useful way to quickly visualize and compare values in a table. Color scale can be applied for the background, font color or data bars. It can also be applied row-wise, column-wise, or table-wise.

Refer to [create rule](create-rule-basic-settings.md) to get started. Once the rule is created and you can see the 'Conditional formatting' side panel, follow the below steps.

Choose 'Color scale' in the 'Format by' dropdown. There are several options enabled as shown in the below image.

<figure><img src="../../.gitbook/assets/5.3.1 Color scale.png" alt=""><figcaption><p>Choosing color scale</p></figcaption></figure>

## 1. Font/Background

Let's go with the default. Click 'Apply'.

<figure><img src="../../.gitbook/assets/5.3.3 Color scale.png" alt=""><figcaption><p>Basic color scale</p></figcaption></figure>

### i. Based on

a) Let's now apply formatting for 2021 Actuals based on the absolute variance between AC and PL. Select '2021 Actuals - 2021 Plan' from the 'Based on' dropdown. Click 'Apply'.&#x20;

<figure><img src="../../.gitbook/assets/5.3.4 Color scale.png" alt=""><figcaption><p>Conditional formatting based on a different measure</p></figcaption></figure>

b) Let's hide the 2021 Plan column and show the variance column. Click on 'Manage columns' and check/uncheck the checkboxes as highlighted.

<figure><img src="../../.gitbook/assets/5.3.5 Color scale.png" alt=""><figcaption><p>Enabling the 2021 Actuals - 2021 Plan column</p></figcaption></figure>

c) You can see that the color scale has been updated to highlight values based on the variance. For eg., even though East -> Tea & coffee is 3.75m, the formatting is dark blue because of the high variance of +3.99m.

<figure><img src="../../.gitbook/assets/5.3.6 Color scale.png" alt=""><figcaption><p>Conditional formatting for 2021 Actuals based on absolute variance AC vs PL</p></figcaption></figure>

### ii. Color scale for

a) Let's now apply color scale for font. Select 'Font' in the 'Color scale for' dropdown. Click 'Apply'.

<figure><img src="../../.gitbook/assets/5.3.19 Color scale.png" alt=""><figcaption><p>Color scale for font</p></figcaption></figure>

b) You can see that the font for 2021 Actuals is formatted sequentially based on the variance.

<figure><img src="../../.gitbook/assets/5.3.8 Color scale.png" alt=""><figcaption><p>Color scale for font</p></figcaption></figure>

c) Let's revert back to background formatting based on 2021 Actuals. Data bars are covered in the [next section](color-scale.md#2.-data-bars).

<figure><img src="../../.gitbook/assets/5.3.10 Color scale.png" alt=""><figcaption><p>Background formatting</p></figcaption></figure>

### iii. Heat map type

a) Notice that the formatting is applied column-wise. That is the maximum and minimum values in a column are formatted using the darkest and lightest gradients.&#x20;

<figure><img src="../../.gitbook/assets/5.3.14 Color scale.png" alt=""><figcaption><p>Column wise formatting</p></figcaption></figure>

b) Also, notice the value of East -> Soda across quarters. The highlighted values are around 15m, but for Q4 it is a darker gradient compared to the first two quarters. This is because of the column-wise formatting.

<figure><img src="../../.gitbook/assets/5.3.15 Color scale.png" alt=""><figcaption><p>Column wise formatting</p></figcaption></figure>

c) Let's now apply row-wise formatting. Select 'Row wise' in the 'Heat map type' dropdown and click 'Apply'. You can see that the maximum and minimum values in a row are formatted using the darkest and lightest gradients.

<figure><img src="../../.gitbook/assets/5.3.12 Color scale.png" alt=""><figcaption><p>Row wise formatting</p></figcaption></figure>

d) Also, notice the highlighted values in Q1. East -> Mineral water(16m) is greater than Pacific -> Soda (10m) but is formatted using a lighter gradient. And East -> Juices and Pacific -> Soda are formatted using the same gradient even though there is a huge difference. This is because of the row-wise formatting.

<figure><img src="../../.gitbook/assets/5.3.13 Color scale.png" alt=""><figcaption><p>Row wise formatting</p></figcaption></figure>

e) The below image shows table-wise formatting. Notice that similar values are formatted using the same gradient throughout the table.

<figure><img src="../../.gitbook/assets/5.3.16 Color scale.png" alt=""><figcaption><p>Table wise formatting</p></figcaption></figure>

### iv. Color scale type

There are a number of types such as Sequential, Diverging, Qualitative, Continuous, etc. You can click on the 'Color scale type' dropdown to see the entire list.

a) Let's apply a 'Diverging' color scale. Select from the dropdown and click 'Apply'.

<figure><img src="../../.gitbook/assets/5.3.18 Color scale.png" alt=""><figcaption><p>Color scale types</p></figcaption></figure>

b) You can see that the backgrounds are formatted using the Diverging scale.

<figure><img src="../../.gitbook/assets/5.3.20 Color scale.png" alt=""><figcaption><p>Diverging color scale</p></figcaption></figure>

c) Below is an example where the Continuous-Range scale is used.

<figure><img src="../../.gitbook/assets/5.3.22 Color scale.png" alt=""><figcaption><p>Continuous-Range scale</p></figcaption></figure>

### &#x20;v. Colors

#### a) Color scheme

For color scale of types Sequential, Diverging, Diverging-color safe, Qualitative and Qualitative-color safe, there are several default color schemes to choose from. You can click on the 'Color scheme' dropdown and choose the desired color scheme.

<figure><img src="../../.gitbook/assets/5.3.23 Color scale.png" alt=""><figcaption><p>Color schemes</p></figcaption></figure>

#### b) Min/max/center

For color scale of types Continuous-Range, Continuous-Diverging Range, Continuous and Continuous-Diverging, you can define the min/max colors and center color if applicable.

<figure><img src="../../.gitbook/assets/5.3.24 Color scale.png" alt=""><figcaption><p>Color selection</p></figcaption></figure>

#### c) Custom color scale

The 'Custom' color scale type can be used to define custom color ranges based on value or percentage. On selecting the custom option, you can see the fields highlighted in the below image. You can define the values/percentages for the ranges, add or delete ranges, define colors and reverse the order. Changes can also be reset to default.

<figure><img src="../../.gitbook/assets/5.3.31 Color scale.png" alt=""><figcaption><p>Custom color scheme</p></figcaption></figure>

#### d) Reverse color

Color scale can be reversed for cases where the minimum and maximum values need to be denoted with the highest and lowest gradients. To achieve this, check the 'Reverse color' checkbox.

<figure><img src="../../.gitbook/assets/5.3.26 Color scale.png" alt=""><figcaption><p>Reversing color scale</p></figcaption></figure>

#### e) Number of bands

By default, the number of bands is defined as 5. But it can be increased or decreased using the 'Number of bands' field. The color scheme field also gets updated to show the gradients.

<figure><img src="../../.gitbook/assets/5.3.27 Color scale.png" alt=""><figcaption><p>Number of bands</p></figcaption></figure>

#### f) **Hide value**

You can choose to show only the color scale and hide the values. To do this, check the 'Hide value' checkbox.

<figure><img src="../../.gitbook/assets/5.3.28 Color scale.png" alt=""><figcaption><p>Hiding values</p></figcaption></figure>

#### g) **Auto font color**

When you apply background conditional formatting in Inforiver, the font colors are automatically adjusted to be in contrast with their backgrounds to enhance readability. But it can be turned off if not required by unchecking the 'Auto font color' checkbox.&#x20;

<figure><img src="../../.gitbook/assets/5.3.29 Color scale.png" alt=""><figcaption><p>Auto font color disabled</p></figcaption></figure>

#### h) **Include null**

In cases where there are null values in your table, you can choose whether to include or exclude them from conditional formatting. In the below image, the 2022 Forecast for Pacific is empty. To show conditional formatting for Pacific as well, check the 'Include null' checkbox.

<figure><img src="../../.gitbook/assets/5.3.30 Color scale.png" alt=""><figcaption><p>Conditional formatting for null values</p></figcaption></figure>

## 2. Data bars

In the previous section, we covered color scales for fonts and backgrounds. In this section, we'll look at data bars. Note that you can either create a new rule as shown here or edit the data bars inserted using the one-click option explained [here](one-click-options.md#4.-data-bars).

a) Select 'Data bars' in the 'Color scale for' dropdown.&#x20;

<figure><img src="../../.gitbook/assets/5.6.4 Data bars.png" alt=""><figcaption><p>Selecting color scale for data bars</p></figcaption></figure>

b) In the side panel, you can see the customization options available.

<figure><img src="../../.gitbook/assets/5.6.5 Data bars.png" alt=""><figcaption><p>Data bar properties</p></figcaption></figure>

c) Let's go with the default settings. Click 'Apply'. The data bar gets added as shown in the below image.

<figure><img src="../../.gitbook/assets/5.6.6 Data bars.png" alt=""><figcaption><p>Data bar added for 2021 Actuals</p></figcaption></figure>

d) Let's now look at each of the customization options. Check the 'Hide value' checkbox and click 'Apply'. You can now see only the data bars and the values are hidden.

<figure><img src="../../.gitbook/assets/5.6.7 Data bars.png" alt=""><figcaption><p>Hiding the values</p></figcaption></figure>

e) By default, the data bars are applied to all the values (values and totals if selected in the row hierarchy levels). If you only want to use data bars for a particular range of values, you can enter a minimum and maximum value as shown in the below image. Data bars are enabled only for values between 8m and 20m in this case.

<figure><img src="../../.gitbook/assets/5.6.8 Data bars.png" alt=""><figcaption><p>Data bars for a min-max range</p></figcaption></figure>

f) Data bars can be aligned left or right using the 'Alignment' field. Right alignment is shown in this example.

<figure><img src="../../.gitbook/assets/5.6.9 Data bars.png" alt=""><figcaption><p>Data bars alignment</p></figcaption></figure>

g) Note that when there are positive and negative values in the column for which you want to use data bars, the options differ as shown in the below image. You can choose to hide the values and select colors for positive and negative values.

<figure><img src="../../.gitbook/assets/5.6.10 Data bars.png" alt=""><figcaption><p>Data bars for positive and negative values</p></figcaption></figure>

In the next section, we'll take a look at [Classification](classification.md).
