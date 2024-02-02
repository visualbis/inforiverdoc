# Forecasting

With Inforiver, you can easily generate a rolling forecast and use methods like period range, an average of period range, etc. to initialize the forecast. You can leverage the integrated time intelligence and time extension features to create half-yearly forecasts or fiscal period forecasts.

## 1. Generating a forecast

To create a forecast, click on the Insert Forecast button in the Insert ribbon. The forecast dialog box has the options listed below

**1. Measure name:** By default, the forecast measure is named ‘Forecast’. This can be updated to a relevant column name.

**2. Forecast period:** The time frame for which the forecast is being generated. Inforiver's time intelligence sets the start date to the current month - you can update the range based on your requirements.

**3. Linked actuals measure:** The new forecast measure will be created for past or closed periods as well. The _Linked actuals measure_ option allows you to select the series to be used as the data source. If Sales is selected, then the forecast measure for 2022 and 2023 will be populated from Sales. If Revenue is selected, then the forecast measure for 2022 and 2023 will be populated from Revenue.&#x20;

<figure><img src="../../.gitbook/assets/2024-02-02_10h27_04.png" alt=""><figcaption><p>Create forecast dialog box</p></figcaption></figure>

## 2. Configuring the forecast

Inforiver allows you to create rolling forecasts and choose different methods to populate the forecast values. &#x20;

**1. Target period:** You can split the forecast period into shorter time frames or configure the forecast for the whole period. In this case, we have split the forecast period into 3 parts: January to March, April to June, and July to December.

<figure><img src="../../.gitbook/assets/2024-02-02_10h41_55.png" alt=""><figcaption><p>Rolling forecast</p></figcaption></figure>

You can also configure for the entire period at one shot as shown below.

<figure><img src="../../.gitbook/assets/2024-02-02_10h55_38.png" alt=""><figcaption><p>Configuration for entire period</p></figcaption></figure>

**2. Select source:** You can choose the measure that will be used as the data source for the forecast. To manually enter the forecast values, select the 'Blank' option.

<figure><img src="../../.gitbook/assets/2024-02-02_10h30_44.png" alt=""><figcaption><p>Forecast data source</p></figcaption></figure>

**3. Apply operation:** There are 3 different methods that you can use to generate a forecast:

* **Period range**: The values from a  specific period range will be used to initialize the forecast. In this case, we have used the sales from Q4 2023 (Copy period range) to populate the forecast for Q1 2024 (Target period). The duration of the period range should match the duration of the target period. E.g., if the target period is 6 months, then you must select a period range spanning 6 months.

<figure><img src="../../.gitbook/assets/2024-02-02_11h08_22.png" alt=""><figcaption><p>Period range</p></figcaption></figure>

* **Single period:** The values for a specific month will be used to initialize the forecast. In this case, we have used the revenue from December 2022 to populate the forecast for Apr to Jun 2024.

<figure><img src="../../.gitbook/assets/2024-02-02_11h13_05.png" alt=""><figcaption><p>Single period</p></figcaption></figure>

* **Average of period range**: The average of a custom time period will be used to initialize the forecast. In this case, we have used the average revenue from Jan 2022 to Dec 2023 to initialize the forecast.

<figure><img src="../../.gitbook/assets/2024-02-02_11h17_28.png" alt=""><figcaption><p>Average of period range</p></figcaption></figure>

**4. Copy period range:** The time frame for which to copy data from the source measure.

<div>

<figure><img src="../../.gitbook/assets/2024-02-02_11h22_11.png" alt=""><figcaption><p>Period range</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Period range (1).png" alt=""><figcaption><p>Single month</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/period range 2 (1).png" alt=""><figcaption><p>Custom time frame</p></figcaption></figure>

</div>

## 3. Analysing the forecast

Let's look at the forecast generated with the configurations in the earlier sections.

* **Closed period forecasts**

The forecast measure generated for previous or closed periods will be greyed out and cannot be edited. In section 1, we had assigned the Sales measure to populate the forecasts for past periods.

<figure><img src="../../.gitbook/assets/2024-02-02_11h35_56.png" alt=""><figcaption><p>Forecasts for closed periods</p></figcaption></figure>

* **Forecast using period range**&#x20;

We used the Sales measure from Oct to Dec 2023, to populate for forecast from Jan to Mar 2024. For clarity, in this image, we have displayed only Sales and Forecast measures.

<figure><img src="../../.gitbook/assets/2024-02-02_11h42_02.png" alt=""><figcaption><p>Period range</p></figcaption></figure>

* **Forecast using single period**

We used the revenue from December 2022 to create the forecast from April to June 2024. For clarity, in this image, we have displayed only Revenue and Forecast measures.

<figure><img src="../../.gitbook/assets/2024-02-02_11h53_58.png" alt=""><figcaption><p>Forecast using single period</p></figcaption></figure>

* **Forecast using average of period range**

We used the average revenue from Jan 2022 to Dec 2023 to create the forecast from July to December 2024.

<figure><img src="../../.gitbook/assets/2024-02-02_12h07_45.png" alt=""><figcaption><p>Average of period range</p></figcaption></figure>

## 4. Date rollover

Once the actual monthly data is available for a particular forecasted month, the report needs to reflect the actuals instead of the forecast. Consider the case below, wherein a forecast has been created from August to year-end.

<figure><img src="../../.gitbook/assets/image (136) (1).png" alt=""><figcaption></figcaption></figure>

To roll over the forecast start period from August to September, in the Insert ribbon, click on _Manage Measures_. In the 'Inserted Columns' side pane, select the forecast measure and click on the edit icon.

<figure><img src="../../.gitbook/assets/image (137) (1).png" alt=""><figcaption><p>Editing the forecast measure</p></figcaption></figure>

In the Data Input side pane, select September from the _Forecast Period_ dropdown and click on the Update button.

<figure><img src="../../.gitbook/assets/image (247).png" alt=""><figcaption></figcaption></figure>

Notice how the Sales and Revenue measures are now available for August and the forecast starts from September onwards.

<figure><img src="../../.gitbook/assets/image (139) (1).png" alt=""><figcaption></figcaption></figure>

## 5. Re-forecasting

After creating a forecast, you can easily re-forecast your data using Inforiver. To edit the forecast, click on _Manage Measures_ in the Insert ribbon. In the 'Inserted Columns' side pane,  click on the edit icon against the forecast measure.

<figure><img src="../../.gitbook/assets/image (250).png" alt=""><figcaption><p>Editing the forecast</p></figcaption></figure>

Click on the Update link against the _Open Forecast Values_ option.&#x20;

<figure><img src="../../.gitbook/assets/image (251).png" alt=""><figcaption><p>Update forecast</p></figcaption></figure>

The Update Forecast dialog box opens - you can smoothly re-forecast your data from here.

<figure><img src="../../.gitbook/assets/image (252).png" alt=""><figcaption><p>Re-forecast configuration</p></figcaption></figure>

## 6. Extending the forecast period

Consider that a forecast has been created from September to December 2023. If you need to extend the forecast to 2024, first, the time frame needs to be updated in _Forecast Settings_. Click on _Manage Measures_ in the Insert ribbon and navigate to the Settings tab. Click on the Manage link against _Forecast Settings._

<figure><img src="../../.gitbook/assets/image (253).png" alt=""><figcaption><p>Extending the forecast period</p></figcaption></figure>

After the forecast period has been extended, follow the steps outlined in the [Re-forecasting](forecasting.md#5.-re-forecasting) section to configure the forecast.

<figure><img src="../../.gitbook/assets/image (254).png" alt=""><figcaption></figcaption></figure>

## 7. Forecast customizations

Inforiver offers a variety of customizations that can be applied once the forecast is created.&#x20;

#### 1. Forecast grand total

If the column grand total is enabled, you can choose whether the grand total for the forecast measure should be derived from open periods, closed periods, or both. To customize the grand total for forecasts, click on the forecast column gripper and select the desired option from the _Total Display_ section.

<figure><img src="../../.gitbook/assets/image (241).png" alt=""><figcaption><p>Total Display</p></figcaption></figure>

**a) All Periods:** The grand total forecast will be the aggregate of the forecasts for open and closed periods.

<figure><img src="../../.gitbook/assets/image (242).png" alt=""><figcaption><p>All Periods</p></figcaption></figure>



**b) Open Periods:** The grand total forecast will be the aggregate of the forecasts for open periods only.

<figure><img src="../../.gitbook/assets/image (243).png" alt=""><figcaption><p>Open Periods</p></figcaption></figure>



**c) Closed Periods:** The grand total forecast will be the aggregate of the forecasts for closed periods only.

<figure><img src="../../.gitbook/assets/image (244).png" alt=""><figcaption><p>Closed Periods</p></figcaption></figure>

#### 2. Show or hide closed periods

You can choose whether to display the forecasts for closed periods. To mask the forecast for closed periods, click on any forecast that is generated for closed periods, click on the _Show/Hide_ icon, and choose _Hide closed periods._

<figure><img src="../../.gitbook/assets/image (245).png" alt=""><figcaption><p>Show/Hide forecasts</p></figcaption></figure>

The forecast for the closed period is hidden as shown in the image below.&#x20;

<figure><img src="../../.gitbook/assets/image (246).png" alt=""><figcaption><p>Hide forecast for closed period</p></figcaption></figure>

To un-hide the forecasts for closed periods, click on any measure belonging to the closed period, click on the _Show/Hide_ icon, and select _Show closed periods_.
