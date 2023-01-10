# Rules (If conditions)

You can apply conditional formatting using font color, style, icons or background based on one or more IF conditions.

Refer to [create rule](create-rule-basic-settings.md) to get started. Once the rule is created and you can see the 'Conditional formatting' side panel, follow the below steps.

a) Choose 'Rules (If conditions)' in the '**Format by**' dropdown. You can see two sections - Style and Conditions.

<figure><img src="../../.gitbook/assets/5.2.35 if conditions.png" alt=""><figcaption><p>Choosing Rules (If conditions)</p></figcaption></figure>

b) Using the '**Style**' section, you can format text based on color/style, apply a background color or select icons.&#x20;

c) In the '**Conditions**' section, you can define conditions using options such as Number, Data selection, Values, Formula and User Selection.

<figure><img src="../../.gitbook/assets/FormatByRules.png" alt=""><figcaption><p>Format by rules</p></figcaption></figure>

Let's look at an example for each of these options.

### 1. Number

In this example, we are highlighting the subcategories where 2021 Actuals are greater than 10 million. Note that we have selected 'Bold' and selected 'Green' as the font color. The numbers field supports scaled entries such as 10m. Click 'Apply' once the changes are done.

<figure><img src="../../.gitbook/assets/5.2.4(2) Number based.png" alt=""><figcaption><p>Conditional formatting based on a numeric input</p></figcaption></figure>

### 2. Data selection

You can also use a cell value in the condition.&#x20;

a) Select 'Data selection', click on the 'Set value' field and select a cell in the report.

<figure><img src="../../.gitbook/assets/5.2.8 Data selection.png" alt=""><figcaption><p>Applying background color to values and totals</p></figcaption></figure>

Note:&#x20;

* In this example, we have used 'Values and Totals' as the 'Row hierarchy levels'. You can see a new field where you can choose whether conditional formatting needs to be applied to the row grand total or not.&#x20;
* We are also using a background color for the formatting.

b) Click on the 'select value from' field and click on a cell in the report. The value gets populated automatically. Click 'Apply'.

<figure><img src="../../.gitbook/assets/5.2.10 Data selection.png" alt=""><figcaption><p>Selecting data from the report </p></figcaption></figure>

c) The formatting gets applied to all the hierarchy levels where 2021 Actuals are greater than the selected value.

<figure><img src="../../.gitbook/assets/5.2.11 Data selection.png" alt=""><figcaption><p>Conditional formatting based on data selection</p></figcaption></figure>

### 3. Value

You can apply conditional formatting based on another measure in the visual. Let's highlight 2021 Actuals when it is greater than the 2021 Plan.

{% hint style="info" %}
Measures that were added from the data source, auto-calculated variances, columns/measures created using calculations, data input and simulations can all be used in the IF condition.
{% endhint %}

a) Click on the highlighted dropdown and select 2021 Plan. Click 'Apply'.

<figure><img src="../../.gitbook/assets/5.2.12 Value.png" alt=""><figcaption><p>Conditional formatting based on another measure </p></figcaption></figure>

b) Note that conditional formatting is applied only to the totals - Categories, Regions and Subregions since we have chosen 'Row hierarchy levels' as 'Totals' and included 'Row grand total'.

<figure><img src="../../.gitbook/assets/5.2.13 Value.png" alt=""><figcaption><p>Conditional formatting when 2021 Actuals > 2021 Plan</p></figcaption></figure>

### 4. Formula

You can create simple formulas using either numeric values or measures. Let's highlight the records where 2021 Actuals are greater than the 2021 Plan by at least 5m. Configure as shown in the below image and click 'Apply'.  &#x20;

<figure><img src="../../.gitbook/assets/5.2.14 Formula.png" alt=""><figcaption><p>Conditional formatting based on formula</p></figcaption></figure>

Tea & coffee in the East subregion is the only record that matches the given condition.

<figure><img src="../../.gitbook/assets/5.2.15 Formula.png" alt=""><figcaption><p>Conditional formatting based on formula</p></figcaption></figure>

As you can see in the side panel, there is a '**Add condition**' option, which lets you create nested AND/OR conditions.&#x20;

Let's consider another example where the conditions are Q4 2021 Actuals greater than 10m, the Category is Beverages and the Sub-regions are Pacific and East.

a) Configure the settings as shown below for the first condition. Click on 'Add condition'.

<figure><img src="../../.gitbook/assets/5.2.16 Formula.png" alt=""><figcaption><p>Nested conditions</p></figcaption></figure>

b) You can see another condition with default selections and an option to select AND/OR. Let's select 'AND' and 'Category' from the highlighted dropdown.

<figure><img src="../../.gitbook/assets/5.2.23 Formula.png" alt=""><figcaption><p>Adding an AND condition</p></figcaption></figure>

c) You can see several options as shown in the below image. Let's go with the default option.

<figure><img src="../../.gitbook/assets/5.2.24 Formula.png" alt=""><figcaption><p>Options for category</p></figcaption></figure>

d) In the 'Choose members' dropdown, select 'Beverages'.

<figure><img src="../../.gitbook/assets/5.2.25 Formula.png" alt=""><figcaption><p>Selecting a category</p></figcaption></figure>

e) Let's now add the third condition. Click on 'Add condition'. In the highlighted dropdown (2021 Plan), select 'Sub Region'.

<figure><img src="../../.gitbook/assets/5.2.26 Formula.png" alt=""><figcaption><p>Adding a third condition</p></figcaption></figure>

f) Select Pacific and East in the dropdown as shown below. Click 'Apply'.

<figure><img src="../../.gitbook/assets/5.2.27 Formula.png" alt=""><figcaption><p>Selecting multiple regions</p></figcaption></figure>

g) You can see that the rows for Juices and Soda for East and Pacific are highlighted based on the three conditions.

<figure><img src="../../.gitbook/assets/5.2.28 Formula.png" alt=""><figcaption><p>Conditional formatting based on nested conditions</p></figcaption></figure>

### 5. User selection

You can apply conditional formatting based on a selection during runtime ie. in the reading view. Let's consider a case where we want conditional formatting to be applied to 2021 Actuals based on a Variance value selected during runtime.

a) Configure as shown in the below image. Note that 2021 Actuals is set in the 'Apply to' field and 'Variance' in the IF condition. Click on the dropdown and select 'Variance'.&#x20;

<figure><img src="../../.gitbook/assets/5.2.30 User selection.png" alt=""><figcaption><p>Conditional formatting based on user selection</p></figcaption></figure>

b) Let's also add an icon. Click on the 'Icon' checkbox. There are several customization options.

<figure><img src="../../.gitbook/assets/5.2.31 User selection.png" alt=""><figcaption><p>Adding an icon</p></figcaption></figure>

c) Click on the icon dropdown and choose the flag icon.

<figure><img src="../../.gitbook/assets/5.2.32 User selection.png" alt=""><figcaption><p>Customizing the icon</p></figcaption></figure>

d) Change the flag color to green and the font color to black. Click 'Apply'.

<figure><img src="../../.gitbook/assets/5.2.33 User selection.png" alt=""><figcaption><p>Customizing the icon color</p></figcaption></figure>

e) Click on a value in any of the variance columns. You can see flag icons in the 2021 Actuals column where the variance is greater than the selected variance.

<figure><img src="../../.gitbook/assets/5.2.34 User selection.png" alt=""><figcaption><p>Conditional formatting based on user selection</p></figcaption></figure>

In the next section, we'll be covering [Color scale](color-scale.md).
