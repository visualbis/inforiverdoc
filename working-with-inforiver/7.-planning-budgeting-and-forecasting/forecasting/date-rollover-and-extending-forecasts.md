# Date rollover and extending forecasts

Once the actual data is available for a particular forecasted period, the report needs to reflect the actuals and the forecast should be closed. In the previous section, we created a forecast for 2024 based on the data from 2023 and 2022. In the image below, notice how January has an open forecast and data for Sales and Revenue (actuals), whereas the rest of 2024 only has the forecast measure.&#x20;

<figure><img src="../../../.gitbook/assets/image (414).png" alt=""><figcaption><p>Closing a forecast</p></figcaption></figure>

Let's see how we can close forecasts and roll over the date in Inforiver. To close a forecast period, click on the Close Period button in the Forecast ribbon. The Close Period dialog box has the following options:

#### 1. Select measure

You can create more than one forecast in Inforiver. From the dropdown, choose the forecast measure for which you want to close the period.

#### 2. Close period till

Based on when you receive the actual data for a forecasted period, you can choose up to when you would like to close forecasts. You have options such as the previous month/quarter/year and the current month/quarter/year. You can also set a custom month until which to close the forecast.

In this example, we received the data for January 2024 in February 2024 - so we can select the 'Previous Month' option to close the forecast till January. If we receive data at the end of a particular month, we can choose 'Current Month', E.g., if we received January data by the end of the month, we would choose current month.

<figure><img src="../../../.gitbook/assets/image (1) (1) (1) (1) (2) (1).png" alt=""><figcaption><p>Close period till option</p></figcaption></figure>

#### 3. Selected Period

This field displays the period to be closed - it will change based on the Close Period selection.&#x20;

<figure><img src="../../../.gitbook/assets/selected period.gif" alt=""><figcaption><p>Selected period</p></figcaption></figure>

#### 4. Extend forecast range

When you close a period, you can choose to extend the forecast. In this case, we generated a forecast from Jan to Dec 2024. When we close the January period, we can extend the forecast to 2025.

<figure><img src="../../../.gitbook/assets/image (2) (1) (1) (1) (2) (1).png" alt=""><figcaption><p>Extend forecast range option</p></figcaption></figure>

#### 5. Duration

If you select the _Extend Forecast Range_ checkbox_,_ the duration dropdown becomes active. In this case, you can choose to extend the forecast till January 2025 (1 month) or Q1 2025 (1 quarter).

<figure><img src="../../../.gitbook/assets/image (3) (1) (1) (1) (2).png" alt=""><figcaption><p>Duration by which to extned the forecast</p></figcaption></figure>

#### 6. Discard

If you do not wish to close the period, you can cancel by clicking on the discard button.

#### 7. Preview

Click on the preview button to open the confirmation dialog box. You can review the period that is being closed as well as the open forecast period.

<figure><img src="../../../.gitbook/assets/image (4) (1) (1) (1) (2).png" alt=""><figcaption><p>Preview forecast</p></figcaption></figure>

When you save, the selected forecast period is closed. Notice that the January forecast is greyed out and has been closed.

<figure><img src="../../../.gitbook/assets/image (5) (1) (1) (1).png" alt=""><figcaption><p>Forecast period closed</p></figcaption></figure>
