# CLOSEDPERIOD

When you need to perform an action specific to the closed or open periods in a forecast, you can use the .CLOSEDPERIOD in conjunction with \[Forecast] to refer to the closed periods. To refer to the open periods, use the NOT operator along with the CLOSEDPERIOD function.&#x20;

## Example

Let us say we want to add adjustment values to the open periods while marking 'closed' for the closed periods. To refer to the closed periods, we have used \[Forecast].CLOSEDPERIOD in the example below. To check and execute the action we have used the conditional statement, [IF](../conditional-statements/).

<figure><img src="../../.gitbook/assets/Forecast reference.png" alt=""><figcaption><p>.CLOSEDPERIOD</p></figcaption></figure>
