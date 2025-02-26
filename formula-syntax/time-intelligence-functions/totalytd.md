# TOTALYTD

The TOTALYTD function evaluates the year-to-date value of the measure in the current context. It should be used in conjunction with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
TOTALYTD([measure])
// Returns the year-to-date value of the measure for every year
```

## Arguments

measure – The measure for which data has to be fetched and aggregated. Required.

## Return Value

Range of data. When used with an aggregation function, it returns a scalar value running-calculated to date, according to the period selected.

## Example

Find below an example where the discount measure is calculated year-to-date.&#x20;

<figure><img src="../../.gitbook/assets/image (9) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>TOTALYTD</p></figcaption></figure>
