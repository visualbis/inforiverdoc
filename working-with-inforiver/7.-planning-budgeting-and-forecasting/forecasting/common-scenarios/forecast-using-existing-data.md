# Forecast using Existing Data

Creating a forecast based on already existing data can be helpful in several scenarios like the following:

1. You can create a forecast based on the actual performance (from past periods).&#x20;
2. You can create a newer version of an already existing forecast, instead of updating forecast data directly. This can be helpful when you want to archive older forecast versions or if you want to run variance analysis between forecast versions.
3. You want to update the forecast submitted by someone else in the organization.

To demonstrate this in Power BI, consider the following example involving ACME Corp. The firm has already performed a forecast (v1) for 2023. They intend to create a newer baseline version (v2) of the forecast, and then make a few more adjustments on it.

The steps involved in creating a new forecast based on existing data are as follows:&#x20;

1. Create a baseline report that shows the existing forecast (Forecast V1).

<figure><img src="../../../../.gitbook/assets/2023 fc.png" alt=""><figcaption><p>Baseline Report (Forecast V1)</p></figcaption></figure>

2. Click on **Insert -> Data Input -> Number -> Copy from another series -> Forecast V1**, as shown below.

<figure><img src="../../../../.gitbook/assets/2023 fc v2.png" alt=""><figcaption><p>Insert Copy of Series 'Forecast V1'</p></figcaption></figure>

3. This creates a copy of the original series. Let us name this new forecast as _Forecast V2_. Click on **Create**.

<figure><img src="../../../../.gitbook/assets/2023 fc v2_1.png" alt=""><figcaption><p>Forecast V2</p></figcaption></figure>

4. You can start editing the individual cell values. For example, double-click the cell corresponding to _Jan Forecast V2_ for _APAC_ and then type '11m' in the formula bar that appears above the table.

<figure><img src="../../../../.gitbook/assets/2023 fc v2_2.png" alt=""><figcaption><p>Edit Values in Forecast V2</p></figcaption></figure>

5. Press Enter, and the cell value automatically gets updated. In addition, the value automatically rolls up to the top (_International_ and _All_ regions) and updates the total.

<figure><img src="../../../../.gitbook/assets/2023 fc v2_3.png" alt=""><figcaption><p>Updated Forecast Version </p></figcaption></figure>

You can continue to make further changes like this to arrive at your finalized forecast version. Retaining the older version of the forecast is helpful to run variance analysis and comparisons as needed. &#x20;

The newer version of the forecast can also be written back to a database destination of your choice.&#x20;

Now that we have seen how to forecast using the existing data, in the [next section](adding-forecasts-for-periods-unavailable-in-the-model.md) we'll learn to add forecasts for the periods that are not available in your data model.

&#x20;
