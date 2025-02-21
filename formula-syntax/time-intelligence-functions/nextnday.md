# NEXTNDAY

The NEXTNDAY function can be used to select data from a given measure, for a specified number of days after the current day. It should be used in conjunction with the SELECT clause and with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
NEXTNDAY(number_of_days)
```

## Arguments

number\_of\_days – The number of days for which data has to be fetched. Required.

## Return value

Range of data.

## Example

```javascript
NEXTNDAY(45) 
//Returns data for 45 days after the current day
```

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) ( (9).png" alt=""><figcaption><p>NEXTNDAY</p></figcaption></figure>
