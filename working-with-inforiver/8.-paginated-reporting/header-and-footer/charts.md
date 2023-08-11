# Charts

In the header and footer, you can add all the inline charts such as sparklines, bullets, range plots, dot plots, and other unique charts such as donut charts and progress bars. Let's take a detailed look.&#x20;

## 1. Adding the chart

a) Click on 'Header & footer' in the 'Design' tab.

<figure><img src="../../../.gitbook/assets/image (123).png" alt=""><figcaption><p>Editing the header</p></figcaption></figure>

b) Choose 'Chart' from the 'Type' option.

<figure><img src="../../../.gitbook/assets/image (118).png" alt=""><figcaption><p>Choosing the chart element</p></figcaption></figure>

c) By default, a donut chart gets inserted based on the data fields added to the report. Here we have a donut chart for the 4 quarters.

<figure><img src="../../../.gitbook/assets/image (116).png" alt=""><figcaption><p>Default chart gets inserted</p></figcaption></figure>

d) You can see the customization options present in the 'Customize' tab. Appearance and Legend config are covered in [customization options](charts.md#4.-customization-options).

<figure><img src="../../../.gitbook/assets/image (127).png" alt=""><figcaption><p>Customization options</p></figcaption></figure>

## 2. Data selection

Note that by default, the table is greyed out as shown in the image.

<figure><img src="../../../.gitbook/assets/image (129).png" alt=""><figcaption><p>Table is greyed out</p></figcaption></figure>

On hovering over the chart, the  data selection button appears.&#x20;

<figure><img src="../../../.gitbook/assets/image (122).png" alt=""><figcaption><p>Change data icon</p></figcaption></figure>

Click on the change data symbol to open the 'Data Selection' dialog box. The data source used to render the chart can be set using the methods listed below:

&#x20; a) Using data from rows

&#x20; b) Using data from columns

&#x20; c) Manually selecting the cells required for the chart

### **a)  Data from rows**

1. To render the chart using row data, click on the 'Select Rows' dropdown.

<figure><img src="../../../.gitbook/assets/image (151).png" alt=""><figcaption><p>Select rows option</p></figcaption></figure>

2. The 'Select Rows' dialog box opens. You can select the rows that will contribute to rendering the chart.

{% hint style="info" %}
Click on the 'Clear' link to reset and remove all the selected rows
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (121).png" alt=""><figcaption><p>Choosing rows to render the chart</p></figcaption></figure>

3. After clicking on 'OK', the selected categories are displayed in the Data Selection dialog box. Click on 'Create' to render the chart.&#x20;

Notice that the rows that are used as data source for the chart have been highlighted.

<figure><img src="../../../.gitbook/assets/image (117).png" alt=""><figcaption><p>Chart rendered using row level data</p></figcaption></figure>

### **b)  Data from columns**

1. To render the chart using column data, click on the 'Select Columns/Measures' dropdown.

<figure><img src="../../../.gitbook/assets/image (152).png" alt=""><figcaption></figcaption></figure>

2. Select the columns and/or measures that will be used to render the chart.

{% hint style="info" %}
Click on 'Clear' to reset and remove the columns that have been selected.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (124).png" alt=""><figcaption><p>Columns and measures selected to render the chart</p></figcaption></figure>

After clicking on 'OK', the columns that are selected are displayed in the Data Selection dialog box. Click on 'Create' to render the chart.

Notice that the columns that are used as data source for the chart have been highlighted.

<figure><img src="../../../.gitbook/assets/image (153).png" alt=""><figcaption><p>Chart rendered using columns or measures</p></figcaption></figure>

### &#x20;c**) Manual data selection**

1. To render the chart using manual data selection, click on the 'Manual Selection' link.

<figure><img src="../../../.gitbook/assets/image (154).png" alt=""><figcaption><p>Manual selection option</p></figcaption></figure>

2\. From the grid, select the cells to be used as data source for the chart, the selection is immediately reflected in the header chart.

<figure><img src="../../../.gitbook/assets/image (155).png" alt=""><figcaption></figcaption></figure>

## 3. Chart types

There are a number of chart types like Donut, Sparkline, Bullet etc. that can be inserted in the header. Let's see how to add or change them.&#x20;

a) By default, a donut chart is added to the header if the Chart option is selected. This can be changed from the Data Selection dialog box.

{% hint style="warning" %}
Some of the variants are not shown here but they can be accessed from the toolbar.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (145).png" alt=""><figcaption><p>Chart type selection</p></figcaption></figure>

The donut chart has now been changed to a Sparkline chart.

<figure><img src="../../../.gitbook/assets/image (146).png" alt=""><figcaption><p>Chart updated to Sparkline</p></figcaption></figure>

b) To easily browse the chart types and variants available, click on the 'Right arrow' in the cell as shown in the image. Notice that in the toolbar it says 'SparkLine'.&#x20;

<figure><img src="../../../.gitbook/assets/image (147).png" alt=""><figcaption><p>Browsing chart types</p></figcaption></figure>

The chart has now been changed to a bar chart.

<figure><img src="../../../.gitbook/assets/image (148).png" alt=""><figcaption><p>Changing the chart to a bar chart</p></figcaption></figure>

c) You can also view and select all the supported chart types and their variants from the toolbar as shown in the image below.

<figure><img src="../../../.gitbook/assets/image (149).png" alt=""><figcaption><p>Selecting the chart from the toolbar</p></figcaption></figure>

d) In case two data points are selected, you can also use variants of the progress bar such as conditional bar, angular bar and donut bar.

<figure><img src="../../../.gitbook/assets/image (144).png" alt=""><figcaption><p>Progress bar </p></figcaption></figure>



## 4. Customization options

Most of the customization options are already covered in [working with charts](../../6.-working-with-charts.md). The customization options unique to header charts are covered here.&#x20;

### a) All chart types

#### Legend config

By default, the legend is shown on the right of the chart, you can change the position to the left or turn it off. To change the legend, click on the 'Legend config' button in the Customize ribbon.&#x20;

<figure><img src="../../../.gitbook/assets/image (132).png" alt=""><figcaption><p>Legend config for header charts</p></figcaption></figure>

When the legend is turned off, the chart will be rendered as shown in the image below.

<figure><img src="../../../.gitbook/assets/image (133).png" alt=""><figcaption><p>Legend disabled</p></figcaption></figure>

### b) Styling donut chart

The appearance of the donut chart can be customized by clicking on the 'Appearance' option. You can see the dialog box shown in the image where you can select the color for each arc, arc size and apply a gradient.

<figure><img src="../../../.gitbook/assets/image (134).png" alt=""><figcaption><p>Appearance customizations</p></figcaption></figure>

* When a **gradient** is applied, you can select the gradient color and the chart gets updated as shown.

<figure><img src="../../../.gitbook/assets/image (135).png" alt=""><figcaption><p>Gradient applied</p></figcaption></figure>

* When there are more than 5 categories selected, the '**Enable others**' option is activated. Note that even though six regions were selected, only five are displayed in the chart. When the 'Enable others' property is set, you can see a segment in the donut called 'Others' which visualizes the sum of the values apart from the top 5 categories. That is, if there are 10 categories added, the last 5 categories will be consolidated and shown as 'Others'.

<figure><img src="../../../.gitbook/assets/image (136).png" alt=""><figcaption><p>Enable others</p></figcaption></figure>



* The name 'Others' can be modified by clicking on the 'Pencil' icon and entering a relevant name in the text field.

<figure><img src="../../../.gitbook/assets/image (137).png" alt=""><figcaption><p>Customizing the 'Others' category</p></figcaption></figure>

* &#x20;The **arc size** can be customized by using the 'Arc size' dropdown. The available options are Small, Medium, Large and Extra large.

<figure><img src="../../../.gitbook/assets/image (139).png" alt=""><figcaption><p>Changing the arc size</p></figcaption></figure>

### c) Styling progress bars

Progress bar appearance can be customized as shown below. You can define positive and negative colors using a color picker.

<figure><img src="../../../.gitbook/assets/image (140).png" alt=""><figcaption><p>Setting the color scheme for progress bars</p></figcaption></figure>

### d) Styling sparklines

In the sparkline customization toolbar, explanations for [Appearance](../../6.-working-with-charts/sparkline-charts.md#viii-appearance), [Null display](../../6.-working-with-charts/sparkline-charts.md#vi-null-display), [Marker](../../6.-working-with-charts/sparkline-charts.md#ii-marker) and [Show label](../../6.-working-with-charts/sparkline-charts.md#viii-show-label) are covered in the '[Working with charts](../../6.-working-with-charts.md)' section.

Let's look at the 'Data config' option.

i) Select the row grand total and choose the sparkline chart type with the area spline variant. You can see the sparkline chart in the header as shown below.&#x20;

<figure><img src="../../../.gitbook/assets/image (141).png" alt=""><figcaption><p>Sparkline on selecting a row</p></figcaption></figure>

ii) Click on 'Data config'. In the dialog box, you can see that all the measures are selected. Let's display only the Unit Price measure in the header. Uncheck the other checkboxes. Select a different color using the color picker if needed. Notice how the chart gets updated.&#x20;

<figure><img src="../../../.gitbook/assets/image (143).png" alt=""><figcaption><p>Selecting measures and setting the chart color</p></figcaption></figure>



In the next section, we'll be covering adding [KPI cards](kpi-cards.md).
