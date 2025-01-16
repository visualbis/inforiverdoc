# MONTHPERIOD

The MONTHPERIOD function can be used to select data from a given measure, for a particular month or a range of months. It should be used in conjunction with the SELECT clause and with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
MONTHPERIOD(year, from_month, to_month)
```

## Arguments

year – The year for which data has to be fetched. Required.

from\_month – The month for which data has to be fetched or the start month if a range is specified. Values can be between 1 and 12. Required.

to\_month - The end month when a range of data has to be fetched. Values can be between 1 and 12. Optional.

## Return value

Range of data.

## Example

```javascript
MONTHPERIOD(2023,1,4) 
//Returns data from January to April of 2023
MONTHPERIOD(2022,5)
//Returns data from May, 2023
```

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Monthperiod without offset</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Monthperiod with offset</p></figcaption></figure>
