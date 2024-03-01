# QTRPERIOD

The QTRPERIOD function can be used to select data from a given measure, for a particular quarter or a range of quarters. It should be used in conjunction with the SELECT clause and with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
QTRPERIOD(year, from_quarter, to_quarter)
```

## Arguments

year – The year for which data has to be fetched. Required.

from\_quarter – The quarter for which data has to be fetched or the start quarter if a range is specified. Values can be between 1 and 4. Required.

to\_quarter - The end quarter when a range of data has to be fetched. Values can be between 1 and 4. Optional.

## Return value

Range of data.

## Example

```javascript
QTRPERIOD(2023,1,3) 
//Returns data from the first to the third quarter of 2023
QTRPERIOD(2023,4)
//Returns data for the fourth quarter of 2023
```

<figure><img src="../../.gitbook/assets/image (54) (1).png" alt=""><figcaption><p>Quarter period without offset</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Quarter period with offset</p></figcaption></figure>
