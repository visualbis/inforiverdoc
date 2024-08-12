# Forecast

Inforiver can automatically close forecasts. This simplifies forecast management when multiple reports with multiple forecast measures are involved. The auto-close can be set up at the report level or workspace level.&#x20;

The Inforiver admin console has a forecast tab where admins can specify when to close forecast measures for that tenant. &#x20;

* The **calendar day** option allows you to specify a designated day of the month when the forecasts will be automatically closed. In the screenshot, we've used the 5th as the calendar day - forecasts will be closed on the 5th of every month, irrespective of holidays/weekdays/weekends.

<figure><img src="../../.gitbook/assets/image (1) (17).png" alt=""><figcaption><p>Calendar day option</p></figcaption></figure>

* The **workday option** considers holidays and weekends and closes the forecasts accordingly i.e. the number of working days excluding holidays and weekends. When you select this option, an additional _Holiday Calendar_ option is enabled. You can choose the holiday list from pre-defined holiday calendars. In the screenshot, we have configured forecasts to be auto-closed on the 15th day of every month, excluding holidays from the selected calendar(s).

<figure><img src="../../.gitbook/assets/image (2) (17).png" alt=""><figcaption><p>Auto close forecasts on selected workday</p></figcaption></figure>

The settings specified in the Inforiver admin console are reflected in the manage forecast settings of the visual. You can override the auto-close settings specified in the admin console at visual-level.

<figure><img src="../../.gitbook/assets/image (3) (16).png" alt=""><figcaption><p>Auto-close at workspace level</p></figcaption></figure>
