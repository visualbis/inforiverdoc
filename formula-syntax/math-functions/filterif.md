# FILTERIF

Returns the list of items that match the given condition

## Syntax

```javascript
FilterIF([List], "Condition")
```

## Arguments

List – List of values&#x20;

Condition - String

## Example

```javascript
Average(FilterIF([Column1,Column2,Column3],">1000"))
```

Returns the average of values in Column1, Column2 and Column3 if they are greater than 1000.
