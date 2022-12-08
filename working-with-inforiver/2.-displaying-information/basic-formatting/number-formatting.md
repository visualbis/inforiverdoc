# Number formatting

Inforiver for Power BI comes prepackaged with _intelligent number formatting & scaling recognition_ capabilities that help display data in a perceptive manner in your table/matrix style reports right out of the box.

## 1. Number scaling

Let us take a sample dataset as shown below. You can immediately spot data of mixed granularity – with values in millions, thousands, and even one that is just a few dollars worth.

<figure><img src="../../../.gitbook/assets/2.4.3.1 Data.png" alt=""><figcaption><p>Data of mixed granularity</p></figcaption></figure>

Let us see how you can handle a dataset of varying granularities & formats using Inforiver.&#x20;

In the Home tab, click on the 'Quick format' dropdown. There are several options, let us look at each of them in detail.

<figure><img src="../../../.gitbook/assets/2.4.1.1 Dropdown menu.png" alt=""><figcaption><p>Number scaling options</p></figcaption></figure>

### a) Measure level scaling

By default, when you assign this data to Inforiver, each measure is formatted using an individual scale. The scaling for each measure is shown in the column header. This is useful to show measures of varying granularities (e.g., Revenue & Quantity) in the same table.

<figure><img src="../../../.gitbook/assets/2.4.1.2 Measure level scaling.png" alt=""><figcaption><p>Measure level scaling</p></figcaption></figure>

### b) Uniform scaling

The 'Uniform' option applies one fixed scale to the entire table and moves the scaling unit display to the header. This is useful when all the measures are of comparable magnitude (e.g., Sales vs Forecast) in the same table.

<figure><img src="../../../.gitbook/assets/2.4.1.3 Uniform scaling.png" alt=""><figcaption><p>Uniform scaling</p></figcaption></figure>

Inforiver automatically chooses the scaling based on the values. But you change it if needed. When you expand the dropdown again, you can see more options. You can select millions, billions, etc. as needed.

<figure><img src="../../../.gitbook/assets/2.4.1.4 Auto Uniform scaling.png" alt=""><figcaption><p>Uniform formatting options</p></figcaption></figure>

### c) Auto scaling

When using the 'auto' option, each cell is formatted individually. In the below image, you can see the suffixes - m and k to denote millions and thousands.

<figure><img src="../../../.gitbook/assets/2.4.1.5 Auto scaling.png" alt=""><figcaption><p>Cell level scaling</p></figcaption></figure>

### d) Native scaling

If you do not want any fancy formatting and need the numbers just as they are in the source data, select the ‘Native’ option.&#x20;

<figure><img src="../../../.gitbook/assets/2.4.1.6 Native scaling.png" alt=""><figcaption><p>Native scaling</p></figcaption></figure>

Inforiver also shows the unscaled values in the tooltip (available upon publishing to service). This helps you scale values without losing the ability to look up the unscaled value whenever required.

<figure><img src="../../../.gitbook/assets/2.4.1.7 Service.png" alt=""><figcaption><p>Tooltip shows unscaled values in 'Reading view'</p></figcaption></figure>

## 2. Percentage, prefix/suffix, and decimals

Inforiver provides options to fine-tune the format at a row, column/measure, or cell level using the icons just below the 'Quick format' dropdown. These options include conversion to % format, attaching prefix/suffix, and increasing/decreasing decimal spaces.&#x20;

<figure><img src="../../../.gitbook/assets/2.4.1.8 Formatting options.png" alt=""><figcaption><p>Number formatting options</p></figcaption></figure>

In this example, we have current year and prior year sales, YoY sales, and Margin.&#x20;

### a) Percentage

As you can see in the footnotes, the measure Margin is actually Margin% and needs to be converted as a percentage.

To do this, let's select the column. % icon gets enabled. Once you click on the icon, the values get converted to percentages.

<div>

<figure><img src="../../../.gitbook/assets/2.4.1.9 Pct.png" alt=""><figcaption><p>Percentage option gets enabled on selecting a column/row/cell</p></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/2.4.2.0 Pct.png" alt=""><figcaption><p>Margins are converted to percentage</p></figcaption></figure>

</div>



### b) Prefix/suffix

Using Inforiver, you can insert prefixes such as currency or suffixes like units.&#x20;

&#x20;In the below example Price is in $ per unit. Select the column and click on the highlighted icon. Enter the prefix and suffix as shown.&#x20;

<figure><img src="../../../.gitbook/assets/2.4.1.11 Prefix suffix.png" alt=""><figcaption><p>Enter prefix and suffix</p></figcaption></figure>

Click 'Apply'. The changes get reflected as highlighted.

<figure><img src="../../../.gitbook/assets/2.4.1.12 Prefix suffix applied.png" alt=""><figcaption><p>Price column shows the added prefix/suffix</p></figcaption></figure>

### c) Decimals

You can increase or decrease decimal places at a cell/row/column level.&#x20;

Let's remove the decimals for the Sales and Price columns. Use Shift+Select to select the two columns and click on the 'decrease decimal' icon twice. The decimals are removed. The 'Increase decimal' option can be used similarly to increase decimal places. &#x20;

<div>

<figure><img src="../../../.gitbook/assets/2.4.1.13 Decrease decimal.png" alt=""><figcaption><p>Select the columns and decrease decimals</p></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/2.4.1.14 Decrease decimal.png" alt=""><figcaption><p>Changes in decimal places are reflected</p></figcaption></figure>

</div>



## 3. Semantic formatting

Inforiver provides a number of options to customize numbers.

In the 'Home' tab, click on the 'Display' settings. In the 'Numbers' tab, you'll find options such as Semantic formatting, Value display, Sign, and more. In this section, let's talk about semantic formatting.&#x20;

On enabling the toggle, you can see the positive and negative options as shown below. By default, they are shown in green and red, but they can be customized using the color picker.&#x20;

<figure><img src="../../../.gitbook/assets/2.4.1.15 Semantic formatting.png" alt=""><figcaption><p>Apply colors to positive and negative numbers</p></figcaption></figure>

You can also display positive and negative numbers in the formats shown below.

<div>

<figure><img src="../../../.gitbook/assets/2.4.1.17 Semantic formatting.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/2.4.1.16 Semantic formatting.png" alt=""><figcaption></figcaption></figure>

</div>
