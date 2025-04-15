# SHIFT

The SHIFT formula returns the date after shifting a date either backwards or forwards by a specified time period, like a month, quarter, or year.

## Syntax

```javascript
MOVINGSUM(inputDate, <offset interval>)
```

## Arguments

inputDate– The date to be shifted. Required.

offset interval - The preset format model, like month("M"), quarter("Q) or year("Y"). Required.

## Return value

Returns a date after shifting the input date by the specified number of months, quarters, etc.

## Example

```javascript
CURRENT_PERIOD, SHIFT(CURRENT_PERIOD, "2M")
//Shifts the date by 2 months
```

We've used SHIFT to shift each month by 2 months. For example, for January, the SHIFT function returns March 01st.

<figure><img src="../../.gitbook/assets/image (1373).png" alt=""><figcaption><p>SHIFT function</p></figcaption></figure>

You can also use SHIFT with forecast open and closed periods. In this example, we've shifted the forecast open period end date backwards by 2 quarters.

<figure><img src="../../.gitbook/assets/image (1374).png" alt=""><figcaption><p>SHIFT for forecast open and closed periods</p></figcaption></figure>
