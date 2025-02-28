# Add Column

You can create calculated measures, dimensions, and conditional columns right within Infobridge and cascade them to target reports. The source report will remain unchanged; you can enhance it with the required dimensions and measures created in Infobridge. Let's explore the different options to create measures, dimensions, and columns within a bridge.

<figure><img src="../../.gitbook/assets/image (1275).png" alt=""><figcaption><p>Add measure/dimension</p></figcaption></figure>

## 1. Add Measure

Write a custom calculation or leverage built-in Infobridge formulas to create a measure. The formula editor opens when you click the **Add Measure** option. Add references to dimensions and measures from the Reference tab. Access built-in functions from the Function tab.

<figure><img src="../../.gitbook/assets/image (1276).png" alt=""><figcaption><p>Adding a new calculated measure</p></figcaption></figure>

Notice how a custom measure has been added to the bridge:

<figure><img src="../../.gitbook/assets/image (1277).png" alt=""><figcaption><p>New measure added from Infobridge</p></figcaption></figure>

## 2. Add Dimension

You can add dimensions directly in a bridge by writing an expression based on specific conditions, or applying calculations. Enter the expression in the formula editor.

<figure><img src="../../.gitbook/assets/image (1278).png" alt=""><figcaption><p>Creating a dimension in Infobridge</p></figcaption></figure>

ingA custom dimension is created in the bridge:

<figure><img src="../../.gitbook/assets/image (1279).png" alt=""><figcaption><p>New dimension added from Infobridge</p></figcaption></figure>

## 3. Split Column

Split a dimension column into multiple dimensions based on a delimiter or position.&#x20;

<figure><img src="../../.gitbook/assets/image (1280).png" alt=""><figcaption><p>Split option in Infobridge</p></figcaption></figure>

In this example, the Benchmark dimension is a comma-separated field. We've used the delimiter option to split this field into 2 dimensions: Benchmark 1 and Benchmark 2.&#x20;

<figure><img src="../../.gitbook/assets/image (1282).png" alt=""><figcaption><p>Splitting dimensions in Infobridge</p></figcaption></figure>

## 4. Conditional Column

Conditional columns are computed columns where the value is determined based on specific conditions or rules applied to other columns. It helps categorize data based on predefined criteria.

For instance, you can calculate the debt-risk level based on the Debt-to-Equity Ratio.

<figure><img src="../../.gitbook/assets/image (1283).png" alt=""><figcaption><p>Sample conditional column</p></figcaption></figure>

Similarly, you can assign a tax rate or shipping rate based on the region.

<figure><img src="../../.gitbook/assets/image (1285).png" alt=""><figcaption><p>Sample conditional column for tax and shipping rates</p></figcaption></figure>

Infobridge provides a no-code, intuitive interface to quickly create conditional columns. Let's add a new dimension to categorize regional markets.

<figure><img src="../../.gitbook/assets/image (1287).png" alt=""><figcaption><p>Creating a conditional column in Infobridge</p></figcaption></figure>

We've created the "Global Market" dimension using the conditional column option.

<figure><img src="../../.gitbook/assets/image (1288).png" alt=""><figcaption><p>Dimension added in Infobridge using the conditional column option</p></figcaption></figure>

