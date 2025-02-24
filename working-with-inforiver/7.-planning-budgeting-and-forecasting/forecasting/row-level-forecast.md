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

**2.1. Target periods:** The forecast time frame is configured when you [create a forecast measure](../forecasting.md#id-1.-generating-a-forecast). You can configure the entire row forecast with a single time range or split the forecast period into multiple time frames. Use the **Add Range** link to create additional forecast ranges.

<div><figure><img src="../../../.gitbook/assets/2025-02-20_17h43_21.png" alt=""><figcaption><p>Forecast split across time ranges</p></figcaption></figure> <figure><img src="../../../.gitbook/assets/2025-02-21_10h12_34.png" alt=""><figcaption><p>Single configuration for the entire forecast period</p></figcaption></figure></div>

When you split the forecast time range, you must create time ranges spanning the entire forecasting period. For example, if your forecasting period is Jan 2025 - Dec 2025, you must cover this entire time period when you split it. Inforiver will display a red error icon and will not allow you to create the forecast until all the time ranges are configured.

<figure><img src="../../../.gitbook/assets/image (5).png" alt=""><figcaption><p>Splitting the forecast time frame</p></figcaption></figure>

**2.2. Set source:** You can opt for a blank forecast to manually enter values or refer to another row.

<figure><img src="../../../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption><p>Configure a blank forecast or use the values from another row</p></figcaption></figure>

**2.3. Source row:** When you choose the **By Row** option in the previous step, you need to select the row whose values will populate the forecast.

<figure><img src="../../../.gitbook/assets/image (2) (1) (1).png" alt=""><figcaption><p>Selecting the row category</p></figcaption></figure>

**2.4. Operation:** You can create forecasts using the following options:

* **Period range:** The forecast values will be copied from the range specified. In this case, we are sourcing the forecast for Jan 2025 to Mar 2025 from Oct 2024 to Dec 2024.

<div><figure><img src="../../../.gitbook/assets/image (3) (1).png" alt=""><figcaption><p>Period range config</p></figcaption></figure> <figure><img src="../../../.gitbook/assets/2025-02-21_10h16_28.png" alt=""><figcaption><p>Period range forecast</p></figcaption></figure></div>

* **Single period:** The values from the selected period are used to populate the forecast.

<div><figure><img src="../../../.gitbook/assets/image (1265).png" alt=""><figcaption><p>Single period config</p></figcaption></figure> <figure><img src="../../../.gitbook/assets/2025-02-21_10h35_12.png" alt=""><figcaption><p>Single period forecast</p></figcaption></figure></div>

* **Average of period range:** Use the average of the selected period range to populate the forecast.

<div><figure><img src="../../../.gitbook/assets/image (1267).png" alt=""><figcaption><p>Average of period range config</p></figcaption></figure> <figure><img src="../../../.gitbook/assets/2025-02-21_11h16_11.png" alt=""><figcaption><p>Average of period range forecast</p></figcaption></figure></div>
