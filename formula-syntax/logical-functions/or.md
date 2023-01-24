# OR

The OR function returns TRUE if **** at least one of the arguments is TRUE and returns FALSE when all the arguments evaluate to FALSE.

## Syntax

```javascript
or( logical_test1, [logical_test2], ... )
```

## Arguments

logical\_test1 – The first condition to be evaluated. This is a required argument.

logical\_test2,.. – The additional conditions to be evaluated. These are optional arguments.

## **Return value**

Either True or False

## **Example**

```javascript
if(or(Region == "West", Region =="East"), 25, 30)
```

Will return 25 if the region is West or East otherwise returns 30

## **Excel equivalent**

[OR](https://support.microsoft.com/en-us/office/or-function-7d17ad14-8700-4281-b308-00b131e22af0)
