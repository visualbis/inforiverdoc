# XOR

The XOR function returns a logical 'Exclusive Or' of all the arguments.

## Syntax

```javascript
xor ( logical_test1, [logical_test2], ... )
```

## Arguments

logical\_test1 – The first condition to be evaluated. This is a required argument.

logical\_test2,.. – The additional conditions to be evaluated. These are optional arguments.&#x20;

## **Return value**

Either True or False

## **Example**

```javascript
if(xor(Region == "West", Category=="Urban"), 25, 30)
```

Returns 25 for all categories in the West except for category Urban, and for all Urban categories except for region West, for all other items, returns 30

## **Excel equivalent**

[XOR](https://support.microsoft.com/en-us/office/xor-function-1548d4c2-5e47-4f77-9a92-0533bba14f37)
