# NEXTNYEAR

The NEXTNYEAR function can be used to select data from a given measure, for a specified number of years after the current year. It should be used in conjunction with the SELECT clause and an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
NEXTNYEAR (number_of_quartersyears)
```

## Arguments

number\_of\_years – The number of years for which data has to be fetched. Required.

## Return value

Range of data.

## Example

```javascript
NEXTNYEAR(2) 
//Returns data for 2 years after the current one
```

<figure><img src="../../.gitbook/assets/image (5) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>NEXTNYEAR</p></figcaption></figure>
