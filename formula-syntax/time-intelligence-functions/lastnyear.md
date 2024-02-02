# LASTNYEAR

The LASTNYEAR function can be used to select data from a given measure, for a specified number of years preceding the current year. It should be used in conjunction with the SELECT clause and with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
LASTNYEAR(number_of_quartersyears)
```

## Arguments

number\_of\_years – The number of preceding years for which data has to be fetched. Required.

## Return value

Range of data.

## Example

```javascript
LASTNYEAR(2) 
//Returns data for 2 years preceding the current one
```

<figure><img src="../../.gitbook/assets/image (9) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>
