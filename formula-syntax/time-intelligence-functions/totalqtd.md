# TOTALQTD

The TOTALQTD function evaluates the quarter-to-date value of the measure in the current context. It should be used in conjunction with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
TOTALQTD([measure])
// Returns the quarter-to-date value of the measure for every quarter
```

## Arguments

measure – The measure for which data has to be fetched and aggregated. Required.

## Return Value

Range of data. When used with an aggregation function, it returns a scalar value running-calculated to date, according to the period selected.

## Example

Find below an example in which the quantity is cumulatively summed every quarter-to-date.

<figure><img src="../../.gitbook/assets/image (10) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>TOTALQTD</p></figcaption></figure>
