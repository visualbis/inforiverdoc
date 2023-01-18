# COUNTIF

Returns the count of item matches the condition, can be used to with BLANK as condition to count the blank values in a column/row

## Syntax

```javascript
Count(list, condition)
```

## Arguments

list - array of numbers or text

condition - string representing a condition

## Example

```javascript
COUNTIF([100,500,120],"<200")
```

Returns 2, since only two values in the given list matches the condition.

## Excel Equivalent

[COUNTIF](https://support.microsoft.com/en-us/office/countif-function-e0de10c6-f885-4e71-abb4-1f464816df34)
