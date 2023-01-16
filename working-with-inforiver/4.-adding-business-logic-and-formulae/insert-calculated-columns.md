# Insert calculated columns

With Inforiver, it is possible to insert a new calculated row, column or measure at the visual level in your Power BI table/matrix style reports, without writing DAX. The rows, measures and columns so created can also be formatted, rearranged, and utilized for downstream calculations.

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

### 2. Visual column

A calculated column works differently from a calculated measure.&#x20;

a) Let us calculate quarter-on-quarter change from Q3 to Q4. Select the 'Visual column' option. Note that a visual column always appears at the last, outside any category or category hierarchies seen in columns.

<figure><img src="../../.gitbook/assets/4.2.14 Column.png" alt=""><figcaption><p>Visual column</p></figcaption></figure>

b) You will also notice that the _References_ section is a bit different. While creating a [new measure](insert-calculated-columns.md#1.-visual-measure), the _References_ section was just listing other available measures (2021 Actuals and 2020 Actuals). This time, it shows every instance of the individual measures (e.g. Q2 - 2021 Actuals, Q3 - 2021 Actuals etc.). Using this, you can traverse right up to the leaf node of any column hierarchy.

<figure><img src="../../.gitbook/assets/4.2.13 Column.png" alt=""><figcaption><p>Reference list</p></figcaption></figure>

c) Enter a title and the formula and click 'Create'.

<figure><img src="../../.gitbook/assets/4.2.16 Column (1).png" alt=""><figcaption><p>Creating a visual column</p></figcaption></figure>

d) You will see the values updated in the report.

<figure><img src="../../.gitbook/assets/4.2.17 Column.png" alt=""><figcaption><p>Quarter on quarter column</p></figcaption></figure>

Let's consider an example where we use some functions.





We have now learnt how to insert a calculated column in a Power BI matrix or a table report using Inforiver.

#### Resources

[Insert Formulas, Columns and Aggregation](https://www.youtube.com/watch?v=hjPAbuYJUSc)
