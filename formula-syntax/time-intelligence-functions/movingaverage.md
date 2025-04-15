# MOVINGAVERAGE

The MOVINGAVERAGE formula returns the average of a measure over a specified date range.&#x20;

## Syntax

```javascript
MOVINGAVERAGE(measure, startDate, endDate)
```

## Arguments

measure– The measure to sum. Required.

startDate – Start date of the range. Required.

endDate- End date of the range. Required.

## Return value

Returns the average of the measure over the specified date range.

## Example

```javascript
MOVINGAVERAGE([Profit], CURRENT_PERIOD, SHIFT(CURRENT_PERIOD, "2M"))
//Calculates the sum of the profit for a particular month and 2 months after it

MOVINGAVERAGE([Sales], DATE(2024,4,1), DATE(2024,8,31))
//Calculates the rolling average between April and August 2024 
```

We've used MOVINGAVERAGE to calculate the rolling average of the profit measure for each month and 2 months after that month. For example, the MOVINGAVERAGE for January would be the average of the profits for January, February, and March.

<figure><img src="../../.gitbook/assets/image (1371).png" alt=""><figcaption><p>MOVINGAVG</p></figcaption></figure>

You can also use MOVINGAVERAGE with forecasts to aggregate your measures over open and closed periods. In this example, we've aggregated the forecast measure for the open periods.

<figure><img src="../../.gitbook/assets/image (1370).png" alt=""><figcaption><p>MOVINGAVERAGE</p></figcaption></figure>
