# AND

The AND function returns TRUE if all the conditions are TRUE and FALSE if any of the conditions are FALSE.

## Syntax

```javascript
and( logical_test1, [logical_test2], ... )
```

## Arguments

logical\_test1 – The first condition to be evaluated. This is a required argument.

logical\_test2,.. – The additional conditions to be evaluated. These are optional arguments.

## **Return value**

Either True or False

## **Example**

```javascript
if(and(Region == "West", Category=="Urban"), 25, 30)
```

Returns 25 if the region is West and the category is Urban, otherwise returns 30

## **Excel equivalent**

[AND](https://support.microsoft.com/en-us/office/and-function-5f19b2e8-e1df-4408-897a-ce285a19e9d9)
