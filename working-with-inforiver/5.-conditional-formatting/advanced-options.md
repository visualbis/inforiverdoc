# Advanced options

You can build your own conditional formatting rules from scratch in a detailed manner or customize the rules created using the one-click options if your report requires it.&#x20;

## 1. Basic settings

a) To create a new rule, select Home -> Conditional Formatting -> Create Rule. A conditional formatting window opens as shown in the below image.

<figure><img src="../../.gitbook/assets/3.png" alt=""><figcaption><p>Create rule</p></figcaption></figure>

b) Rename the rule by editing the '**Title**' field.

c) You can apply conditional formatting to the row headers, rows, column headers, or columns/measures. Choose the desired option in the '**Apply to**' field.

d) You can apply conditional formatting to values and totals, totals only or values only. By default, 'Values only' will be selected. Customize as required using the '**Row hierarchy levels**' field.

<div>

<figure><img src="../../.gitbook/assets/5.2.2 Apply to.png" alt=""><figcaption><p>Apply to - Options</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/5.2.3 Levels.png" alt=""><figcaption><p>Row hierarchy levels - Options</p></figcaption></figure>

</div>

e) There are a number of conditional formatting formats that you can use to create rules. You can select the desired format using the ‘**Format by**’ field. The available options are Rules (If Conditions), Color Scale, Classification and Ranking.

<figure><img src="../../.gitbook/assets/5.2.1 Format by.png" alt=""><figcaption><p>Format by - Options</p></figcaption></figure>

Let's take a look at each of the formats.

## 2. Rules (If conditions)

You can apply conditional formatting using font color, style, icons or background based on one or more IF conditions.

a) Choose 'Rules (If conditions)' in the '**Format by**' dropdown.

b) Using the '**Style**' section, you can format text based on color/style, apply a background color or select icons.&#x20;

c) In the '**Conditions**' section, you can define conditions using options such as Number, Data selection, Values, Formula and User Selection.

<figure><img src="../../.gitbook/assets/FormatByRules.png" alt=""><figcaption><p>Format by rules</p></figcaption></figure>

Let's look at an example for each of these options.

### i) Number

In this example, we are highlighting the subcategories where 2021 Actuals are greater than 10 million. Note that we have selected 'Bold' and selected 'Green' as the font color. The numbers field supports scaled entries such as 10m. Click 'Apply' once the changes are done.

<figure><img src="../../.gitbook/assets/5.2.4(2) Number based.png" alt=""><figcaption><p>Conditional formatting based on a numeric input</p></figcaption></figure>

### ii) Data selection

You can also use a cell value in the condition. Select 'Data selection', click on the 'Set value' field and select a cell in the report.

Note:&#x20;

a) In this example, we have used 'Values and Totals' as the 'Row hierarchy levels'. You can see a new field where you can choose whether conditional formatting needs to be applied to the row grand total or not.&#x20;

b) We are also using a background color for the formatting.

<figure><img src="../../.gitbook/assets/5.2.8 Data selection.png" alt=""><figcaption><p>Applying background color to values and totals</p></figcaption></figure>

Click on the 'select value from' field and click on a cell in the report. The value gets populated automatically. Click 'Apply'.

<figure><img src="../../.gitbook/assets/5.2.10 Data selection.png" alt=""><figcaption><p>Selecting data from the report </p></figcaption></figure>

The formatting gets applied to all the hierarchy levels where 2021 Actuals are greater than the selected value.

<figure><img src="../../.gitbook/assets/5.2.11 Data selection.png" alt=""><figcaption><p>Conditional formatting based on data selection</p></figcaption></figure>

### iii) Value

You can apply conditional formatting based on another measure in the visual. Let's highlight 2021 Actuals when it is greater than the 2021 Plan.

{% hint style="info" %}
Measures that were added from the data source, auto-calculated variances, columns/measures created using calculations, data input and simulations can all be used in the IF condition.
{% endhint %}

Click on the highlighted dropdown and select 2021 Plan. Click 'Apply'.

<figure><img src="../../.gitbook/assets/5.2.12 Value.png" alt=""><figcaption><p>Conditional formatting based on another measure </p></figcaption></figure>

Note that conditional formatting is applied only to the totals - Categories, Regions and Subregions since we have chosen 'Row hierarchy levels' as 'Totals' and included 'Row grand total'.

<figure><img src="../../.gitbook/assets/5.2.13 Value.png" alt=""><figcaption><p>Conditional formatting when 2021 Actuals > 2021 Plan</p></figcaption></figure>







## 3. Color scale





## 4. Classification





## 5. Ranking







