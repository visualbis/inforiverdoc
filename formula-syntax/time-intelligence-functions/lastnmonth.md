# LASTNMONTH

The LASTNMONTH function can be used to select data from a given measure, for a specified number of months preceding the current month. It should be used in conjunction with the SELECT clause and with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
LASTNMONTH(number_of_months)
```

## Arguments

number\_of\_months – The number of preceding months for which data has to be fetched. Required.

## Return value

Range of data.

## Example

```javascript
LASTNMONTH(15) 
//Returns data for 15 months preceding the current one
```

<figure><img src="../../.gitbook/assets/image (7) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>LASTNMONTH</p></figcaption></figure>
