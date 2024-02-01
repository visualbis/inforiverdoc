# SETVISIBILITY

SETVISIBILITY can be used to show or hide rows, columns, and measures.

| NAME                                                                                  | DESCRIPTION                                          |
| ------------------------------------------------------------------------------------- | ---------------------------------------------------- |
| [SETVISIBILITY(ROW\_NAME)](setvisibility.md#id-1.-setvisibility-row\_name)            | Show or hide specific row categories                 |
| [SETVISIBILITY(COLUMNS)](setvisibility.md#id-2.-setvisibility-columns)                | Show or hide specific columns                        |
| [SETVISIBILITY(MEASURE\_NAME)](setvisibility.md#id-3.-setvisibility-measure)          | Show or hide specific measures                       |
| [SETVISIBILITY(ROW, COLUMN)](setvisibility.md#id-4.-setvisibility-row-column-measure) | Show or hide a measure for a particular row category |

### 1. SETVISIBILITY(ROW\_NAME)

Show or hide specific row categories - passing a value of TRUE will display the row, and passing a value of FALSE will hide it.

### Syntax

```javascript
SETVISIBILITY(ROW_NAME, BOOLEAN_ARG)
```

### Arguments

ROW\_NAME - Name of the row category to show or hide.

BOOLEAN\_ARG - Set to TRUE to enable the rule. Set to FALSE to disable the rule.

### Example

```
SETVISIBILITY([United States], FALSE) #Hides the United States row category and all child nodes under it
SETVISIBILITY([International], TRUE) #Displays the International row category
SETVISIBILITY([Technology], THIS) #Use with a toggle variable to show or hide the technology category
```

<figure><img src="../../.gitbook/assets/image (395).png" alt=""><figcaption><p>Show or hide rows using set visibility</p></figcaption></figure>

### 2. SETVISIBILITY(COLUMNS)

Show or hide specific columns - passing a value of TRUE will display the columns, and passing a value of FALSE will hide it.

### Syntax

```javascript
SETVISIBILITY(COLUMNS.COLUMN_NAME, BOOLEAN_ARG)
```

### Arguments

COLUMN\_NAME - The column to be shown or hidden.

BOOLEAN\_ARG - Set to TRUE to enable the rule. Set to FALSE to disable the rule.

### Example

```
SETVISIBILITY(COLUMNS.[2019 > Qtr 1 > Actuals, FALSE) #Hides the Actuals measure for 2019, qtr 1
SETVISIBILITY(COLUMNS.[2019 > Qtr 1 > March > Plan, TRUE) #Displays the Plan for 2019, Q1, March
SETVISIBILITY(COLUMNS.[2019 > Qtr 1 > March > Plan,THIS) #Use with a toggle variable to show or hide the Qtr1 Plan
```

<figure><img src="../../.gitbook/assets/image (394).png" alt=""><figcaption><p>Show or hide columns using set visibility</p></figcaption></figure>

### 3. SETVISIBILITY(MEASURE)

Show or hide a particular measure - passing a value of TRUE will display the columns, and passing a value of FALSE will hide it.

### Syntax

```javascript
SETVISIBILITY(MEASURE_NAME, BOOLEAN_ARG)
```

### Arguments

MEASURE\_NAME - Name of the measure to be hidden.

BOOLEAN\_ARG - Set to TRUE to enable the rule. Set to FALSE to disable the rule.

### Example

```
SETVISIBILITY([Plan], FALSE) #Hides the Plan measure
SETVISIBILITY([Actuals], TRUE) #Displays the Actuals measure
SETVISIBILITY([Actuals], THIS) #Use with a toggle variable to show or hide the Actuals measure
```

<figure><img src="../../.gitbook/assets/image (396).png" alt=""><figcaption><p>Display the Actuals measure using set visibility</p></figcaption></figure>

### 4. SETVISIBILITY(ROW, COLUMN)

Show or hide a measure for a particular row category and column. Passing a value of TRUE will display the row category for a particular column and measure. Passing a value of FALSE will hide it.

### Syntax

```javascript
SETVISIBILITY(ROW_NAME, COLUMNS.COLUMN_NAME, BOOLEAN_ARG)
```

### Arguments

ROW\_NAME - Name of the row category to show or hide.

COLUMN\_NAME - Name of the column to show or hide.

BOOLEAN\_ARG - Set to TRUE to enable the rule. Set to FALSE to disable the rule.

### Example

```
SETVISIBILITY([[Furniture], COLUMNS.[West > Sum of Profit]], FALSE) #Hides the column for a row category
SETVISIBILITY([[Furniture], COLUMNS.[Central > Sum of Quantity]], TRUE) #Shows the column for a row category
SETVISIBILITY([[Furniture], COLUMNS.[Central > Sum of Quantity]], THIS) #Use with a toggle variable to show or hide the Quantity for furniture
```

<figure><img src="../../.gitbook/assets/image (385).png" alt=""><figcaption><p>Setvisibility row and column</p></figcaption></figure>
