# DIVIDE

The DIVIDE function returns the division of the two numbers.

## Syntax

```javascript
divide (Numerator, Denominator, Alternate)
```

## Arguments

Numerator, Denominator - The values to be divided. These are required arguments.

Alternate - An alternate value when the division returns an error. This is an optional argument. In case the denominator is null and there is no alternate, returns a !DIV/0 error.

## Example

```javascript
divide (COLUMN1, COLUMN2, 0)
```

Returns COLUMN1/COLUMN2 and if any error returns 0
