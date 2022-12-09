# Basic inline charts

With Inforiver, you can deliver a range of charts and visualizations in your matrix reports in a single click. The available chart options are shown in the below image.

<figure><img src="../../.gitbook/assets/2.5.1 Charts overview.png" alt=""><figcaption><p>40+ charts and visualizations </p></figcaption></figure>

## Overview

1. **Trend** - Incorporate **sparklines, spark columns**, and its variants such as win-loss trend to capture performance over time
2. **Performance** - Utilize different types of **bullet charts**, including the normalized bullet visualization (proposed by International Business Communication Standards)
3. **Distribution** - Highlight distribution across categories using **stacked charts and waterfall** visualizations
4. **Magnitude** - Deliver **bar, lollipop & pin** **charts, and data bars** for highlighting the magnitude and significance
5. **Changes/deviation** - Track changes over time or with respect to benchmark by using **dot plot, arrow plot, dumbbell plot & range plot** charts
6. Comparison - Compare multiple measures and visualize absolute and relative variances using **colored bar & lollipop/pin** charts&#x20;
7. KPI cards - Insert **KPI cards** in a single click using the available presets; cards can be customized further
8. **Blend columns/KPIs -** Blend **two measures in a single column** along with formatting, including conditional formatting&#x20;

{% hint style="info" %}
In this section, only the basics of charts will be covered. For advanced customizations, visit [working with charts](../6.-working-with-charts.md).
{% endhint %}

## 1. Trend

You can insert sparklines and their variants in a single click for visualizing data across time periods. There are 9 variants available in Inforiver.

In the below example, we have 12 months of data across regions and categories. Click on the sparkline icon highlighted and choose the column sparkline.&#x20;

<figure><img src="../../.gitbook/assets/2.5.2 sparkline.png" alt=""><figcaption><p>Sparkline and its variants</p></figcaption></figure>

The sparkline chart gets applied. You can see the minimum and maximum values for each row in red and green.&#x20;

In the toolbar, you can see the 'Customize' tab which gets enabled. We'll cover these toolbar options in a later section.

<figure><img src="../../.gitbook/assets/2.5.3 sparkline.png" alt=""><figcaption><p>Sparkline customization options</p></figcaption></figure>

## 2. Performance

Inforiver provides 2 and 3-value bullet charts and a clustered bar for visualizing performance.

### a) 2-value bullet

In this example, I have 2022 Actuals and Plan across regions and categories. Select the 2 measures and click on the 'bullet' icon and select the 'Integrated variance bar' as highlighted.

<figure><img src="../../.gitbook/assets/2.5.4 2 value bullet.png" alt=""><figcaption><p>Bullet chart variants</p></figcaption></figure>

&#x20;The bullet chart gets inserted as shown. The variance between actuals and plan is shown in red/green.

<figure><img src="../../.gitbook/assets/2.5.5 2 value bullet.png" alt=""><figcaption><p>Bullet chart customization options</p></figcaption></figure>

### b) 3-value bullet

To enable the 3-value bullets, add one more measure as shown below. We'll choose the 'Bullet with marker' as highlighted.

<figure><img src="../../.gitbook/assets/2.5.6 3 value bullet.png" alt=""><figcaption><p>3-value bullet variants</p></figcaption></figure>

This type of bullet chart also displays the comparison band. The legend is highlighted below. These options can be customized from the toolbar.

<figure><img src="../../.gitbook/assets/2.5.7 3 value bullet.png" alt=""><figcaption><p>Bullet with marker</p></figcaption></figure>

### c) Clustered bar

The clustered bar is applicable only when using one of these 4 bullet variants - Stephen Few's Qualitative bullet, Qualitative bullet with marker, Comparative bullet, and Bullet with marker.

Click on 'Series display' in the 'Customize' tab. Change the '**Additional target**' to '**Bar**' instead of 'Line'.

In the popup screen, enable 'Clustered bar'.

<figure><img src="../../.gitbook/assets/2.5.8 clustered bar.png" alt=""><figcaption><p>Enabling clustered bar</p></figcaption></figure>

The clustered bar gets applied.

<figure><img src="../../.gitbook/assets/2.5.9 clustered bar.png" alt=""><figcaption><p>Clustered bar</p></figcaption></figure>

## 3. Distribution

### a) Stacked charts

In this example, we have 2022 actuals across regions. Let us use a stacked chart to see the composition based on subcategories for the regions.

Select all the subcategory columns and click on the 'Bullet' icon. We have 2 options - A stacked bar and a percentage stacked bar.&#x20;

<figure><img src="../../.gitbook/assets/2.5.13 stacked chart.png" alt=""><figcaption><p>Stacked chart options</p></figcaption></figure>

Let's select the percentage stacked bar. The chart gets added.&#x20;

<figure><img src="../../.gitbook/assets/2.5.14 stacked chart.png" alt=""><figcaption><p>Percentage stacked bar</p></figcaption></figure>

Let's hide the subcategory columns. In the toolbar, click on the 'Manage columns' toolbar. Uncheck the highlighted measure - 2022 Actuals.

<figure><img src="../../.gitbook/assets/2.5.15 stacked chart.png" alt=""><figcaption><p>Hide subcategory columns</p></figcaption></figure>

Select the column with the chart and drag using the arrow next to the column header to resize. There are a number of customization options available, which will be covered in a later section.

<figure><img src="../../.gitbook/assets/2.5.16 stacked chart.png" alt=""><figcaption><p>Resize the chart</p></figcaption></figure>

### b) Waterfall charts

Let us visualize the contribution of the subcategories to the total margin.

Select the 'Margin' column and click on the 'Waterfall' icon. There are 3 options - we'll choose the colored waterfall.

<figure><img src="../../.gitbook/assets/2.5.17 waterfall chart.png" alt=""><figcaption><p>Waterfall chart options</p></figcaption></figure>

You can see that the highest positive and negative contributions are from Lamps and Refrigerators respectively.

<figure><img src="../../.gitbook/assets/2.5.18 waterfall chart.png" alt=""><figcaption><p>Waterfall chart to visualize margin contribution</p></figcaption></figure>

### c) Progress bar

To visualize the contribution of each category and subcategory to the total sales using the progress bar, click on the 'Quick formula' dropdown in the 'Insert' tab.

<figure><img src="../../.gitbook/assets/2.5.22 progress bar.png" alt=""><figcaption><p>Inserting contribution %</p></figcaption></figure>

Select the '% Contribution to Grand Total' option. In the side panel, check 'Enable bar chart' and click 'Create'.

<figure><img src="../../.gitbook/assets/2.5.23 progress bar.png" alt=""><figcaption><p>Enabling bar chart</p></figcaption></figure>

The progress bar gets added. You also have options to customize the display. You can choose to display only the percentage, value, or both. The bar color can also be changed.

<figure><img src="../../.gitbook/assets/2.5.24 progress bar.png" alt=""><figcaption><p>Progress bar</p></figcaption></figure>

## 4. Magnitude



## 5. Changes/deviation

In this example, let's visualize the pay gap between men and women in UK and US.

Select the two measures - average salary of men and women. Click on the 'Bullet' icon and select the 'Dot plot' icon highlighted.&#x20;

<figure><img src="../../.gitbook/assets/2.5.19 dot plot.png" alt=""><figcaption><p>Chart options for visualizing changes/deviation</p></figcaption></figure>

The dot plot gets inserted.&#x20;

<figure><img src="../../.gitbook/assets/2.5.20 dot plot.png" alt=""><figcaption><p>Dot plot</p></figcaption></figure>

Let's hide the salary columns and resize the dot plot.&#x20;

You can insert an axis for easy comprehension. In the 'Customize' tab, click on the 'Show axis' option.

<figure><img src="../../.gitbook/assets/2.5.21 dot plot.png" alt=""><figcaption><p>Show axis</p></figcaption></figure>

## 6. Comparison



## 7. KPI cards



## 8. Blend columns/KPIs

Let's blend the Sales and Margin% columns in a single column.&#x20;

In the 'Insert' tab, click on the 'Blend' option in the 'Column' section. A blank measure gets inserted and the 'Blend measure' side panel opens.&#x20;

Enter the title and select the measures as shown from the dropdown. Click 'Create'.

<figure><img src="../../.gitbook/assets/2.5.10 blend kpi.png" alt=""><figcaption><p>Blend measures side panel</p></figcaption></figure>

The columns are blended to create a single column. Note that Margin % is displayed below Sales. This is because we have used the default 'Vertical' as 'Blend direction'.

<figure><img src="../../.gitbook/assets/2.5.11 blend kpi.png" alt=""><figcaption><p>Blend measures vertically</p></figcaption></figure>

If you want to display in a horizontal orientation, change the 'Blend direction' to 'Horizontal'.

<figure><img src="../../.gitbook/assets/2.5.12 blend kpi.png" alt=""><figcaption><p>Blend measures horizontally</p></figcaption></figure>
