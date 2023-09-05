# EOMONTH

The EOMONTH function takes a date as input and returns the last day of the month, which is a specified number of months from the input date. Node references are also accepted as arguments. Use [DATE.SET()](date.set.md) to set the format of the output date.

## Syntax

```javascript
eomonth(date, value)
```

## Arguments

date – The date which is passed as input to the function.

value – The number of months to be added to the input date. Can be positive or negative.

## Return value

Date

## Example

```javascript
EOMONTH('8/15/2023', 3)
```

Returns 30/11/2023.

<figure><img src="../../.gitbook/assets/image (227).png" alt=""><figcaption><p>EOMONTH</p></figcaption></figure>
