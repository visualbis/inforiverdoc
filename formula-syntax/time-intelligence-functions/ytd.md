# YTD

The YTD function can be used to select data from a given measure, for the current year. If an offset parameter is provided, previous years will also be returned. It should be used in conjunction with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
YTD(measure, offset)
```

## Arguments

measure – The measure for which data has to be fetched. Required.

offset -   Number of preceding years for which data has to be fetched. Optional.

## Return value

Range of data.

## Example

```javascript
YTD([Sales])
//Returns data from the Sales measure for the current year
YTD([Sales,2)
//Returns data for the past 2 years and for the current year
```

<figure><img src="../../.gitbook/assets/image (15) (1) (1).png" alt=""><figcaption><p>YTD with offset</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (16) (1) (1).png" alt=""><figcaption><p>YTD without offset</p></figcaption></figure>
