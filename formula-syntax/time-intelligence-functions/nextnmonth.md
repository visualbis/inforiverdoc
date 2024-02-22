# NEXTNMONTH

The NEXTNMONTH function can be used to select data from a given measure, for a specified number of months after the current month. It should be used in conjunction with the SELECT clause and with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
NEXTNMONTH(number_of_months)
```

## Arguments

number\_of\_months – The number of months for which data has to be fetched. Required.

## Return value

Range of data.

## Example

```javascript
NEXTNMONTH(15) 
//Returns data for 15 months before the current month
```

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption><p>NEXTNMONTH</p></figcaption></figure>
