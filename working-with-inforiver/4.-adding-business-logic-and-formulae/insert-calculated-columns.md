# Insert calculated columns

With Inforiver, it is possible to insert a new calculated row, column or measure at the visual level in your Power BI table/matrix style reports, without writing DAX. The rows, measures and columns so created can also be formatted, rearranged, and utilized for downstream calculations.

The Excel-like formula engine supports 50+ functions (logical, boolean, math functions and more). The formula editor provides syntax, examples and features such as autocomplete, multi-line support and more to help users create, and troubleshoot formulas

### 1. Visual measure

Let us take this example, where we have sales data for two years, 2021 and 2020, by quarter. We will now try to insert a measure that calculates the percentage variance using the formula (2021 Actuals - 2020 Actuals) / 2020 Actuals.

<figure><img src="../../.gitbook/assets/4.2.1 Data.png" alt=""><figcaption><p>Sales for 2021 and 2020 by quarter</p></figcaption></figure>

a) To insert a measure, select 'Insert Formula' from the 'Insert' tab. A side panel opens on the right.

<figure><img src="../../.gitbook/assets/4.2.2 Measure.png" alt=""><figcaption><p>Visual measure</p></figcaption></figure>

b) You will see two options in the 'Insert as' field: Visual Measure (the default) and Visual Column. Let us go ahead with the default option - the visual measure.&#x20;

The visual measure behaves like a measure, except that it is inserted directly in your visual (bypassing the data model). In the image below, note that this new measure is inserted under each quarter.

<figure><img src="../../.gitbook/assets/4.2.3 Measure.png" alt=""><figcaption><p>Visual measure</p></figcaption></figure>

c) Once you place the cursor inside the formula editor, you will see a context assistant pop-up. You can access other references or functions through this context assistant.

<figure><img src="../../.gitbook/assets/4.2.5 Measure.png" alt=""><figcaption><p>List of references</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/4.2.11 Measure.png" alt=""><figcaption><p>List of functions</p></figcaption></figure>

d) Let us go ahead and start typing in values. As you key in a formula, the _References_ list automatically refreshes to show a narrower set of options.&#x20;

<figure><img src="../../.gitbook/assets/4.2.6 Measure.png" alt=""><figcaption><p>Reference list</p></figcaption></figure>

e) We will go ahead and complete the formula as shown below. The rectangular parentheses in the formula indicate that these are not normal text but references to other measures.

<figure><img src="../../.gitbook/assets/4.2.7 Measure.png" alt=""><figcaption><p>Formula entered</p></figcaption></figure>

f) Give the calculated measure a proper name, say 'Variance %', and click 'Create'.&#x20;

<figure><img src="../../.gitbook/assets/4.2.8 Measure.png" alt=""><figcaption><p>Creating a measure</p></figcaption></figure>

g) You would have now inserted a calculated measure in your report. However, you will notice that the values are in absolute numbers and not in percentage terms.

<figure><img src="../../.gitbook/assets/4.2.9 Measure.png" alt=""><figcaption><p>Measure inserted</p></figcaption></figure>

h) To convert the values to a percentage format, click on the % icon from the 'Home' tab. As you do this, you will also notice that the formula bar at the top of the matrix shows how the measure is calculated.

<figure><img src="../../.gitbook/assets/4.2.10 Measure.png" alt=""><figcaption><p>Formula bar showing the calculation</p></figcaption></figure>

We have successfully inserted a calculated measure at the visual level in our Power BI matrix report.

We have used the default '[Row aggregation type](insert-manual-input-columns/insert-manual-input-columns.md#i-row-aggregation-type)' which is 'Formula'. This property is covered in detail in the Number column section.

### 2. Visual column

A calculated column works differently from a calculated measure. Let's consider two examples.

#### Example 1:

a) Let us calculate quarter-on-quarter change from Q3 to Q4. Select the 'Visual column' option. Note that a visual column always appears at the last, outside any category or category hierarchies seen in columns.

<figure><img src="../../.gitbook/assets/4.2.14 Column.png" alt=""><figcaption><p>Visual column</p></figcaption></figure>

b) You will also notice that the _References_ section is a bit different. While creating a [new measure](insert-calculated-columns.md#1.-visual-measure), the _References_ section was just listing other available measures (2021 Actuals and 2020 Actuals). This time, it shows every instance of the individual measures (e.g. Q2 - 2021 Actuals, Q3 - 2021 Actuals etc.). Using this, you can traverse right up to the leaf node of any column hierarchy.

<figure><img src="../../.gitbook/assets/4.2.13 Column.png" alt=""><figcaption><p>Reference list</p></figcaption></figure>

c) Enter a title and the formula and click 'Create'.

<figure><img src="../../.gitbook/assets/4.2.16 Column.png" alt=""><figcaption><p>Creating a visual column</p></figcaption></figure>

d) You will see the values updated in the report.

<figure><img src="../../.gitbook/assets/4.2.17 Column.png" alt=""><figcaption><p>Quarter on quarter column</p></figcaption></figure>

#### Example 2:

Let's consider an example where we use some functions. In the below example, we want to insert a column which displays the multiplier - 2022 Actuals/2022 Plan.&#x20;

a) Click on 'Insert formula'. Notice that there is no option to insert as a visual measure or column. This is because there is no column hierarchy.

<figure><img src="../../.gitbook/assets/4.2.22 Column.png" alt=""><figcaption><p>Inserting a new column</p></figcaption></figure>

b) Enter the title and the formula. Click 'Create'.&#x20;

<figure><img src="../../.gitbook/assets/4.2.23 Column.png" alt=""><figcaption><p>Defining the calculation</p></figcaption></figure>

c) Notice that there are Div/0! errors for two of the rows. There are two ways to deal with calculation errors.&#x20;

**i) Display settings -> Suppress calculation errors**

In the 'Home' tab, click on 'Display' settings. In the side panel, go to the 'Numbers' tab.&#x20;

<figure><img src="../../.gitbook/assets/4.2.24 Column.png" alt=""><figcaption><p>Suppress calculation errors</p></figcaption></figure>

Turn on the 'Suppress calculation errors' toggle. You can see a new field called 'Custom error text'.

<figure><img src="../../.gitbook/assets/4.2.25 Column.png" alt=""><figcaption><p>Suppress calculation errors</p></figcaption></figure>

You can define a custom text such as N.A., 0 or leave it blank. In the below image, we have entered 0. You can see the changes in the rows.&#x20;

<figure><img src="../../.gitbook/assets/4.2.26 Column.png" alt=""><figcaption><p>Define custom error text</p></figcaption></figure>

**ii) Using IFNA function**

Another way to handle calculation errors is by using the IFNA function. When an expression results in an error, you can replace it with a value as shown below.&#x20;

<figure><img src="../../.gitbook/assets/4.2.27 Column.png" alt=""><figcaption><p>Using IFNA function</p></figcaption></figure>

**iii) Using the IF function**

Another indirect approach would be to use IF/nested IF statements to define the value when the expression results in an error.&#x20;

<figure><img src="../../.gitbook/assets/4.2.28 Column.png" alt=""><figcaption></figcaption></figure>

We have now learnt how to insert calculated columns/measures in a Power BI matrix or a table report using Inforiver.

#### Resources

[Insert Formulas, Columns and Aggregation](https://www.youtube.com/watch?v=hjPAbuYJUSc)

[Visual calculations using Inforiver](https://inforiver.com/visual-calculations-powerbi/)
