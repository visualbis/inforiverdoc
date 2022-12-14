# What-if analysis & simulations

Everyday business decision-making involves stakeholders asking a lot of ‘what-if’ questions. However, typical business intelligence and reporting tools fail to provide this very capability that decision-makers and analysts need most. As a result, users end up exporting report data to Excel to create their own models for offline analyses.

Inforiver provides two ways to model & simulate outcomes for your ‘what-if’ questions. Let us look at them one by one.

### 1. Edit a cell directly&#x20;

This method involves overwriting existing data in your report directly. However, Business Intelligence & Analytics tools typically do not provide this capability as there is no standard option to persist or write back the modified data.

With Inforiver, you receive the option to not only edit data directly – but also to write back to a database, or export the data to Excel/PDF files.

To simulate outcomes in Inforiver by editing data, you select a specific cell and start typing in a new value. Just as with Excel, a cell editor shows up just over the value.

<figure><img src="../../.gitbook/assets/4.7.5 Edit cell.png" alt=""><figcaption><p>Edit a cell directly</p></figcaption></figure>

Type in the new value and press enter to update the value and table totals automatically. There is also an _edit_ icon that appears next to the value indicating that the cell has been edited.

<figure><img src="../../.gitbook/assets/4.7.6 Edit cells (1).png" alt=""><figcaption><p>Cell edited successfully</p></figcaption></figure>

An alternate method to achieve the same outcome is to double-click a specific cell. This opens a formula bar at the top where you can make similar adjustments.

<figure><img src="../../.gitbook/assets/4.7.6 Edit cells (2).png" alt=""><figcaption><p>Editing using a formula bar</p></figcaption></figure>

Inforiver also allows you to use expressions with scaled values (e.g., 11250 + 0.5k) and percentages (e.g., 11250 + 10%). You can use this in both the in-cell editor and the formula bar.

You can update even cells/columns that display charts/graphs using the above method. After the update, the charts or graphs render again based on the updated value.

### 2. Use a simulation slider

Another method to create projections in Power BI is to use the intuitive _simulation_ capability offered by Inforiver. Compared to the previous method, this approach has the benefit of automatically tracking variances for each record.

To use this feature, select the 2022 Actuals field and click on the ‘Simulate’ icon in the menu. This creates a simulation output field based on the input field (_2022 Actuals_, in this case).

<figure><img src="../../.gitbook/assets/4.7.1 Simulation.png" alt=""><figcaption><p>What-if analysis and simulations</p></figcaption></figure>

The side panel provides the following options:

a) **Insert as** - Visual measure or column

b) **Simulation based on** - A measure based on which the simulation series is created

c) **Variance formatting style** - To define whether an increase is good or bad

d) **Show slider** - To enable/disable the slider. If the slider is disabled, simulation can still be performed by cell editing

e) **Value range** - By default, each cell can be simulated from -100% to +100% of its value

Once the field has been created, you can click on any cell in this new simulation-enabled field. This will display a small slider icon next to it. Hovering over this icon reveals a slider. Clicking and dragging the slider changes the value in the cell. It also shows a percentage change as you keep moving the slider to the right or to the left. The value & totals get updated once you release the slider.

<figure><img src="../../.gitbook/assets/4.7.2(2) Simulation.png" alt=""><figcaption><p>Simulation slider</p></figcaption></figure>

&#x20;In the example above, we have increased the value for the category Water in the region Pacific by 22%, which results in an overall sales increase of 1%.&#x20;

When a parent cell is simulated, the change is distributed to the child levels. Simulating Grand Total -> East by 15% increases Beverages and Water for East region by the same percentage.

<figure><img src="../../.gitbook/assets/4.7.3 Simulation.png" alt=""><figcaption><p>Simulating at a parent level</p></figcaption></figure>

Multiple cells can be simulated at once. Use Shift/Ctrl + click to select cells and use the slider on any one cell to simulate.

<figure><img src="../../.gitbook/assets/4.7.4 Simulation.png" alt=""><figcaption><p>Simulating multiple cells</p></figcaption></figure>

When the simulation slider is disabled, double-click on the cell and edit directly as shown below.&#x20;

{% hint style="info" %}
All the variances are in red because the negative variance formatting style has been applied.
{% endhint %}

<figure><img src="../../.gitbook/assets/4.7.7 Simulation.png" alt=""><figcaption><p>Simulation using cell editor and negative variance formatting style</p></figcaption></figure>

To learn more about simulations in Power BI, read this [blog](https://inforiver.com/blog/general/5-ways-to-run-dynamic-what-if-simulations-in-power-bi/). &#x20;
