# SORT

The SORT function accepts a series of values and returns an array of the values sorted in ascending order.

## Syntax

```javascript
sort(value1,[value2]...)
```

## Arguments

value1,\[value2] – A series of numerical values to be sorted.

## Example

Consider that we are analyzing quarterly revenue. We need to determine the least but one revenue amount. In order to achieve this, we can use the sort function to sort the quarterly revenue for each row in ascending order. The sort function returns an array, we can access the elements using their index as shown in the image below.

<figure><img src="../../.gitbook/assets/image (164) (1).png" alt=""><figcaption><p>Application of SORT function</p></figcaption></figure>

In the example above, the variable 'a' holds the resulting array from the sort function. We can then access the least quarterly revenue element using the index a\[0] and the highest quarterly revenue using a\[3].

{% hint style="info" %}
To sort in descending order use the SORTDESC function.
{% endhint %}
