# DATEADD

The DATEADD function adds a specified number of days to the input date. The input date should be in MM/DD/YYYY format. Node references are also accepted as arguments. Use [DATE.SET()](date.set.md) to set the format of the output date.

## Syntax

```javascript
dateadd(date, value)
```

## Arguments

date – The date which is passed as input to the function.

value – The number of days to be added to the input date. Can be positive or negative.

## Return value

Date

## Example

```javascript
DATEADD('8/2/2023',5)
```

Returns 7/8/2023.

<figure><img src="../../.gitbook/assets/image (168).png" alt=""><figcaption></figcaption></figure>
