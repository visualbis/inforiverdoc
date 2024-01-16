# TOPN

Rank your data based on a category for a particular measure, for example, you can display the top-performing region, based on revenue.

## 1. SETTOPN

### Syntax

```javascript
SETTOPN(CATEGORY_NAME, COLUMNS.COLUMNS_NAME, VALUE, BOOLEAN_ARG)
```

### Arguments

CATEGORY\_NAME - The category group within which to select the top range.

COLUMN\_NAME - The measure used to select the top range.

VALUE - The number of top ranks to display.

BOOLEAN\_ARG - Set to TRUE to enable ranking. Set to FALSE to disable ranking.

### Example

```
SETTOPN([Sub-Category], COLUMNS.[Qtr4 > Sales], 2, TRUE) #Shows the 2 sub categories with top Q4 sales
SETTOPN([Sub-Category], COLUMNS.[Qtr4 > Sales], 20, FALSE) #Shows the sub categories with top 20 percentage Q4 sales
SETTOPN([Sub-Category], COLUMNS.[Qtr4 > Sales], THIS, TRUE) #Use with a slider or stepper variable to pass the value for the 'THIS' parameter
SETTOPN([Sub-Category], COLUMNS.[Qtr4 > Sales], 2, THIS) #Control the 'THIS' parameter using a toggle variable button
```

<figure><img src="../../.gitbook/assets/image (399).png" alt=""><figcaption><p>Top N</p></figcaption></figure>

## 2. SETBOTTOMN

### Syntax

```javascript
SETBOTTOMN(CATEGORY_NAME, COLUMNS.COLUMNS_NAME, VALUE, BOOLEAN_ARG)
```

### Arguments

CATEGORY\_NAME - The category group within which to select the bottom range.

COLUMN\_NAME - The measure used to select the bottom range.

VALUE - The number of bottom ranks to display.

BOOLEAN\_ARG - Set to TRUE to enable ranking. Set to FALSE to disable ranking.

### Example

```
SETBOTTOMN([Sub-Category], COLUMNS.[Qtr 1 > Profit], 3, TRUE) #Shows the 3 sub categories with the least Q1 profit
SETBOTTOMN([Sub-Category], COLUMNS.[Qtr4 > Sales], 20, FALSE) #Show the sub categories with the bottom 20 percentage of Q4 sales
```

<figure><img src="../../.gitbook/assets/image (398).png" alt=""><figcaption><p>Bottom N</p></figcaption></figure>

## 3. SETTOPBOTTOMN

### Syntax

```javascript
SETBOTTOMN(CATEGORY_NAME, COLUMNS.COLUMNS_NAME, VALUE, BOOLEAN_ARG)
```

### Arguments

CATEGORY\_NAME - The category group within which to select the top and bottom range.

COLUMN\_NAME - The measure used to select the top and bottom range.

VALUE - The number of top and bottom ranks to display.

BOOLEAN\_ARG - Set to TRUE to enable ranking. Set to FALSE to disable ranking.

### Example

```
SETTOPBOTTOMN([Sub-Category], COLUMNS.[Grand Total > Profit], 1, TRUE) #Shows the sub category with the most and least overall profit
SETTOPBOTTOMN([Sub-Category], COLUMNS.[Grand Total > Profit], 10, FALSE) #Show the sub categories with the top and bottom 10 percentage of overall profit
```
