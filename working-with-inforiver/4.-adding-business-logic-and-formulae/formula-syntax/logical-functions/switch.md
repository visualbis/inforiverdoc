# SWITCH

Evaluates an expression against a list of values and returns the result corresponding to the first matching value. If there is no match, an optional default value is returned.

## Syntax

```javascript
SWITCH( expression, value1, result1, value2, result2, ... value_n, result_n [ default] )
```

## Arguments

expression – The statement to be evaluated.

value1, value2, … value\_n – The list of values to be compared against the expression.

result1, result2, … result\_n – The result to be returned if the expression matches with the corresponding value in the argument list.

default – The default value to be returned if the expression does not match with any of the values in the argument list. This is an optional argument.

## **Return Value**

result when the expression matches with value, default in case there was no match.

## **Example**

```javascript
SWITCH(Region, "West", 25, "East",30, 50)
```

Will return 25, if the region is West and 30 is region is East and 50 for all other regions.

## **Excel Equivalent**

[https://support.microsoft.com/en-us/office/switch-function-47ab33c0-28ce-4530-8a45-d532ec4aa25e](https://support.microsoft.com/en-us/office/switch-function-47ab33c0-28ce-4530-8a45-d532ec4aa25e)
