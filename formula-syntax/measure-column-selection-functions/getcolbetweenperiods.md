# GETCOLBETWEENPERIODS

The GETCOLBETWEENPERIODS function can be used to select data from a given measure, for a specified period. It should be used with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
GETCOLBETWEENPERIODS(fromDate, toDate, measures)
```

## Arguments

fromDate– The starting period from when data is to be fetched. Required.

toDate– The end period till when data is to be fetched. Required.

measures - Specify the measures for which to fetch data. Leaf-level measures will be taken if measures are not explicitly specified. Optional.

## Return value

Range of data.

## Example

```javascript
GETCOLBETWEENPERIODS(DATE.ADDMONTH(-6), DATE.ADDMONTH(2), [[Profit]])
//Returns the profit measure for specified the date range 
```

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Getcolbetweenperiods</p></figcaption></figure>
