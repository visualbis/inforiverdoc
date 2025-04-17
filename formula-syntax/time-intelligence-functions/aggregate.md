# AGGREGATE

The AGGREGATE formula performs a specific aggregation like min/max/avg/sum on a measure over a specified time range.

## Syntax

```javascript
MOVINGAVERAGE(measure, startDate, endDate, aggregationType)
```

## Arguments

measure– The measure to sum. Required.

startDate – Start date of the range. Required.

endDate- End date of the range. Required.

aggregationType - Aggregation method like AVG/SUM/MIN/MAX/MEDIAN. Required.

## Return value

Returns the custom aggregation applied on the measure over the specified date range.

## Example

```javascript
AGGREGATE([Profit], SHIFT(CURRENT_PERIOD, "-1M"), SHIFT(CURRENT_PERIOD, "-3M"), "MIN")
//Calculates the minimum of the profit in the past 3 months

AGGREGATE([Sales], DATE(2024,4,1), DATE(2024,8,31), "MEDIAN")
//Calculates the median of sales between April and August 2024
```

The AGGREGATE function has been used to find the minimum sales 3 months prior to each month in the report.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1).png" alt=""><figcaption><p>AGGREGATE</p></figcaption></figure>

