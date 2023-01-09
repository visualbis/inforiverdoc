# Basic inline charts

With Inforiver, you can deliver a range of charts and visualizations in your matrix reports in a single click. The available chart options are shown in the below image.

<figure><img src="../../.gitbook/assets/2.5.1 Charts overview.png" alt=""><figcaption><p>40+ charts and visualizations </p></figcaption></figure>

## Overview

1. **Trend** - Incorporate **sparklines, spark columns**, and their variants such as the win-loss trend to capture performance over time
2. **Performance** - Utilize different types of **bullet charts**, including the normalized bullet visualization (proposed by International Business Communication Standards)
3. **Distribution** - Highlight distribution across categories using **stacked charts and waterfall** visualizations
4. **Magnitude** - Deliver **bar, lollipop & pin** **charts, and data bars** for highlighting the magnitude and significance
5. **Changes/deviation** - Track changes over time or with respect to benchmark by using **dot plot, arrow plot, dumbbell plot & range plot** charts
6. **Comparison** - Compare multiple measures and visualize absolute and relative variances using **colored bar & lollipop/pin** charts&#x20;
7. **KPI cards** - Insert **KPI cards** in a single click using the available presets; cards can be customized further
8. **Blend columns/KPIs -** Blend **two measures in a single column** along with formatting, including conditional formatting&#x20;

{% hint style="info" %}
In this section, only the basics of charts will be covered. For advanced customizations, visit [working with charts](../6.-working-with-charts.md).
{% endhint %}

## 1. Trend

You can insert sparklines and their variants in a single click for visualizing data across time periods. There are 9 variants available in Inforiver.

In the below example, we have 12 months of data across regions and categories.&#x20;

a) Click on the 'Sparkline' icon highlighted and choose the 'Column sparkline'.&#x20;

<figure><img src="../../.gitbook/assets/2.5.2 sparkline.png" alt=""><figcaption><p>Sparkline and its variants</p></figcaption></figure>

b) The spark column appears incorporating data for all the months. You can see the minimum and maximum values for each row in red and green.&#x20;

In the toolbar, you can see the 'Customize' tab which gets enabled. We'll cover these toolbar options in a later section.

<figure><img src="../../.gitbook/assets/2.5.3 sparkline.png" alt=""><figcaption><p>Sparkline customization options</p></figcaption></figure>

## 2. Performance

Inforiver provides 2 and 3-value bullet charts and a clustered bar for visualizing performance.

### i) 2-value bullet charts

In this example, we have 2022 Actuals and Plan across regions and categories.&#x20;

a) Select the 2 measures and click on the 'Bullet' icon and select the 'Integrated variance bar' as highlighted.

<figure><img src="../../.gitbook/assets/2.5.4 2 value bullet.png" alt=""><figcaption><p>Bullet chart variants</p></figcaption></figure>

b) The bullet chart gets inserted showing a comparison of the two measures. The variance between actuals and plan is shown in red/green.

<figure><img src="../../.gitbook/assets/2.5.5 2 value bullet.png" alt=""><figcaption><p>Bullet chart customization options</p></figcaption></figure>

### ii) 3-value bullet charts

a) To enable the 3-value bullets, add one more measure as shown below. We'll choose the 'Bullet with marker' as highlighted.

<figure><img src="../../.gitbook/assets/2.5.6 3 value bullet.png" alt=""><figcaption><p>3-value bullet variants</p></figcaption></figure>

b) This type of bullet chart also displays the comparison band. The legend is highlighted below. These options can be customized from the toolbar.

<figure><img src="../../.gitbook/assets/2.5.7 3 value bullet.png" alt=""><figcaption><p>Bullet with marker</p></figcaption></figure>

### iii) Clustered bars

The clustered bar is applicable only when using one of these 4 bullet variants - Stephen Few's Qualitative bullet, Qualitative bullet with marker, Comparative bullet, and Bullet with marker.

a) Click on 'Series display' in the 'Customize' tab. Change the '**Additional target**' to '**Bar**' instead of 'Line'.

In the popup screen, enable 'Clustered bar'.

<figure><img src="../../.gitbook/assets/2.5.8 clustered bar.png" alt=""><figcaption><p>Enabling clustered bar</p></figcaption></figure>

b) The clustered bar gets applied.

<figure><img src="../../.gitbook/assets/2.5.9 clustered bar.png" alt=""><figcaption><p>Clustered bar</p></figcaption></figure>

## 3. Distribution

### i) Stacked charts

In this example, we have 2022 actuals across regions. Let's use a stacked chart to see the composition based on subcategories for the regions.

a) Select all the subcategory columns and click on the 'Bullet' icon. There are 2 options - A stacked bar and a percentage stacked bar.&#x20;

<figure><img src="../../.gitbook/assets/2.5.13 stacked chart.png" alt=""><figcaption><p>Stacked chart options</p></figcaption></figure>

b) Select the percentage stacked bar. The chart gets added.&#x20;

<figure><img src="../../.gitbook/assets/2.5.14 stacked chart.png" alt=""><figcaption><p>Percentage stacked bar</p></figcaption></figure>

c) Let's hide the subcategory columns. In the toolbar, click on the 'Manage columns' toolbar. Uncheck the highlighted measure - 2022 Actuals.

<figure><img src="../../.gitbook/assets/2.5.15 stacked chart.png" alt=""><figcaption><p>Hide subcategory columns</p></figcaption></figure>

d) Select the column with the chart and drag using the arrow next to the column header to resize. There are a number of customization options available, which will be covered in a later section.

<figure><img src="../../.gitbook/assets/2.5.16 stacked chart.png" alt=""><figcaption><p>Resize the chart</p></figcaption></figure>

### ii) Waterfall charts

Let's visualize the contribution of the subcategories to the total margin.

a) Select the 'Margin' column and click on the 'Waterfall' icon. There are 3 options - we'll choose the colored waterfall.

<figure><img src="../../.gitbook/assets/2.5.17 waterfall chart.png" alt=""><figcaption><p>Waterfall chart options</p></figcaption></figure>

b) You can see that the highest positive and negative contributions are from Lamps and Refrigerators respectively.

<figure><img src="../../.gitbook/assets/2.5.18 waterfall chart.png" alt=""><figcaption><p>Waterfall chart to visualize margin contribution</p></figcaption></figure>

### iii) Progress bars

a) To visualize the contribution of each category and subcategory to the total sales using the progress bar, click on the 'Quick formula' dropdown in the 'Insert' tab.

<figure><img src="../../.gitbook/assets/2.5.22 progress bar.png" alt=""><figcaption><p>Inserting contribution %</p></figcaption></figure>

b) Select the '% Contribution to Grand Total' option. In the side panel, check 'Enable bar chart' and click 'Create'.

<figure><img src="../../.gitbook/assets/2.5.23 progress bar.png" alt=""><figcaption><p>Enabling bar chart</p></figcaption></figure>

c) The progress bar gets added. You also have options to customize the display. You can choose to display only the percentage, value, or both. The bar color can also be changed.

<figure><img src="../../.gitbook/assets/2.5.24 progress bar.png" alt=""><figcaption><p>Progress bar</p></figcaption></figure>

## 4. Magnitude

### i) Bar charts

Let's insert a solid bar chart for sales. &#x20;

a) Select the column and click on the highlighted icon.

<figure><img src="../../.gitbook/assets/2.5.25 bar.png" alt=""><figcaption><p>Simple bar chart</p></figcaption></figure>

b) The bar chart gets added. There are a number of customization options such as fill pattern, comparison bands, and axis config.&#x20;

<figure><img src="../../.gitbook/assets/2.5.26 bar.png" alt=""><figcaption><p>Simple bar chart</p></figcaption></figure>

c) Let's apply comparison bands. Click on the 'Comparison bands' icon. A popup screen opens. You can customize the number of bands, and colors, and define bands based on percentage or value. We'll go with the default. Click 'Save'. The bands get applied.

<figure><img src="../../.gitbook/assets/2.5.27 bar.png" alt=""><figcaption><p>Adding a comparison band</p></figcaption></figure>

### ii) Lollipop/pin charts

To visualize Margin%, let's use the lollipop chart.&#x20;

a) Click on the column and then the icon highlighted.

<figure><img src="../../.gitbook/assets/2.5.28 bar.png" alt=""><figcaption><p>Lollipop chart</p></figcaption></figure>

b) The 'Simple lollipop' chart gets inserted.

<figure><img src="../../.gitbook/assets/2.5.29 bar.png" alt=""><figcaption><p>Simple lollipop chart added</p></figcaption></figure>

### iii) Data bars

Let us add data bars for the total customers column.&#x20;

a) In the 'Conditional formatting' dropdown, select 'Data bars' and choose a color. If you would like to use a different color, you can still choose one of them. This selection can be customized in the next step.&#x20;

<figure><img src="../../.gitbook/assets/2.5.31data bar (1).png" alt=""><figcaption><p>Data bar</p></figcaption></figure>

b) On selecting a color, the data bars appear and you can also see a side panel. Here you can apply customizations such as applying data bars based on a different measure, applying to totals, and so on.

<figure><img src="../../.gitbook/assets/2.5.32 data bar.png" alt=""><figcaption><p>Data bar customizations</p></figcaption></figure>

## 5. Changes/deviation

In this example, let's visualize the pay gap between men and women in UK and US.

a) Select the two measures - average salary of men and women. Click on the 'Bullet' icon and select the 'Dot plot' icon highlighted.&#x20;

<figure><img src="../../.gitbook/assets/2.5.19 dot plot.png" alt=""><figcaption><p>Chart options for visualizing changes/deviation</p></figcaption></figure>

b) The dot plot gets inserted.&#x20;

<figure><img src="../../.gitbook/assets/2.5.20 dot plot.png" alt=""><figcaption><p>Dot plot</p></figcaption></figure>

c) Let's hide the salary columns and resize the dot plot.&#x20;

You can insert an axis for easy comprehension. In the 'Customize' tab, click on the 'Show axis' option.

<figure><img src="../../.gitbook/assets/2.5.21 dot plot.png" alt=""><figcaption><p>Show axis</p></figcaption></figure>

## 6. Comparison

In this example, let's compare current sales and prior year sales.&#x20;

a) Assign 2022 Actuals to 'Values (AC)' and 2021 Actuals to 'Compare to prior period (PY)'.

<figure><img src="../../.gitbook/assets/2.5.33 comparison.png" alt=""><figcaption><p>Assigning AC and PY</p></figcaption></figure>

b) In the 'Home' tab, click on the 'Manage columns' dropdown. You can see 2 new columns created automatically - (2022 Actuals - 2021 Actuals) and (2022 Actuals - 2021 Actuals)%. Click on the checkboxes to enable these columns.

<figure><img src="../../.gitbook/assets/2.5.34 comparison.png" alt=""><figcaption><p>Variance and variance % columns</p></figcaption></figure>

Let us now add the bar and pin charts for the absolute and relative variances respectively.

### i) Bar charts

a) Select the variance column and click on the 'Bar' chart icon. Select the 'Colored bar'.&#x20;

<figure><img src="../../.gitbook/assets/2.5.35 comparison.png" alt=""><figcaption><p>Inserting colored bar for variance</p></figcaption></figure>

b) The bar chart gets inserted. Note that the positive variances are highlighted in green and the negative variances in red. For the cases where the reverse is true, 'Invert colored bar' can be used.

<figure><img src="../../.gitbook/assets/2.5.36 comparison.png" alt=""><figcaption><p>Variance using bar chart</p></figcaption></figure>

### ii) Lollipop/pin charts

To visualize (2022 Actuals - 2021 Actuals)%, let's use the lollipop chart.&#x20;

a) Click on the column and then the icon highlighted.

<figure><img src="../../.gitbook/assets/2.5.37 comparison.png" alt=""><figcaption><p>Inserting bar colored lollipop for variance%</p></figcaption></figure>

b) The 'Bar colored lollipop' chart gets inserted.

<figure><img src="../../.gitbook/assets/2.5.38 comparison.png" alt=""><figcaption><p>Variance% using lollipop chart</p></figcaption></figure>

## 7. KPI cards

Inforiver provides a number of KPI card presets which can be customized as required. You can also create KPI cards from scratch.

Let's insert a KPI card in this report.&#x20;

a) Hover over the header and click on the '6 dots' icon. Click on 'Preset'.

<figure><img src="../../.gitbook/assets/2.5.39 kpi card.png" alt=""><figcaption><p>Editing header</p></figcaption></figure>

b) The 'Header & footer' tab opens up as shown below. There are a number of 'Header presets' to choose from. The 5th header preset features 2 KPI cards. But let us create a KPI card using a KPI preset. &#x20;

Click on the dropdown as highlighted and select 'KPI'.

<figure><img src="../../.gitbook/assets/2.5.40 kpi card.png" alt=""><figcaption><p>Header footer customization screen</p></figcaption></figure>

c) Click 'Proceed'.

<figure><img src="../../.gitbook/assets/2.5.41 kpi card.png" alt=""><figcaption><p>Warning message</p></figcaption></figure>

d) A simple KPI card gets inserted. Let us see how to insert a preset.

<figure><img src="../../.gitbook/assets/2.5.42 kpi card.png" alt=""><figcaption><p>Simple KPI card</p></figcaption></figure>

e) Click on 'KPI presets'. The KPI preset panel opens up. Go to the 'Combo' tab and select the preset highlighted below.

<figure><img src="../../.gitbook/assets/2.5.43 kpi card.png" alt=""><figcaption><p>KPI presets</p></figcaption></figure>

f) Click 'Proceed'.

<figure><img src="../../.gitbook/assets/2.5.44 kpi card.png" alt=""><figcaption><p>Warning message</p></figcaption></figure>

g) The selected KPI preset gets applied. Let's now edit the KPI card to display the variances as desired. Close the side panel.&#x20;

<figure><img src="../../.gitbook/assets/2.5.45 kpi card.png" alt=""><figcaption><p>KPI preset gets inserted</p></figcaption></figure>

h) Ideally, 2022 Actuals should be displayed on the top followed by 2022 Plan and 2021 Actuals and their variances.&#x20;

In the floating toolbar, click on the 'Data selection' icon highlighted. The matrix is no longer greyed out.&#x20;

Select the grand total cells in the order shown in the below image by using Shift+Click. The KPI card gets updated.

<figure><img src="../../.gitbook/assets/2.5.46 kpi card.png" alt=""><figcaption><p>Selecting data to display in KPI cards</p></figcaption></figure>

i) KPI cards can be resized by hovering on the container border and dragging it to the desired size. Click on 'Close editor' as highlighted.

<figure><img src="../../.gitbook/assets/2.5.47 kpi card.png" alt=""><figcaption><p>Resize KPI cards</p></figcaption></figure>

j) The KPI card is shown below.

<figure><img src="../../.gitbook/assets/2.5.48 kpi card.png" alt=""><figcaption><p>KPI card inserted</p></figcaption></figure>

## 8. Blend columns/KPIs

Let's blend the Sales and Margin% columns in a single column.&#x20;

a) In the 'Insert' tab, click on the 'Blend' option in the 'Column' section. A blank measure gets inserted and the 'Blend measure' side panel opens.&#x20;

Enter the title and select the measures as shown from the dropdown. Click 'Create'.

<figure><img src="../../.gitbook/assets/2.5.10 blend kpi.png" alt=""><figcaption><p>Blend measures side panel</p></figcaption></figure>

b) The columns are blended to create a single column. Note that Margin % is displayed below Sales. This is because we have used the default 'Vertical' as 'Blend direction'.

<figure><img src="../../.gitbook/assets/2.5.11 blend kpi.png" alt=""><figcaption><p>Blend measures vertically</p></figcaption></figure>

c) If you want to display in a horizontal orientation, change the 'Blend direction' to 'Horizontal'.

<figure><img src="../../.gitbook/assets/2.5.12 blend kpi.png" alt=""><figcaption><p>Blend measures horizontally</p></figcaption></figure>

There are several customization options available for the charts and visualizations which will be covered in [working with charts](../6.-working-with-charts.md).
