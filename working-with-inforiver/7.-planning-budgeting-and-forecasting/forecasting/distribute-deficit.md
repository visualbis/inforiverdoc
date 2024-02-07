# Distribute deficit

After a forecast is defined, it is a common occurrence for the actual values to fall short of the forecasted values. The difference between the actuals and the forecast is termed the deficit. With Inforiver, you can distribute the deficit among open forecast periods.

To demonstrate this feature, we have created a forecast for Q1 2024 and allocated 300k - distributed equally among January, February, and March. The January forecast has been closed since actuals are available. The forecast for January is 100k but the actual sales are only 52.98 k. Let's see how to distribute this deficit with Inforiver.

#### 1. Select the forecast measure and click on the distribute deficit option

From the Measures Compared dropdowns, you can select the measures for which the deficit is being calculated. In this case, we have calculated the deficit between forecast and sales. The calculated deficit is 47, 018.27.&#x20;

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption><p>Distribute deficit window</p></figcaption></figure>

#### 2. Select the forecast measure and distribution range

If you have multiple forecast measures in your report, from the Distribute to dropdown, select the forecast to which the deficit should be distributed. Click on the calendar icon to choose the period for distribution.

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption><p>Setting the distribution time range</p></figcaption></figure>

#### 3. Set the distribution method

There are two methods for distribution, we'll look at an example for each of them.

<figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Distribution method</p></figcaption></figure>

&#x20;In this scenario, both Feb and March have the same forecast values, so equal distribution and distribution by weights would have the same outcome. The deficit of 47k has been distributed equally between the Feb and March forecasts and added to the existing forecasted value.

<figure><img src="../../../.gitbook/assets/image (3).png" alt=""><figcaption><p>Deficit distributed to Feb and Mar</p></figcaption></figure>

Let's consider a scenario where the forecasts for Feb and Mar have different values.

<figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Different forecast values</p></figcaption></figure>

a) Distribute equally:

<figure><img src="../../../.gitbook/assets/image (5).png" alt=""><figcaption><p>Distribute equally</p></figcaption></figure>

b) Distribute by weights:

<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption><p>Distribute by weights</p></figcaption></figure>
