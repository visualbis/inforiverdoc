# LASTNQTR

The LASTNQTR function can be used to select data from a given measure, for a specified number of quarters preceding the current quarter. It should be used in conjunction with the SELECT clause and with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
LASTNQTR(number_of_quarters)
```

## Arguments

number\_of\_quarters – The number of preceding quarters for which data has to be fetched. Required.

## Return value

Range of data.

## Example

```javascript
LASTNQTR(6) 
//Returns data for 6 quarters preceding the current one
```

<figure><img src="../../.gitbook/assets/image (8) (1).png" alt=""><figcaption></figcaption></figure>
