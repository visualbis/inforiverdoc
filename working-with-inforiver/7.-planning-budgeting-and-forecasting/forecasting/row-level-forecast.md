# Row level forecast

Create row-level forecasts to predict outcomes at a detailed level, such as based on the region or product line. After creating a regular forecast, you can create row-level forecasts by selecting a row and choosing the **Forecast Row** option from the Insert Row menu.

<figure><img src="../../../.gitbook/assets/image (1255).png" alt=""><figcaption><p>Forecast row option</p></figcaption></figure>

### 1. Generating a forecast

The options shown in the screenshot need to be configured to generate a row forecast.

<figure><img src="../../../.gitbook/assets/image (1256).png" alt=""><figcaption><p>Options for generating a row forecast</p></figcaption></figure>

**1.1. Row name:** The row category label that will hold forecasted values.

**1.2. Insert as:** Choose to insert a single forecast row or replicate the forecast row across all levels of the hierarchy with the Templated option.

{% hint style="info" %}
Select the Templated option when the row categories repeat across all levels of the hierarchy.
{% endhint %}

<div><figure><img src="../../../.gitbook/assets/image (1257).png" alt=""><figcaption><p>Single forecast row</p></figcaption></figure> <figure><img src="../../../.gitbook/assets/2025-02-20_16h17_40.png" alt=""><figcaption><p>Templated row forecast</p></figcaption></figure></div>

**1.4. Closed period:** The forecast row for earlier or closed periods can be populated by referencing the values from another row or by entering a formula.

<div><figure><img src="../../../.gitbook/assets/image (1258).png" alt=""><figcaption><p>Closed period forecast from linked row</p></figcaption></figure> <figure><img src="../../../.gitbook/assets/2025-02-20_16h26_22.png" alt=""><figcaption><p>Closed period forecast based on formula</p></figcaption></figure></div>

**1.5. Open period:** The forecasts for future or open periods can be populated in 3 ways

* **Linked row:** Refer to the values from another row.

<figure><img src="../../../.gitbook/assets/image (1259).png" alt=""><figcaption><p>Open forecasts based on linked row</p></figcaption></figure>

* **Formula**: Enter a formula to populate open forecasts.

<figure><img src="../../../.gitbook/assets/image (1260).png" alt=""><figcaption><p>Open forecasts based on a formula</p></figcaption></figure>

* **Data input:** Manually enter forecast values. When you choose the data input option, you can specify default values for the forecast. Opt for a static value, reference another row, or specify a formula.

<div><figure><img src="../../../.gitbook/assets/image (1261).png" alt=""><figcaption><p>Static default value</p></figcaption></figure> <figure><img src="../../../.gitbook/assets/2025-02-20_17h27_12.png" alt=""><figcaption><p>Default value based on another row</p></figcaption></figure> <figure><img src="../../../.gitbook/assets/2025-02-20_17h28_41.png" alt=""><figcaption><p>Default value based on a formula</p></figcaption></figure></div>
