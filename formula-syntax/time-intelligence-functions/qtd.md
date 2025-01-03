# QTD

The QTD function can be used to select data from a given measure, for the current quarter. If an offset parameter is provided, previous quarters will also be returned. It should be used in conjunction with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
QTD(measure, offset)
```

## Arguments

measure – The measure for which data has to be fetched. Required.

offset -  Number of preceding quarters for which data has to be fetched. Optional.

## Return value

Range of data.

## Example

```javascript
QTD([Sales])
//Returns data from the Sales measure for the current quarter
QTD([Sales],5)
//Returns data for the past 5 quarters and the current quarter
```

<figure><img src="../../.gitbook/assets/image (12) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>QTD without offset</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (14) (1) (1) (1) (1).png" alt=""><figcaption><p>QTD with offset</p></figcaption></figure>
