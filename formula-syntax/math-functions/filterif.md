# FILTERIF

The FILTERIF function returns the list of items that match the given condition.

## Syntax

```javascript
filterif([List], Condition)
```

## Arguments

List - A list of values. This is a required argument.

Condition - The condition to be evaluated. This is a required argument.

## Example

```javascript
Average(FilterIF([Column1,Column2,Column3],">1000"))
```

Returns the average of values in Column1, Column2 and Column3 if they are greater than 1000
