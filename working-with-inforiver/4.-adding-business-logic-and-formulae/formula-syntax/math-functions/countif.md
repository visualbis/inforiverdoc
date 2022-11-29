# COUNTIF

Returns the count of item matches the condition, can be used to with BLANK as condition to count the blank values in a column/row

## Syntax

```javascript
Count(list, condition)
```

## Example

```javascript
COUNTIF([100,500,120],"<200")
```

Returns 2, since only two values in the given list matches the condition.
