# Autoclose forecasts

Inforiver can automatically close forecasts, provided that you are aware of when the actuals are expected to be received. You can specify the close day either from the Inforiver console or from the edit forecast settings.&#x20;

## 1. Inforiver console

To close the forecast measures in all the reports on a particular tenant, you can set up auto close from the [Inforiver console](../../../advanced-topics/admin-console/).  This feature is useful in scenarios where you have multiple reports and multiple forecast measures.

In the admin console, navigate to Settings > Forecast. In the Auto Close Forecast section, you can set the calendar day or work day on which all forecasts should be closed. Select the _Disabled_ option if you do not want to close forecasts automatically.&#x20;

### i) Calendar day

You can specify a particular day of the month when forecasts should be closed.

{% hint style="warning" %}
The forecasts will be closed irrespective of whether the designated day is a weekend or a holiday.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (10) (1) (2).png" alt=""><figcaption><p>Admin console auto close setup</p></figcaption></figure>

Open forecasts are closed automatically on the calendar day specified in the admin console. This setting can be viewed in the edit forecast settings as well.

<figure><img src="../../../.gitbook/assets/image (11) (1).png" alt=""><figcaption><p>Auto close settings</p></figcaption></figure>

### ii) Workday

The workday option excludes weekends and holidays and will close the forecast on the specified working day. You can select the holiday calendar(s) to refer to when the workday option is chosen.

<figure><img src="../../../.gitbook/assets/image (13) (1).png" alt=""><figcaption><p>Auto close using workdays</p></figcaption></figure>

This setting can be viewed in the edit forecast settings as well.

<figure><img src="../../../.gitbook/assets/image (14).png" alt=""><figcaption><p>Auto close for workday set at admin console</p></figcaption></figure>

## 2. Auto close settings at report level

You can specify a particular day on which to close forecasts, which is set at the report level. You can additionally set the [calendar ](autoclose-forecasts.md#i-calendar-day)or [workday ](autoclose-forecasts.md#ii-workday)options.

<figure><img src="../../../.gitbook/assets/image (15).png" alt=""><figcaption><p>Auto close from manage forecast </p></figcaption></figure>

When you auto-close forecasts, Inforiver can automatically extend the forecast period as well. Select the **Auto-extend period range by 1 month** checkbox to enable this feature.

<figure><img src="../../../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>
