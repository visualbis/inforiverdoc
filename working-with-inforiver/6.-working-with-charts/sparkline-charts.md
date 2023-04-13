# Sparkline charts

A sparkline is typically used to show trends in a series of values over time, such as stock prices or website traffic. Sparklines are often used in dashboards and other data visualizations to provide a  quick and condensed view of a data series.

Inforiver provides _line, area, baseline, column_s, and _win-loss_ sparkline charts.

## 1. Adding the chart

In this example, we have 12 months of data across regions and categories and we want to visualize using a column sparkline chart.

a) To insert a sparkline chart, you need to add a time dimension in the column field. Note that we have added 'Month' in the 'Columns' field in the Visualization pane.&#x20;

<figure><img src="../../.gitbook/assets/sparkline-select.png" alt=""><figcaption><p>Data mapping</p></figcaption></figure>

b) Select a column for which you want to insert the sparkline chart. In the following image, the 2022 Actuals for the month Jan has been selected.&#x20;

The sparkline chart option gets enabled. From the 'Sparkline chart' drop-down, select the 'Column sparkline chart'.&#x20;

<figure><img src="../../.gitbook/assets/sparkline-column-chart-type-selection.png" alt=""><figcaption><p>Column and chart type selection</p></figcaption></figure>

c) The spark column appears incorporating data for all the months. You can see the _minimum_ and _maximum_ values for each row in _red_ and _green_. You can see the 'Customize' tab in the toolbar and the following [customization options](sparkline-charts.md#2.-customization-options).

<figure><img src="../../.gitbook/assets/sparkline-cistomization-option.png" alt=""><figcaption><p>Sparkline customization options</p></figcaption></figure>

{% hint style="info" %}
You can select a **subset of the columns** using Shift/Ctrl + Click if you do not want to visualize all the periods as a sparkline.
{% endhint %}

## 2. Customization options

The following options are available for customizing a sparkline chart.

{% hint style="info" %}
Depending on the type of sparkline chart chosen, some of these options may or may not be available.
{% endhint %}

### **i) Sparkline**&#x20;

You can change your current sparkline chart type by clicking on the drop-down arrow in the 'Sparkline' section. In the image below, we have changed the chart type from '_Column sparkline_' to '_Baseline_'.

<figure><img src="../../.gitbook/assets/sparkline-chart-type (1).png" alt=""><figcaption><p>Sparkline chart type options</p></figcaption></figure>

### **ii) Marker**&#x20;

From the 'Marker' drop-down, you can select the type of marker points you want to insert in your chart. Adding marker points in your chart helps you to analyze and understand the data better. You can insert marker for:

* **All points** - All the points in the chart
* **None** - No points at all
* **Min, Max, First, Last** - Only for the minimum, maximum, first, and last values in the chart
* **Min, Max** - Only for the minimum and maximum values
* **First, Last** - Only for the first and last values
* **Max** - Only for the maximum value
* **Last** - Only for the last value

<figure><img src="../../.gitbook/assets/sparkline-marker-type.png" alt=""><figcaption><p>Sparkline marker type</p></figcaption></figure>

### **iii) Scale bands**&#x20;

'Scale bands' visually display information about the overall distribution of values. If the distribution of values falls in the _first quartile (0-25%)_, then it is represented by a _lighter shade of gray_. However, if the value distribution falls in the _last quartile (75-100%)_, then it is represented by a _darker shade of gray_.&#x20;

{% hint style="info" %}
The scale bands option is available only if you select any of the standard sparkline chart types (_Line Linear, Line Spline,_ or _Line Stepped_).
{% endhint %}

<figure><img src="../../.gitbook/assets/sparkline-scale-band (1).png" alt=""><figcaption><p>Sparkline scale band</p></figcaption></figure>

### **iv) Show column**&#x20;

From the 'Show column' section, you can choose whether to show the _Min, Max, Avg,_ or _Sum_ columns or _All children (enabled by default)._ In the below image, the _Avg_ and _Min_ columns are enabled in the Show Column option, and the report shows the Min and Average columns.

<figure><img src="../../.gitbook/assets/sparkline-show-column (1).png" alt=""><figcaption><p>Sparkline show column</p></figcaption></figure>

### **v) Axis config**&#x20;

You can configure the _type_ and _style_ of the axis line from the 'Axis config' option. Clicking on the 'Axis Config' option will open up the Axis config modal, in which you can choose the type and style of the axis.

{% hint style="info" %}
The axis config option is available only for the _baseline_ chart.
{% endhint %}

<figure><img src="../../.gitbook/assets/sparkline-axis-config (1).png" alt=""><figcaption></figcaption></figure>

**Type** - An axis in a chart basically serves as a reference making it easy to interpret other data values with respect to it. Depending on the axis type you choose, the axis will get displayed at the

* **Median** - Median value of the data set
* **Average** - Average value of the data set
* **Mid value** - Mid value of the data set
* **Standard deviation** - Standard deviation of the data set
* **Custom** - When the custom option is chosen, you can define a custom value for the axis as shown below.

<figure><img src="../../.gitbook/assets/Custom axis.png" alt=""><figcaption><p>Custom axis configuration</p></figcaption></figure>

**Style** - This option lets you configure how the axis line of the chart should look like. You can select any of the following styles for the axis line - _Solid, Dotted, Dashed, Long dashed_ and _Double solid._

### **vi) Null display**&#x20;

Using the 'Null display' option, you can configure how you want to connect the null values in your dataset. In this example, the 2023 Budget for Feb and May are blank.&#x20;

* **Connect over nulls** - If you select this option, then all the null data points in the dataset will be connected over by lines.&#x20;

<figure><img src="../../.gitbook/assets/Connect over null.png" alt=""><figcaption><p>Connect over nulls</p></figcaption></figure>

* **Consider null as 0** - All the null values in the dataset will be considered '_0' (Zero)_

<figure><img src="../../.gitbook/assets/Consider null as 0.png" alt=""><figcaption><p>Consider null as 0</p></figcaption></figure>

* **Skip the nulls** - All the null values will be skipped

### **vii) Padding**&#x20;

Using the 'Padding' option, you can change the padding/spacing between the bars. The default padding value is 5.

{% hint style="info" %}
The padding option is available only for the _Column_ and _Win/Loss_ Sparklines.
{% endhint %}

<figure><img src="../../.gitbook/assets/sparkline-padding.png" alt=""><figcaption><p>Sparkline padding option</p></figcaption></figure>

### viii) Appearance

This option lets you change the appearance of the sparkline charts. Clicking on this option will open up an 'Appearance' model in which you can configure the following properties:

<figure><img src="../../.gitbook/assets/sparkline-appearance.png" alt=""><figcaption><p>Sparkline appearance option</p></figcaption></figure>

**a) Apply default theme** - Enabling this option will apply default power BI themes and colors to your sparkline charts

<figure><img src="../../.gitbook/assets/sparkline-default-theme.png" alt=""><figcaption><p>Sparklinee default theme</p></figcaption></figure>

**b) Stroke width** - With this option, you can configure the width of the stroke of your sparkline charts. The default is 1.

<figure><img src="../../.gitbook/assets/sparkline-stroke-width.png" alt=""><figcaption><p>Sparkline stroke width</p></figcaption></figure>

**c) Base color** - Using this option you can configure the base color of the strokes of the sparkline charts

**d) Max** - This option lets you set the color of the maximum point in the chart

**e) Min** - This option lets you configure the color of the minimum point in the chart

**f) Label** - This option lets you configure the color of the data label in the chart

**g) Apply gradient** - With this option, you can enable or disable the gradient coloring. If you enable this option, two additional options become available. The 'Area above 1' and 'Area above 2' using which you can set the starting and ending colors for the area above the axis.

<figure><img src="../../.gitbook/assets/sparkline-gradient.png" alt=""><figcaption><p>Sparkline apply gradient</p></figcaption></figure>

**h) Line above** - With this option, you can set the color of the line above the axis

**i) Line below** - With this option, you can set the color of the line below the axis

**j) Area above** - With this option you can customize the color of the area above the axis

**k) Area below** - With this option you can customize the color of the area below the axis

<figure><img src="../../.gitbook/assets/sparkline-color-options.png" alt=""><figcaption><p>Sparkline color options</p></figcaption></figure>

**l) Axis color** - This option lets you customize the color of the axis line

**m) Positive color** - Using this option you can customize the positive color of the bar

**n) Negative color** - Using this option you can customize the negative color of the bar

<figure><img src="../../.gitbook/assets/sparkline-axis-color.png" alt=""><figcaption><p>Variance color option</p></figcaption></figure>

### viii) Show label&#x20;

You can configure whether to show or hide data labels using this option. Data labels are shown by default. Clicking on this option once will hide the data labels and clicking again will show the labels.

<figure><img src="../../.gitbook/assets/sparkline-show-llabel.png" alt=""><figcaption><p>Sparkline show label</p></figcaption></figure>

### **ix) Remove sparkline**&#x20;

Clicking on the 'Remove sparkline' option removes the sparkline chart from the report and restores it to the original number format.

<figure><img src="../../.gitbook/assets/remove-sparkline (2).png" alt=""><figcaption><p>Remove sparkline chart</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/remove-chart.png" alt=""><figcaption><p>After chart removal</p></figcaption></figure>

In this section, we covered the sparkline charts. Navigate to the next section to learn more about [stacked charts](stacked-charts.md).&#x20;
