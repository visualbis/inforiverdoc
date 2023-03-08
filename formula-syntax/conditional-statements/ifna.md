# IFNA

The IFNA function returns the value you specify if a formula returns the #N/A error value; otherwise, it returns the result of the formula.

## Syntax

```javascript
ifna(value1,value2)
```

## Arguments

value1- The argument that is checked for the #N/A error value

value2- The value to return if the formula evaluates to the #N/A error value

## **Return value**

Either value1 or value2

## **Example**

```javascript
ifna((AC-PY)/PY, 0)
```

Returns AC-PY/PY if the value is a number else returns 0

## **Excel equivalent**

[IFNA](https://support.microsoft.com/en-us/office/ifna-function-6626c961-a569-42fc-a49d-79b4951fd461)
