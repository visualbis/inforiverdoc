# HAS\_SOME

The HAS\_SOME identifier checks if one or more of the specified values are part of the list. It can be used with formula columns, and data input columns (select, multi-select) and returns TRUE or FALSE.

## Syntax

```javascript
has_some(column1, [column2],..., searchvalue1, [searchvalue2],...)
```

## Arguments

column1, column2 - The list of columns where the search needs to be performed. The argument column1 is required and other columns are optional.

searchvalue1, searchvalue2 - The list of values of to search in the columns. The argument searchvalue1 is required and other searchvalues are optional.

## **Example**

Let us consider the below scenario.&#x20;

The 'Project status' column is created using the data input column of type single select and status is defined for each product. Based on the status, funds are allocated and the expected project completion time is defined.&#x20;

The 'Fund allocation' column is a data input - number column, which uses the HAS\_SOME identifier to search for status and assign funds based on project status.&#x20;

<figure><img src="../../.gitbook/assets/Formula has some 1.png" alt=""><figcaption><p>Using the HAS_SOME identifier</p></figcaption></figure>

Another formula column is created using HAS\_SOME to display the project completion time.

<figure><img src="../../.gitbook/assets/Formula has some.png" alt=""><figcaption><p>Using the HAS_SOME identifier</p></figcaption></figure>
