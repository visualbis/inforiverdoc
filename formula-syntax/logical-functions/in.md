# IN

The IN function returns TRUE if the value being searched for is present in the input array.

## Syntax

```javascript
in(value,[item1,item2...])
```

## Arguments

value - The string which is being searched for

\[item1,item2...] - The input array to searched

## **Return value**

Either True or False

## **Example**

```javascript
if(in(Region, ["West","East"]),25, 30)
```

Returns 25 if the region is West or East otherwise returns 30
