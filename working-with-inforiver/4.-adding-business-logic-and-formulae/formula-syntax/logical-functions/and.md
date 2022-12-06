# AND

An AND statement returns TRUE only if all the arguments are TRUE and returns FALSE if any of the arguments is FALSE.

## Syntax

```javascript
AND( logical_test1, [logical_test2], ... )
```

## Arguments

logical\_test1 – The first condition to be evaluated. This is a required argument.

logical\_test2,.. – The additional conditions to be evaluated. These are optional arguments.

## **Return Value**

Either True or False

## **Example**

```javascript
IF(AND(Region == "West", Category=="Urban"), 25, 30)
```

Will return 25 if the region is West and category is Urban otherwise returns 30

## **Excel Equivalent**

[AND](https://support.microsoft.com/en-us/office/and-function-5f19b2e8-e1df-4408-897a-ce285a19e9d9)
