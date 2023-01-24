# IN

The IN function returns TRUE if the list of values being searched is in the array.

## Syntax

```javascript
in(value,[item1,item2...]
```

## Arguments

value - The string which is being searched

item1,item2 - The values which are being searched in the array

## **Return value**

Either True or False

## **Example**

```javascript
if(in(Region, ["West","East"]),25, 30)
```

Returns 25 if the region is West or East otherwise returns 30
