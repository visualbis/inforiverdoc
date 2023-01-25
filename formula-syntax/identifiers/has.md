# HAS

The HAS identifier checks if the specified value is part of the list. It can be used with formula columns, and data input columns (select, multi-select) and returns TRUE or FALSE.

## Syntax

```javascript
has(column1, [column2],..., searchvalue)
```

## Arguments

column1, column2 - The list of columns where the search needs to be performed. The argument column1 is required and other columns are optional.

searchvalue - The value to be searched in the columns. This is a required argument.&#x20;

## **Example**

Let us consider the below scenario.&#x20;

We need to check if the [level](level.md) is a leaf level and increase sales by 50%. This has been achieved using the HAS identifier as shown in the below image.

<figure><img src="../../.gitbook/assets/Formula has.png" alt=""><figcaption><p>Using the HAS identifier</p></figcaption></figure>
