# Rules (If conditions)

You can apply conditional formatting using font color, style, icons, or background based on one or more IF conditions.

Refer to the [Create Rule](create-rule-basic-settings.md) section to get started. Once the rule is created and you can see the Conditional Formatting side panel, follow the below steps.

**STEP 1:** Choose 'Rules (If conditions)' in the **Format by** dropdown. You can see two sections - Style and Conditions.

<figure><img src="../../.gitbook/assets/5.2.35 if conditions.png" alt=""><figcaption><p>Choosing Rules (If conditions)</p></figcaption></figure>

**STEP 2:** Using the **Style** section, you can format text based on color/style, apply a background color, or select icons.&#x20;

**STEP 3:** In the 'Conditions' section, you can define conditions using options such as Number, Data selection, Values, Formula, and User Selection.

<figure><img src="../../.gitbook/assets/FormatByRules.png" alt=""><figcaption><p>Format by rules</p></figcaption></figure>

**STEP 4:** When you have inline charts in your reports, conditional formatting rules can be applied to the chart labels or the chart itself. Select the desired option(s) from the **Impact on** lis&#x74;**.** Notice how the bars for subcategories with sales > 20k are highlighted in blue.

<figure><img src="../../.gitbook/assets/image (1206).png" alt=""><figcaption><p>Impact on</p></figcaption></figure>

Let's look at examples for each of these options.

## Style

* **Font style: bold, italic, underline**

Set the font style based on conditional formatting rules. Notice how we've applied Bold, Italics, and Underlined the values that satisfy the condition. Click on the <img src="../../.gitbook/assets/image (1) (10).png" alt="" data-size="line">icon to apply a color for the underline.

<figure><img src="../../.gitbook/assets/image (2) (9).png" alt=""><figcaption><p>Font style</p></figcaption></figure>

* **Cell background**

Highlight the cells that match a conditional formatting rule by applying a background color.

<figure><img src="../../.gitbook/assets/image (3) (9).png" alt=""><figcaption><p>Cell background</p></figcaption></figure>

* **Font color**

Apply a custom font color when a conditional formatting rule is met.

<figure><img src="../../.gitbook/assets/image (4) (7).png" alt=""><figcaption><p>Font color</p></figcaption></figure>

* **Cell borders**

Highlight cells that satisfy the conditional formatting rule by setting a custom border. You can choose the border color by clicking the<img src="../../.gitbook/assets/image (5) (9).png" alt="" data-size="line"> icon.

<figure><img src="../../.gitbook/assets/image (6) (10).png" alt=""><figcaption><p>Applying borders</p></figcaption></figure>

* **Adding icons or text**

Display icons to apply conditional formatting on your data. You can also use custom icons by clicking the Upload Icon link.

<figure><img src="../../.gitbook/assets/image (7) (10).png" alt=""><figcaption><p>Applying icons</p></figcaption></figure>

You can position the text/icons with respect to the cell values. You can also choose to display only the icons or text and hide the cell values.

<figure><img src="../../.gitbook/assets/Untitled Project (1) (1) (1) (1) (1) (1).gif" alt=""><figcaption><p>Using icons and text</p></figcaption></figure>

When you use icons, you have an additional option to align your icons in the grid. By default, the icons are left aligned.

<div><figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Aligning icons</p></figcaption></figure> <figure><img src="../../.gitbook/assets/conditional-formatting-icon-alignment-left-2048x1159.png" alt=""><figcaption><p>Left-align option disabled</p></figcaption></figure></div>

* **Hiding values**

Business reporting may require withholding certain information to protect strategic interests. You can use conditional formatting rules to mask values based on specific criteria.

<figure><img src="../../.gitbook/assets/image (8) (9).png" alt=""><figcaption><p>Hiding values</p></figcaption></figure>

* **Hatched fill pattern**

Highlight your data with hatched cell backgrounds – this feature allows you to spotlight your data with hatched styling.

<figure><img src="../../.gitbook/assets/image (1101).png" alt=""><figcaption><p>Hatched CF</p></figcaption></figure>

## Conditions

### 1. Number

In this example, we are highlighting the subcategories where 2021 Actuals are greater than 10 million. Note that we have selected 'Bold' and selected 'Green' as the font color. The numbers field supports scaled entries such as 10m. Click 'Apply' once the changes are done.

<figure><img src="../../.gitbook/assets/5.2.4(2) Number based.png" alt=""><figcaption><p>Conditional formatting based on a numeric input</p></figcaption></figure>

### 2. Data selection

You can also use a cell value in the condition.&#x20;

2.1. Select 'Data selection', click on the 'Set value' field and select a cell in the report.

<figure><img src="../../.gitbook/assets/5.2.8 Data selection.png" alt=""><figcaption><p>Applying background color to values and totals</p></figcaption></figure>

Note:&#x20;

* In this example, we have used 'Values and Totals' as the 'Row hierarchy levels'. You can see a new field where you can choose whether conditional formatting needs to be applied to the row grand total or not.&#x20;
* We are also using a background color for the formatting.

2.2. Click on the 'select value from' field and click on a cell in the report. The value gets populated automatically. Click 'Apply'.

<figure><img src="../../.gitbook/assets/5.2.10 Data selection.png" alt=""><figcaption><p>Selecting data from the report </p></figcaption></figure>

2.3. The formatting is applied to all the hierarchy levels where 2021 Actuals are greater than the selected value.

<figure><img src="../../.gitbook/assets/5.2.11 Data selection.png" alt=""><figcaption><p>Conditional formatting based on data selection</p></figcaption></figure>

### 3. Value

You can apply conditional formatting based on another measure in the visual. Let's highlight 2021 Actuals when it is greater than the 2021 Plan.

{% hint style="info" %}
Measures that were added from the data source, auto-calculated variances, columns/measures created using calculations, data input and simulations can all be used in the IF condition.
{% endhint %}

3.1. Click on the highlighted dropdown and select 2021 Plan. Click 'Apply'.

<figure><img src="../../.gitbook/assets/5.2.12 Value.png" alt=""><figcaption><p>Conditional formatting based on another measure </p></figcaption></figure>

3.2. Note that conditional formatting is applied only to the totals - Categories, Regions, and Subregions since we have chosen 'Row hierarchy levels' as 'Totals' and included 'Row grand total'.

<figure><img src="../../.gitbook/assets/5.2.13 Value.png" alt=""><figcaption><p>Conditional formatting when 2021 Actuals > 2021 Plan</p></figcaption></figure>

### 4. Formula

You can create simple formulas using either numeric values or measures. Let's highlight the records where 2021 Actuals are greater than the 2021 Plan by at least 5m. Configure as shown in the below image and click 'Apply'.  &#x20;

<figure><img src="../../.gitbook/assets/5.2.14 Formula.png" alt=""><figcaption><p>Conditional formatting based on formula</p></figcaption></figure>

Tea & coffee in the East subregion is the only record that matches the given condition.

<figure><img src="../../.gitbook/assets/5.2.15 Formula.png" alt=""><figcaption><p>Conditional formatting based on formula</p></figcaption></figure>

The '**Add condition**' option lets you create nested AND/OR conditions.&#x20;

Let's consider another example where the conditions are Q4 2021 Actuals greater than 10m, the Category is Beverages and the Sub-regions are Pacific and East.

**STEP 1:** Configure the settings as shown below for the first condition. Click on 'Add condition'.

<figure><img src="../../.gitbook/assets/5.2.16 Formula.png" alt=""><figcaption><p>Nested conditions</p></figcaption></figure>

**STEP 2:** You can see another condition with default selections and an option to select AND/OR. Let's select 'AND' and 'Category' from the highlighted dropdown.

<figure><img src="../../.gitbook/assets/5.2.23 Formula.png" alt=""><figcaption><p>Adding an AND condition</p></figcaption></figure>

**STEP 3:** You can see several options as shown in the below image. Let's go with the default option.

<figure><img src="../../.gitbook/assets/5.2.24 Formula.png" alt=""><figcaption><p>Options for category</p></figcaption></figure>

**STEP 4:** In the 'Choose members' dropdown, select 'Beverages'.

<figure><img src="../../.gitbook/assets/5.2.25 Formula.png" alt=""><figcaption><p>Selecting a category</p></figcaption></figure>

**STEP 5:** Let's now add the third condition. Click on 'Add condition'. In the highlighted dropdown (2021 Plan), select 'Sub Region'.

<figure><img src="../../.gitbook/assets/5.2.26 Formula.png" alt=""><figcaption><p>Adding a third condition</p></figcaption></figure>

**STEP 6:** Select Pacific and East in the dropdown as shown below. Click 'Apply'.

<figure><img src="../../.gitbook/assets/5.2.27 Formula.png" alt=""><figcaption><p>Selecting multiple regions</p></figcaption></figure>

**STEP 7:** You can see that the rows for Juices and Soda for East and Pacific are highlighted based on the three conditions.

<figure><img src="../../.gitbook/assets/5.2.28 Formula.png" alt=""><figcaption><p>Conditional formatting based on nested conditions</p></figcaption></figure>

### 5. User selection

You can apply conditional formatting based on a selection during runtime ie. in the reading view. Let's consider a case where we want conditional formatting to be applied to 2021 Actuals based on a Variance value selected during runtime.

**STEP 1:** Configure as shown in the below image. Note that 2021 Actuals is set in the 'Apply to' field and 'Variance' in the IF condition. Click on the dropdown and select 'Variance'.&#x20;

<figure><img src="../../.gitbook/assets/5.2.30 User selection.png" alt=""><figcaption><p>Conditional formatting based on user selection</p></figcaption></figure>

**STEP 2:** Let's also add an icon. Click on the 'Icon' checkbox. There are several customization options.

<figure><img src="../../.gitbook/assets/5.2.31 User selection.png" alt=""><figcaption><p>Adding an icon</p></figcaption></figure>

**STEP 3:** Click on the icon dropdown and choose the flag icon.

<figure><img src="../../.gitbook/assets/5.2.32 User selection.png" alt=""><figcaption><p>Customizing the icon</p></figcaption></figure>

**STEP 4:** Change the flag color to green and the font color to black. Click 'Apply'.

<figure><img src="../../.gitbook/assets/5.2.33 User selection.png" alt=""><figcaption><p>Customizing the icon color</p></figcaption></figure>

**STEP 5:** Click on a value in any of the variance columns. You can see flag icons in the 2021 Actuals column where the variance is greater than the selected variance.

<figure><img src="../../.gitbook/assets/5.2.34 User selection.png" alt=""><figcaption><p>Conditional formatting based on user selection</p></figcaption></figure>

### 6. Dates

With Inforiver, you can compare date dimensions in rows and columns and automatically format cells based on the comparison. Let's add date dimensions in the row and column parameters. To compare two date dimensions, select the **Compare Date** option. In the example below, we used conditional formatting to highlight the cells where the order date exceeds the ship date.

<figure><img src="../../.gitbook/assets/image (504).png" alt=""><figcaption><p>Compare date dimensions</p></figcaption></figure>

In the example above, we compared each ship date against each order date and highlighted the cells with the order date greater than the ship date. Instead of comparing each cell, you can also compare a date dimension with the minimum or maximum value of another date dimension. To demonstrate this, let's highlight the cells with the order date greater than the minimum ship date.

<figure><img src="../../.gitbook/assets/image (506).png" alt=""><figcaption><p>Highlight cells with order date greater than minimum of ship date</p></figcaption></figure>

You can compare date dimensions against static dates using the Selected Date option and specify the date to be compared against.

<figure><img src="../../.gitbook/assets/image (505).png" alt=""><figcaption><p>Compare against static dates</p></figcaption></figure>

### 7. Conditional formatting for data input fields

Highlight your data input fields like number, dropdown, and person columns with conditional formatting. When users enter values, you can specify rules to automatically apply formatting when the rules are satisfied e.g. spotlight the cells when the budget entered exceeds a certain limit.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Conditional formatting for data input fields</p></figcaption></figure>

### 8. Rules for non-numeric measures

You can apply conditional formatting to non-numeric measures using conditions like **is blank/is not blank/contains/does not contain,** etc. In this example, we've set a hatched background for the cells with blank customer names.

<figure><img src="../../.gitbook/assets/image (6) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

In the next section, we'll be covering [Color scale](color-scale.md).
