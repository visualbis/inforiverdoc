# VALUEAT

The VALUEAT function returns the value of a measure for a specified date or a date shift relative to the current column.&#x20;

## Syntax

```javascript
VALUEAT([measure], <offset interval>)
```

## Arguments

measure – The measure for which data has to be fetched. Required.

offset interval - The preset format model, like month("M"), quarter("Q) or year("Y"). Required.

## Return value

The measure value at a specific point in time.

## Example

```
VALUEAT([Sales], "-1M")
//Returns the sales measure from the preceding month

VALUEAT([Sales], "1Q")
//Returns the sales measure from the next quarter
```

Let's look at a monthly sales report. The VALUEAT function can be applied to return the value of the sales measure for a particular month(s) preceding or after the current month. This is useful in evaluating the financial performance relative to other periods.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Fetching the measure value for the previous month</p></figcaption></figure>

Similarly, we can fetch the sales value for the next quarter as shown in this example.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Fetching the measure value for the next quarter</p></figcaption></figure>
