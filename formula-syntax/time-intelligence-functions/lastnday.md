# LASTNDAY

The LASTNDAY function can be used to select data from a given measure, for a specified number of months preceding the current day. It should be used in conjunction with the SELECT clause and with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
LASTNDAY(number_of_days)
```

## Arguments

number\_of\_days – The number of preceding days for which data has to be fetched. Required.

## Return value

Range of data.

## Example

```javascript
LASTNDAY(45) 
//Returns data for 45 days preceding the current one
```

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1)  (14).png" alt=""><figcaption><p>LASTNDAY</p></figcaption></figure>
