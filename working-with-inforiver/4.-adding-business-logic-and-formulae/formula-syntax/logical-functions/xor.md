# XOR

Returns a logical 'Exclusive Or' of all arguments

## Syntax

```javascript
XOR ( logical_test1, [logical_test2], ... )
```

## Arguments

logical\_test1 – The first condition to be evaluated. This is a required argument.

logical\_test2,.. – The additional conditions to be evaluated. These are optional arguments.&#x20;

## **Return Value**

Either True or False

## **Example**

```javascript
IF(XOR(Region == "West", Category=="Urban"), 25, 30)
```

Will return 25 for all category in the West except for category Urban, and returns 25 for all Urban category under all region except for west, for all other items returns 30

## **Excel Equivalent**

XOR
