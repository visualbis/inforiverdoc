# ISNUMBER

The ISNUMBER function returns the logical value TRUE if the value argument is a valid number; otherwise, it returns FALSE.&#x20;

## Syntax

```javascript
isnumber(value)
```

## Arguments

value - cell or reference or expression

## **Return value**

Either True or False

## **Example**

```javascript
if(isnumber((AC-PY)/PY), (AC-PY)/PY, 0)
```

Returns AC-PY/PY if the value is a number else returns 0

## **Excel equivalent**

[ISNUMBER](https://support.microsoft.com/en-us/office/is-functions-0f2d7971-6019-40a0-a171-f2d869135665)
