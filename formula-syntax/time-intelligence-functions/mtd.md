# MTD

The MTD function can be used to select data from a given measure, for the current month. If an offset parameter is provided, previous months will also be returned. It should be used in conjunction with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
MTD(measure, offset)
```

## Arguments

measure – The measure for which data has to be fetched. Required.

offset -  Number of preceding months for which data has to be fetched. Optional.

## Return value

Range of data.

## Example

```javascript
MTD([Sales])
//Returns data from the Sales measure for the current month
MTD([Sales,2)
//Returns data for the past 2 months and the current month
```

<figure><img src="../../.gitbook/assets/image (10) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>MTD with offset</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (11) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>MTD without offset</p></figcaption></figure>

