# HAS\_ALL

The HAS\_ALL identifier checks if all the specified values are part of the list. It can be used with formula columns, and data input columns (select, multi-select) and returns TRUE or FALSE. the&#x20;

## Syntax

```javascript
has_all(column1, [column2],..., searchvalue1, [searchvalue2],...)
```

## Arguments

column1, column2 - The list of columns where the search needs to be performed. The argument column1 is required and other columns are optional.

searchvalue1, searchvalue2 - The list of values of to search in the columns. The argument searchvalue1 is required and other searchvalues are optional.

## **Example**

Let us consider below scenario.&#x20;

We are tracking the project status across four quarters and if there is at least one quarter where the status is 'In Review' and another quarter where the status is 'In Progress', then the overall status will be updated as 'On track'. Otherwise, it'll be updated to 'Not on track'.

<figure><img src="../../.gitbook/assets/Formula has all.png" alt=""><figcaption><p>Using the HAS_ALL identifier</p></figcaption></figure>
