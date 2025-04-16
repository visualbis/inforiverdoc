# MOVINGSUM

The MOVINGSUM formula returns the sum of a measure over a specified date range.&#x20;

## Syntax

```javascript
MOVINGSUM(measure, startDate, endDate)
```

## Arguments

measure– The measure to sum. Required.

startDate – Start date of the range. Required.

endDate- End date of the range. Required.

## Return value

Returns the sum of the measure over the specified date range.

## Example

```javascript
MOVINGSUM([Profit], CURRENT_PERIOD, SHIFT(CURRENT_PERIOD, "2M"))
//Calculates the sum of the profit for a particular month and 2 months after it

MOVINGSUM([Sales], DATE(2024,4,1), DATE(2024,8,31))
//Calculates the rolling sum between April and August 2024 
```

We've used MOVINGSUM to calculate the rolling sum of the profit measure for each month and 2 months after that month. For example, the MOVINGSUM for January would be the sum of the profits for January, February, and March.

<figure><img src="../../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption><p>MOVINGSUM example</p></figcaption></figure>

You can also use MOVINGSUM with forecasts to aggregate your measures over open and closed periods. In this example, we've aggregated the forecast measure for the open periods.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

