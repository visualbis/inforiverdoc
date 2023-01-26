# Waterfall charts

A waterfall chart is a type of chart that is used to display how an initial value is affected by a series of intermediate positive or negative values, leading to a final value. It is often used to show the breakdown of the total change in a value, such as a financial metric like net income or cash flow.&#x20;

Waterfall charts are often used in finance and accounting to show the flow of money in and out of a business, but can also be used in other industries such as manufacturing, sales, and production.

Inforiver offers 3 variations of the waterfall chart: _Solid, Colored,_ and _Invert Colored._

* **Solid waterfall** - All the bars are represented by the same solid color.&#x20;
* **Colored waterfall** - By default, the positive and negative values are represented using green and red bars, but they can be customized.
* **Invert colored waterfall** - This chart type is the exact opposite of the colored waterfall chart. The positive and negative values are represented using red and green bars, but they can be customized.

## 1. Adding the chart

In this example, we will visualize the contribution of the subcategories to the total margin using a waterfall chart.

a) We have added 'SubCategory' in the 'Rows' field and 'Total cost', 'Sales', 'Margin', 'Margin %', and 'Total customers' in the 'Values (AC)' field in the visualization pane.

<figure><img src="../../.gitbook/assets/waterfall-chart-pane.png" alt=""><figcaption><p>Data mapping</p></figcaption></figure>

b) Select the column for which you want to insert the waterfall chart. In the following image, the margin column has been selected.

The waterfall chart option gets enabled. From the 'Waterfall chart' drop-down, select the 'Colored waterfall chart'.&#x20;

<figure><img src="../../.gitbook/assets/waterfall-chart-selection (2).png" alt=""><figcaption><p>Column and chart type selection</p></figcaption></figure>

c) The waterfall chart gets inserted as shown below. You can see the 'Customize' tab in the toolbar and the following [customization options](waterfall-charts.md#2.-customization-options).

<figure><img src="../../.gitbook/assets/waterfall-chart.png" alt=""><figcaption><p>Inserting a waterfall chart</p></figcaption></figure>

## 2. Customization options

Inserting a waterfall chart will open up the following customization options.

### **i) Waterfall chart type**&#x20;

You can change your current waterfall chart type from this drop-down.

<figure><img src="../../.gitbook/assets/waterfall-chart-type.png" alt=""><figcaption><p>Waterfall chart type customization</p></figcaption></figure>

### **ii) Continuous**&#x20;

Enabling this option will display a continuous waterfall chart across row hierarchies.

{% hint style="info" %}
The 'Continuous' option is available only if the selected column has a row hierarchy.
{% endhint %}

To create a row hierarchy, we have added the 'Category' in the 'Rows' field in the Visualization pane.

<figure><img src="../../.gitbook/assets/waterfallchart-visualization-pane (1).png" alt=""><figcaption><p>Data mapping</p></figcaption></figure>

Select the 'Sales' column, and from the 'Waterfall chart' drop-down, select the 'Colored waterfall chart'.  The waterfall chart gets inserted as shown below.

<figure><img src="../../.gitbook/assets/waterfall-chart-insertion.png" alt=""><figcaption><p>Waterfall chart insertion with row hierarchy</p></figcaption></figure>

The continuous option now becomes available under the 'Customize' tab. Enabling this option will display a continuous waterfall chart as shown in the image below.

<figure><img src="../../.gitbook/assets/continuous-waterfall-insertion (2).png" alt=""><figcaption><p>Inseerting a continuous waterfall chart</p></figcaption></figure>

### **iii) Axis config**&#x20;

This option lets you configure the axis-related settings. Clicking on this option opens up an 'Axis' modal from which you can choose to&#x20;

* **Show Y-axis** - Enabling this option will display the Y-axis on the chart
* **Show X-axis** - Enabling this option will display the X-axis on the chart
* **Hide ticks** - Enabling this option will hide the tick intervals on the axis

{% hint style="info" %}
Note that some of these options may not be enabled for you depending on the type of waterfall chart inserted and the properties chosen.
{% endhint %}

<figure><img src="../../.gitbook/assets/waterfall-axis-config.png" alt=""><figcaption><p>Watefall axis config configuration</p></figcaption></figure>

### **iv) Data label config**&#x20;

This option lets you configure the arrangement and display properties for data labels. The modal has the following properties:

* **Data label** - You can enable or disable this checkbox to show or hide data labels for the chosen column/metrics.&#x20;

{% hint style="info" %}
The 'Show label' and 'Percentage scaling' options are available only if the 'Data label' option is enabled.
{% endhint %}

* **Show label** - Inforiver provides the option to display the data labels simply as _labels_, _percentages_, or _both_. In the below example, we have chosen the 'Both' option.
* **Percentage scaling** - Using this option you can configure the scaling of the percentage data label. The available scaling options are
  1. **Universal -** This is the default option and it indicates the percentage contribution of the value to the grand total.
  2. **By level -** Whereas 'By level' indicates the percentage contribution of the value to its parent level or category.

{% hint style="info" %}
The 'Percentage scaling' option becomes available, only if the 'Show label' value is set to either 'Percentage' or 'Both'.
{% endhint %}

<figure><img src="../../.gitbook/assets/waterfall-show-datalabel.png" alt=""><figcaption><p>Waterfall chart data label configuration</p></figcaption></figure>

### **v) Fill pattern**&#x20;

You can customize the fill pattern of the bar to any of these IBCS notations: _Solid, Outlined,_ or _Hatched_.

<figure><img src="../../.gitbook/assets/waterfall-fill-pattern.png" alt=""><figcaption><p>Waterfall chart fill pattern</p></figcaption></figure>

### vi) Appearance

This option lets you change the appearance of the waterfall charts. Clicking on this option will display a 'Colors' or 'Series Display' sub-option (depending on the type/variant of the chart inserted). Clicking on either of these sub-options will open up an 'Appearance' model in which you can configure the following properties:

<figure><img src="https://lh3.googleusercontent.com/IDWvOtcckB8KokeXzdnOuBJ8ZM-5h09qhiu4ka2QYYcuAH9hM9jB1PICKca4cVG-msK3HFz9xAjues-CpdxN_y-BBu-Y5FpbHzODRYdd63lAoJHNu_bcPiSIvvEsdjo1ZI3P2bIi9VocbK-5CFAEcf0JzY_jPmcfrzSIDtwSuKbPiG71hRWFFftZxeWUBw" alt=""><figcaption><p>Appearance modal</p></figcaption></figure>

{% hint style="info" %}
Some of these properties/options may or may not be available depending on the inserted chart type and variant.
{% endhint %}

**a) Positive color** - Using this option you can customize the positive color of the bar/marker

**b) Negative color** - Using this option you can customize the negative color of the bar/marker

**c) Axis color** - This option lets you set the axis color of the chart

<figure><img src="https://lh5.googleusercontent.com/h9W4sxojkezlcffIknQQOnGLv8-u6gJDjpwwrU4g809oMAy_FRrbMJkX-Gn37Ugt-q-ewrh2IdS1kbzSBT7X9ou-tqdMPmN0sZYs6lB3yGteuZ8vGwNgjYm-ltIRYfDGHdiNhCF4JmH2WTELJGE1d3L2mMGWFfj8sWCL-FDlFkfoZrqHTRXVrfnPuXxBLw" alt=""><figcaption><p>Variance and axis color options</p></figcaption></figure>

**d) Data label color** - This option lets you set the color of the data labels in the chart

{% hint style="info" %}
The following properties are present in the 'Series Display' option available under the 'Appearance' option of **waterfall charts**.
{% endhint %}

**e) Bar color** - This option is available only for solid bar charts and will let you customize the color of the bar.

**f) Gradient** - Enabling this option will allow you to set a gradient color to your bar chart. If you enable this option, the Min and Max color options become available using which you can set the color for the min value and the max value.

<figure><img src="https://lh4.googleusercontent.com/YpwW5fsQqD3hU3as9s6z_jsmv30VQC1OxrVEhYl7E9L3AZHb-2doU2pSWd3ZBOguy1RAfyv6XOwcCIjF16xUkVYhzVNiKjEeTpwuSJTK11r_EU6MeIsDnC42ZWRyUMiCs44M5SMqaGC7m2yonYeimK_9ncLeLt9CFmfC_3B2e0bTOz_rgRyV3lDw2h31AA" alt=""><figcaption><p>Appearance series display options</p></figcaption></figure>

In this section, we covered waterfall charts. Navigate to the next section to learn more about the [bar and pin charts](bar-and-pin-charts.md).

#### Resources

[Waterfall charts: A finance professional's best friend](https://inforiver.com/insights/waterfall-charts-finance-professionals-best-friend/)
