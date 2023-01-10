# Color scale

Another commonly used type of conditional formatting is the 'color scale,' which applies a gradient fill to a range of cells based on their values. This is a useful way to quickly visualize and compare values in a table. Color scale can be applied for the background, font color or data bars. It can also be applied row-wise, column-wise, or table-wise.

Refer to [create rule](./) to get started. Once the rule is created and you can see the 'Conditional formatting' side panel, follow the below steps.

Choose 'Color scale' in the '**Format by**' dropdown. There are several options enabled as shown in the below image.

<figure><img src="../../../.gitbook/assets/5.3.1 Color scale.png" alt=""><figcaption><p>Choosing color scale</p></figcaption></figure>

Let's go with the default. Click 'Apply'.

<figure><img src="../../../.gitbook/assets/5.3.3 Color scale.png" alt=""><figcaption><p>Basic color scale</p></figcaption></figure>

### 1. Based on

a) Let's now apply formatting for 2021 Actuals based on the absolute variance between AC and PL. Select '2021 Actuals - 2021 Plan' from the 'Based on' dropdown. Click 'Apply'.&#x20;

<figure><img src="../../../.gitbook/assets/5.3.4 Color scale.png" alt=""><figcaption><p>Conditional formatting based on a different measure</p></figcaption></figure>

b) Let's hide the 2021 Plan column and show the variance column. Click on 'Manage columns' and check/uncheck the checkboxes as highlighted.

<figure><img src="../../../.gitbook/assets/5.3.5 Color scale.png" alt=""><figcaption><p>Enabling the 2021 Actuals - 2021 Plan column</p></figcaption></figure>

c) You can see that the color scale has been updated to highlight values based on the variance. For eg., even though East -> Tea & coffee is 3.75m, the formatting is dark blue because of the high variance of +3.99m.

<figure><img src="../../../.gitbook/assets/5.3.6 Color scale.png" alt=""><figcaption><p>Conditional formatting for 2021 Actuals based on absolute variance AC vs PL</p></figcaption></figure>

### 2. Color scale for

a) Let's now apply color scale for font. Select 'Font' in the 'Color scale for' dropdown. Click 'Apply'.

<figure><img src="../../../.gitbook/assets/5.3.19 Color scale.png" alt=""><figcaption><p>Color scale for font</p></figcaption></figure>

b) You can see that the font for 2021 Actuals is formatted sequentially based on the variance.

<figure><img src="../../../.gitbook/assets/5.3.8 Color scale.png" alt=""><figcaption><p>Color scale for font</p></figcaption></figure>

c) Let's choose the third option - Data bars in the 'Color scale for' dropdown. Click 'Apply'. The data bars are formatted as shown below.

<figure><img src="../../../.gitbook/assets/5.3.9 Color scale.png" alt=""><figcaption><p>Color scale for data bars</p></figcaption></figure>

d) Let's revert back to background formatting based on 2021 Actuals.&#x20;

<figure><img src="../../../.gitbook/assets/5.3.10 Color scale.png" alt=""><figcaption><p>Background formatting</p></figcaption></figure>

### 3. Heat map type

a) Notice that the formatting is applied column-wise. That is the maximum and minimum values in a column are formatted using the darkest and lightest gradients.&#x20;

<figure><img src="../../../.gitbook/assets/5.3.14 Color scale.png" alt=""><figcaption><p>Column wise formatting</p></figcaption></figure>

b) Also, notice the value of East -> Soda across quarters. The highlighted values are around 15m, but for Q4 it is a darker gradient compared to the first two quarters. This is because of the column-wise formatting.

<figure><img src="../../../.gitbook/assets/5.3.15 Color scale.png" alt=""><figcaption><p>Column wise formatting</p></figcaption></figure>

c) Let's now apply row-wise formatting. Select 'Row wise' in the 'Heat map type' dropdown and click 'Apply'. You can see that the maximum and minimum values in a row are formatted using the darkest and lightest gradients.

<figure><img src="../../../.gitbook/assets/5.3.12 Color scale.png" alt=""><figcaption><p>Row wise formatting</p></figcaption></figure>

d) Also, notice the highlighted values in Q1. East -> Mineral water(16m) which is greater than Pacific -> Soda (10m) but is formatted using a lighter gradient. And East -> Juices and Pacific -> Soda are formatted using the same gradient even though there is a huge difference. This is because of the row-wise formatting.

<figure><img src="../../../.gitbook/assets/5.3.13 Color scale.png" alt=""><figcaption><p>Row wise formatting</p></figcaption></figure>

e) The below image shows table-wise formatting. Notice that similar values are formatted using the same gradient throughout the table.

<figure><img src="../../../.gitbook/assets/5.3.16 Color scale.png" alt=""><figcaption><p>Table wise formatting</p></figcaption></figure>

### 4. Color scale type

There are a number of types such as Sequential, Diverging, Qualitative, Continuous, etc. You can click on the 'Color scale type' dropdown to see the entire list.

a) Let's apply a 'Diverging' color scale. Select from the dropdown and click 'Apply'.

<figure><img src="../../../.gitbook/assets/5.3.18 Color scale.png" alt=""><figcaption><p>Color scale types</p></figcaption></figure>

b) You can see that the backgrounds are formatted using the Diverging scale.

<figure><img src="../../../.gitbook/assets/5.3.20 Color scale.png" alt=""><figcaption><p>Diverging color scale</p></figcaption></figure>

c) Below is an example where the Continuous-Range scale is used.

<figure><img src="../../../.gitbook/assets/5.3.22 Color scale.png" alt=""><figcaption><p>Continuous-Range scale</p></figcaption></figure>

### &#x20;5. Color scheme

a) For color scale of types Sequential, Diverging, Diverging-color safe, Qualitative and Qualitative-color safe, there are several default color schemes to choose from. You can click on the 'Color scheme' dropdown and choose the desired color scheme.

<figure><img src="../../../.gitbook/assets/5.3.23 Color scale.png" alt=""><figcaption><p>Color schemes</p></figcaption></figure>

b) For color scale of types Continuous-Range, Continuous-Diverging Range, Continuous and Continuous-Diverging, you can define the min/max colors and center color if applicable.

<figure><img src="../../../.gitbook/assets/5.3.24 Color scale.png" alt=""><figcaption><p>Color selection</p></figcaption></figure>

c) The 'Custom' color scale type can be used to define custom color ranges based on value or percentage. On selecting the custom option, you can see the fields highlighted in the below image. You can define the values/percentages for the ranges, add or delete ranges, define colors and reverse the order. Changes can also be reset to default.

<figure><img src="../../../.gitbook/assets/5.3.31 Color scale.png" alt=""><figcaption><p>Custom color scheme</p></figcaption></figure>

d) Color scale can be reversed for cases where the minimum and maximum values need to be denoted with the highest and lowest gradients. To achieve this, check the '**Reverse color**' checkbox.

<figure><img src="../../../.gitbook/assets/5.3.26 Color scale.png" alt=""><figcaption><p>Reversing color scale</p></figcaption></figure>

e) By default, the number of bands is defined as 5. But it can be increased or decreased using the '**Number of bands**' field. The color scheme field also gets updated to show the gradients.

<figure><img src="../../../.gitbook/assets/5.3.27 Color scale.png" alt=""><figcaption><p>Number of bands</p></figcaption></figure>

f) You can choose to show only the color scale and hide the values. To do this, check the '**Hide value**' checkbox.

<figure><img src="../../../.gitbook/assets/5.3.28 Color scale.png" alt=""><figcaption><p>Hiding values</p></figcaption></figure>

g) When you apply background conditional formatting in Inforiver, the font colors are automatically adjusted to be in contrast with their backgrounds to enhance readability. But it can be turned off if not required by unchecking the '**Auto font color**' checkbox.&#x20;

<figure><img src="../../../.gitbook/assets/5.3.29 Color scale.png" alt=""><figcaption><p>Auto font color disabled</p></figcaption></figure>

h) In cases where there are null values in your table, you can choose whether to include or exclude them from conditional formatting. In the below image, the 2022 Forecast for Pacific is empty. To show conditional formatting for Pacific as well, check the '**Include null**' checkbox.

<figure><img src="../../../.gitbook/assets/5.3.30 Color scale.png" alt=""><figcaption><p>Conditional formatting for null values</p></figcaption></figure>

In the next section, we'll take a look at [Classification](classification.md).
