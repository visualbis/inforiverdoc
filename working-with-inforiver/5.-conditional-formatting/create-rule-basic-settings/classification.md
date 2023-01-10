# Classification

Inforiver provides data classification based on text, icons and ratings.

Refer to [create rule](./) to get started. Once the rule is created and you can see the 'Conditional formatting' side panel, follow the below steps.

Choose 'Classification' in the '**Format by**' dropdown. There are several options enabled as shown in the below image.

<figure><img src="../../../.gitbook/assets/5.4.1 Classification.png" alt=""><figcaption><p>Conditional formatting based on classification</p></figcaption></figure>

Click on the 'Display' dropdown. You can see the three types of classifications already mentioned. Let's look at them one by one.

<figure><img src="../../../.gitbook/assets/5.4.2 Classification.png" alt=""><figcaption><p>Classification types</p></figcaption></figure>

### 1. Text

Many times, it may become essential to categorize performance. A common technique used by enterprises to categorize inventory, vendors or materials is [ABC analysis](https://en.wikipedia.org/wiki/ABC\_analysis). Inforiver delivers this capability right out of the box.&#x20;

a) Select 'ABC' from the 'Display' dropdown. Let's go with the default settings. Click 'Apply'.

<figure><img src="../../../.gitbook/assets/5.4.3 Classification.png" alt=""><figcaption><p>ABC analysis</p></figcaption></figure>

b) The rows are classified and the text is displayed on the left of the data.

<figure><img src="../../../.gitbook/assets/5.4.4 Classification.png" alt=""><figcaption><p>ABC analysis</p></figcaption></figure>

c) You can also have the classifications appear in a separate column if required. Check the '**Show as new column**' checkbox.

<figure><img src="../../../.gitbook/assets/5.4.5 Classification.png" alt=""><figcaption><p>Display text in new column</p></figcaption></figure>

d) When there are charts in the column where classification is to be applied, check the '**Apply to charts**' checkbox. In the below image, 2021 Actuals are visualized using bar charts and the colors defined for the ABC ranges are used for formatting.

<figure><img src="../../../.gitbook/assets/5.4.6 Classification.png" alt=""><figcaption><p>Classification applied to charts</p></figcaption></figure>

e) You can also choose to display only the classification text by clicking on 'Only text' in the '**Text position**' dropdown.

<figure><img src="../../../.gitbook/assets/5.4.7 Classification.png" alt=""><figcaption><p>Displaying only text</p></figcaption></figure>

f) You can see two new fields getting enabled as shown below. Let's apply the '**Color for**' font and add 'Percentage text' on the left. You can see the contribution percentage displayed on the left along with the text.&#x20;

<figure><img src="../../../.gitbook/assets/5.4.8 Classification.png" alt=""><figcaption><p>Only text along with percentages</p></figcaption></figure>

g) Instead of color for the font, background color can also be applied. Select 'Background' in the 'Color for' dropdown.

<figure><img src="../../../.gitbook/assets/5.4.9 Classification.png" alt=""><figcaption><p>Background color for ABC classification</p></figcaption></figure>

h) You can define custom ranges using the 'Add range', 'Text editor', 'Color picker' and 'Reverse text/color order' options as shown below.

<figure><img src="../../../.gitbook/assets/5.4.10 Classification.png" alt=""><figcaption><p>Customizing the ranges</p></figcaption></figure>

i) Ranges can also be defined using numeric values. Click on the 'Value' option. The values get populated automatically based on the defined percentages, but they can be further edited.

<figure><img src="../../../.gitbook/assets/5.4.11 Classification.png" alt=""><figcaption><p>Ranges based on numeric values</p></figcaption></figure>

j) You can delete specific ranges or reset all changes using the icons highlighted in the below image.&#x20;

<figure><img src="../../../.gitbook/assets/5.4.12 Classification.png" alt=""><figcaption><p>Deleting and resetting ranges</p></figcaption></figure>

### 2. Icon set

Icon-based formatting provides the same properties as text-based formatting. Refer to [Text](classification.md#1.-text) for more details. We'll only at a simple example for icon sets.&#x20;

In the 'Display' dropdown, choose the 'Five arrows' option. Click 'Apply'. Note that we have applied formatting to 2021 Actuals based on 2021 Actuals - 2021 Plan. Hence, we can see which categories have done worse/better than the plan.

<figure><img src="../../../.gitbook/assets/5.4.14 Classification.png" alt=""><figcaption><p>Classification based on icon sets</p></figcaption></figure>

### 3. Rating

You can also use star-based ratings as seen in e-commerce sites in the product feedback section.

a) Select the '3 stars' option from the 'Display' dropdown and click 'Apply'.

<figure><img src="../../../.gitbook/assets/5.4.15 Classification.png" alt=""><figcaption><p>Conditional formatting - Rating</p></figcaption></figure>

b) You can see the 1-5 rating icons on the left of the data. By default, the number of ranges has been set to 5.

<figure><img src="../../../.gitbook/assets/5.4.16 Classification.png" alt=""><figcaption><p>5-star rating</p></figcaption></figure>

c) You can move the ratings to a separate column by clicking on the '**Show as new column**' checkbox.

<figure><img src="../../../.gitbook/assets/5.4.17 Classification.png" alt=""><figcaption><p>Ratings in a new column</p></figcaption></figure>

d) Check the '**Invert rating**' checkbox in cases where higher values need to show lower ratings.

<figure><img src="../../../.gitbook/assets/5.4.18 Classification.png" alt=""><figcaption><p>Inverted ratings</p></figcaption></figure>

e) As seen in text and icon-based formatting, you can choose only to display the classification or change the position. In the below example, we have chosen the 'Only rating' option.

<figure><img src="../../../.gitbook/assets/5.4.19 Classification.png" alt=""><figcaption><p>Displaying only rating</p></figcaption></figure>

f) You can customize the number of icons that appear in your scale – '**Number of range**s' has been set to 3 in this case.&#x20;

<figure><img src="../../../.gitbook/assets/5.4.20 Classification.png" alt=""><figcaption><p>Changing the number of ranges</p></figcaption></figure>

g) The rating text can be shown on the left or right. Select the position and color as shown below.

<figure><img src="../../../.gitbook/assets/5.4.21 Classification.png" alt=""><figcaption><p>Rating text</p></figcaption></figure>

h) In Inforiver, you have the option to configure value ranges for each of the ratings. Click on the '**Enable custom**' checkbox. For every half rating, you'll be able to define percentage/value ranges in the 'From' and 'To' fields as shown in the below image.

<figure><img src="../../../.gitbook/assets/5.4.22 Classification.png" alt=""><figcaption><p>Custom ranges</p></figcaption></figure>

i) To reverse the order of colors and reset all changes to the ranges, click on the highlighted icons.

<figure><img src="../../../.gitbook/assets/5.4.23Classification.png" alt=""><figcaption><p>Reorder colors and reset changes</p></figcaption></figure>

In the next section, let's look at [Ranking](ranking.md).
