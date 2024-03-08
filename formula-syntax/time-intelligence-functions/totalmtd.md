# TOTALMTD

The TOTALMTD function evaluates the month-to-date value of the measure in the current context. It should be used in conjunction with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
TOTALMTD([measure])
// Returns the month-to-date value of the measure for every month
```

## Arguments

measure – The measure for which data has to be fetched and aggregated. Required.

## Return Value

Range of data. When used with an aggregation function, it returns a scalar value running-calculated to date, according to the period selected.

## Example

Find below an example in which the quantity is cumulatively summed every month-to-date.

<figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption><p>TOTALMTD</p></figcaption></figure>
