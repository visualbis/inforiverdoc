# YEARPERIOD

The YEARPERIOD function can be used to select data from a given measure, for a particular year or a range of years. It should be used in conjunction with the SELECT clause and with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
YEARPERIOD(from_year, to_year)
```

## Arguments

from\_year – The year for which data has to be fetched or the start year if a range is specified. Required.

to\_year - The end year when a range of data has to be fetched. Optional.

## Return value

Range of data.

## Example

```javascript
YEARPERIOD(2020,2023) 
//Returns data from 2020 to 2023
YEARPERIOD(2023)
//Returns data from 2023
```

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption><p>Yearperiod without offset</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption><p>Yearperiod with offset</p></figcaption></figure>
