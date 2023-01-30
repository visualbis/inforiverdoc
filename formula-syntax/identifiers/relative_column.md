# RELATIVE\_COLUMN

The RELATIVE\_COLUMN identifier returns the value of the column relative to the current column.

## Syntax

```
[Row1].Relative_Column(-1)
```

## Arguments

\[Row1] - Reference to a row

The argument should be a negative number.

## Example

The company is planning to add one more size as Extra Large from January 2014. The expected sales for each month are going to be the same as the previous month's value for the Large size.&#x20;

Relative\_Column points to the previous month’s value. January value will be applied for February and so on. Since we do not have December 2013 sales, January 2014 will be blank.&#x20;

<figure><img src="../../.gitbook/assets/Formula relative row.png" alt=""><figcaption><p>Row relative column</p></figcaption></figure>

If you want to display a value instead of a blank, use IF and Group index as shown below.

<figure><img src="../../.gitbook/assets/Formula relative row na.png" alt=""><figcaption><p>Concatenating with IF and GROUP_INDEX </p></figcaption></figure>

Note that we have used this formula in a template row, so the Extra Large row gets inserted for each category as highlighted in yellow.
