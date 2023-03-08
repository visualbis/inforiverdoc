# SWITCH

The SWITCH function evaluates an expression against a list of values and returns the result corresponding to the first matching value. If there is no match, an optional default value is returned.

## Syntax

```javascript
switch( expression, val1, res1, val2, res2, ... val_n, res_n, default )
```

## Arguments

exp – The statement to be evaluated

val1, val2, … val\_n – The list of values to be compared against the expression

res1, res2, … res\_n – The result to be returned in case of a match

default – The default value to be returned if the expression does not match with any of the values in the argument list. This is an optional argument.

## **Return value**

Result when the expression matches with value, default in case there was no match.

## **Example**

```javascript
SWITCH(Region, "West", 25, "East",30, 50)
```

Will return 25 if the region is West, 30 if the region is East and 50 for all the other regions

## **Excel equivalent**

[SWITCH](https://support.microsoft.com/en-us/office/switch-function-47ab33c0-28ce-4530-8a45-d532ec4aa25e)
