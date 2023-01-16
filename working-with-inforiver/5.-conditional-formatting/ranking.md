# Ranking

One common use of conditional formatting is to highlight the top/bottom N ranked items in a report, which can help to quickly identify the most important or relevant items in the data.

Refer to [create rule](create-rule-basic-settings.md) to get started. Once the rule is created and you can see the 'Conditional formatting' side panel, follow the below steps.

Choose 'Ranking' in the 'Format by' dropdown. You can see the options shown in the below image. Using the 'Style' section, you can format text based on color/style, apply a background color or select icons.&#x20;

<figure><img src="../../.gitbook/assets/5.5.1 Ranking.png" alt=""><figcaption><p>Conditional formatting based on Top N ranking</p></figcaption></figure>

a) Let's apply icon-based formatting to the Top 3 subcategories based on Q4 2021 Actuals. Update the highlighted properties as shown below and click 'Apply'.

<figure><img src="../../.gitbook/assets/5.5.2 Ranking.png" alt=""><figcaption><p>Customizing the rule</p></figcaption></figure>

b) The top 3 categories based on Q4 2021 Actuals show an icon on the left as shown below.

<figure><img src="../../.gitbook/assets/5.5.3 Ranking.png" alt=""><figcaption><p>Conditional formatting applied based on Top N ranking </p></figcaption></figure>

c) You can also apply ranking based on percentages. In the below image, the bottom 50% of subcategories based on Q4 2021 Actuals are highlighted in red.

<figure><img src="../../.gitbook/assets/5.5.6 Ranking.png" alt=""><figcaption><p>Conditional formatting for bottom 50% of subcategories</p></figcaption></figure>

d) You can apply conditional formatting for the top and bottom items using the 'Both' option. In the below image, conditional formatting has been applied for the top and bottom subcategories.

<figure><img src="../../.gitbook/assets/5.5.5 Ranking.png" alt=""><figcaption><p>Conditional formatting for top and bottom subcategories</p></figcaption></figure>

e) Let's create one more rule for highlighting the top 2 subregions. Create a new rule and configure it as shown below. Click 'Apply'.

<figure><img src="../../.gitbook/assets/5.5.7 Ranking.png" alt=""><figcaption><p>Applying CF for subregions based on Ranking</p></figcaption></figure>

f) Conditional formatting doesn't get applied. This is because the subregion level is a total level but we have defined 'Row hierarchy levels' as 'Values only'.

<figure><img src="../../.gitbook/assets/5.5.8 Ranking.png" alt=""><figcaption><p>Conditional formatting for totals</p></figcaption></figure>

g) Change the 'Row hierarchy levels' to 'Values and totals' and click 'Apply'. You can see East and Pacific are highlighted.

<figure><img src="../../.gitbook/assets/5.5.9 Ranking.png" alt=""><figcaption><p>Multiple ranking rules </p></figcaption></figure>

In the next section, we'll be looking at [managing rules](manage-rules.md).
