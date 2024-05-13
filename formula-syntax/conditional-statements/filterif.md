# FILTERIF

The FILTERIF function can be used to filter an array of values based on a given condition. It returns an array, hence it has to be used in conjunction with an aggregate function like SUM or AVERAGE. It can be used to populate a [calculated row](../../working-with-inforiver/4.-adding-business-logic-and-formulae/insert-calculated-rows/).

## Syntax

```javascript
filterif( list, condition)
```

## Arguments

list – The input list of values on which the filter is to be applied

condition – The condition to be evaluated

## Return value

Returns an array.

## Example 1

```javascript
sum(filterif([United States].DESCENDANTS, ROW.LABEL = 'Soda'))
```

The formula above will use FILTERIF to filter all the rows under Region 'United States' with category = 'Soda'. It will then sum up all these values column-wise.

<figure><img src="../../.gitbook/assets/image (230).png" alt=""><figcaption><p>FILTERIF usage</p></figcaption></figure>

## Example 2

```javascript
average(filterif([Column1,Column2,Column3],">1000"))
```

Returns the average of values in Column1, Column2, and Column3 if they are greater than 1000
