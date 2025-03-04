# Pivot column

## Pivot column

The Pivot Column option helps you restructure your data for better analysis and easier comparisons. Pivoting data essentially means converting row values from one column into multiple columns. To demonstrate pivoting data, let's take the region-wise sales for home appliances as an example.&#x20;

<figure><img src="../../.gitbook/assets/image (1289).png" alt=""><figcaption><p>Sample data</p></figcaption></figure>

We've pivoted the tabular data above based on the PRODUCT column. Notice how the product column has been converted into multiple columns - Microwave, Refrigerator, and Coffee Machines.

<figure><img src="../../.gitbook/assets/image (1290).png" alt=""><figcaption><p>Pivoted data based on the product field</p></figcaption></figure>

Let's see how we can pivot columns in Infobridge. The sample table contains country, product, and market data.  We'll pivot the "Product" dimension.

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption><p>Sample query to pivot data</p></figcaption></figure>

Select "Product" from the **Category** dropdown. We'll leave default options for the **Operations** and **Values** fields unchanged.

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption><p>Pivot column configuration</p></figcaption></figure>

Notice how each product is now a separate column.

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption><p>Pivoted column based on the product dimension</p></figcaption></figure>

We can choose different aggregation types like average, minimum, or maximum when we pivot a column as shown below

<figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption><p>Other aggregation types</p></figcaption></figure>

## Unpivot column

Unpivot does the opposite of pivot - it converts multiple column dimensions into a single row dimension. Let's consider the Product example - the sales for each product is captured in a separate column.

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Sales for each product is in a separate column</p></figcaption></figure>

Click on the **Unpivot** option from the Transform ribbon. Select the columns to be unpivoted into rows from the Column dropdown. We've selected all the product columns.

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption><p>Unpivot columns</p></figcaption></figure>

When you click Apply, each product column is converted into a single column titled "Attribute" that contains all the products as multiple rows. The sales for each product is also converted into a single column titled "Value" with multiple rows corresponding to each product.

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption><p>Unpivoted data for the product columns</p></figcaption></figure>

Finally let's use the **Rename Column** button to change the name of the default "Attribute" and "Value" columns to relevant, meaningful names.

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption><p>Rename unpivoted columns</p></figcaption></figure>
