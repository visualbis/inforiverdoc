# NEXTNQTR

The NEXTNQTR function can be used to select data from a given measure, for a specified number of quarters after the current quarter. It should be used with the SELECT clause and an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
NEXTNQTR(number_of_quarters)
```

## Arguments

number\_of\_quarters – The number of quarters for which data has to be fetched. Required.

## Return value

Range of data.

## Example

```javascript
NEXTNQTR(6) 
//Returns data for 6 quarters after the current quarter
```

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>NEXTNQTR</p></figcaption></figure>
