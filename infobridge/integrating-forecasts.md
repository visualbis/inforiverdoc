# Integrating forecasts

You can have historical and current data in one visual and may have configured your forecasts in a different Inforiver visual. Inforiver can detect and seamlessly integrate future periods from a bridge. Let's look at how to integrate forecasts with Infobridge.

To demonstrate this feature, we created a Forecast for 2025. [Learn more about forecasting with Inforiver](../working-with-inforiver/7.-planning-budgeting-and-forecasting/).

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Creating an Inforiver forecast</p></figcaption></figure>

The target visual contains historical/current sales for 2022, 2023, and 2024.  Let's look at how to import the 2025 forecast from the previous visual into this target report.

<figure><img src="../.gitbook/assets/image (1070).png" alt=""><figcaption><p>Target visual with current and historical data</p></figcaption></figure>

**STEP 1:** Create a bridge to access the forecast data from the visual. We have created a bridge titled FC2025.

<figure><img src="../.gitbook/assets/image (1068).png" alt=""><figcaption><p>Creating a bridge for the forecast</p></figcaption></figure>

**STEP 2:** Create an Infobridge integration to the FC2025 bridge to access the forecast.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Creating an Infobridge integration</p></figcaption></figure>

**STEP 3**: Use the Insert Measure option, to insert the forecast measure from the bridge into the target visual. Notice how Inforiver creates the time extension without any manual intervention.

<figure><img src="../.gitbook/assets/image (1071).png" alt=""><figcaption><p>Inserting the forecast measure from the bridge</p></figcaption></figure>

The 2025 forecast is imported into the target report:

<figure><img src="../.gitbook/assets/image (1072).png" alt=""><figcaption><p>Forecast inserted with seamless time extension</p></figcaption></figure>

{% hint style="info" %}
The forecast columns inserted for previous years will be blank. We’ve hidden them using the column gripper options.
{% endhint %}
