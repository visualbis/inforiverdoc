# FILTER

The FILTER formula filters measure values across a period range and returns only those values that satisfy specified conditions. Combine the FILTER function with an aggregation function like SUM/AVG, etc.

## Syntax

```javascript
FILTER(measure, periodRange, condition1, condition2)
```

## Arguments

measure– The measure to filtered. Required.

periodRange – A period range array returned by the PERIOD\_RANGE function. Required.

condition1/condition2- A condition that must evaluate to TRUE or FALSE. Use the THIS keyword to refer to the current value. Required.

## Return value

Returns a range of measure values that satisfy the specified condition.

## Example

```javascript
FILTER([Sales], PERIOD_RANGE(DATE(2023,1,1),DATE(2023,12,31),THIS>1000)
//Returns the sales values in 2023 which are greater than 1000
```

In this sales report, we have used the FILTER function with SUM to aggregate only the cells that satisfy a certain condition. We are summing up the sales only when the sales is greater than 1000. The FILTER measure is blank for the "Fasteners" row as none of the cells have sales > 1000. Take a look at the "Envelopes" row. The sales for Q1 and Q4 satisfy the condition that sales should be > 1000; those two cells are returned by the FILTER function and summed up.

<figure><img src="../../.gitbook/assets/image (1375).png" alt=""><figcaption><p>FILTER</p></figcaption></figure>
