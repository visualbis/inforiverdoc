# PERIOD\_RANGE

The PERIOD\_RANGE function returns an array of date ranges between two specified dates. It can be used with other functions like FILTER.

## Syntax

```javascript
PERIOD_RANGE(fromDate, toDate)
```

## Arguments

fromDate- The start of the date range. Required.

toDate- The end date of the range. Required.

## Return value

Array of dates

## Example

```javascript
PERIOD_RANGE(DATE(2023,1,1),DATE(2023, 12,31))
//Create a date range for 2023
```

The PERIOD\_RANGE function can be used with forecasts as well. In this application of the PERIOD\_RANGE function

* The PERIOD\_RANGE function is used to select the open forecast periods
* The FILTER function filters out the forecast values > 1000 for open periods
* The open forecasts greater than 1000 are then summed up

<figure><img src="../../.gitbook/assets/image (1377).png" alt=""><figcaption><p>PERIOD_RANGE function used with forecasts</p></figcaption></figure>
