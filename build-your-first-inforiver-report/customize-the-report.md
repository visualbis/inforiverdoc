# Customize the report

Unlike Excel or Power BI, Inforiver allows you to easily reorganize the items in your report, without the risk of overwriting the contents. First, let’s customize the order of the categories. Whenever you hover over a row, you’ll notice four horizontal lines appear to the far left.

This allows you to manually reorder a row. Simply click on it and drag it to drag the entire row. To do this in Power BI, you’d have to create a customer sort column for the exact sort order you want.

Next, let’s imagine we wanted to add a row with a custom formula. Click on the row for net revenue. Then, in the ribbon, go to Insert -> Row -> Insert Row Calculated Row. Alternatively, you can click on the 4 bars to the left of the selected row and select insert row.

For our calculated row we want to calculate gross profit margin. To set started, enter “Gross Margin %” into the title. We want to calculate the following: (**Net Revenue** – **Cost of Goods** **Sold**) / **Net Revenue**. When entering the formula, you can either click on the rows being referenced, or you can use the dot notation. So, for Net Revenue, the dot notation would be **\[Operating Profit].\[Gross Profit].\[Net Revenue]**.

Once you are done, your row configuration should look like this:

Finally, go to Home -> Number on the ribbon and format this row as a percentage.
