# RELATIVE

The RELATIVE identifier changes the absolute cell/column reference to a relative reference.

## Syntax

Cell reference

```javascript
Relative(CELL_REF)
```

Column reference

```
[Column1].Relative(-1)
```

## Arguments

CELL\_REF - Reference to a cell

\[Column1] - Reference to a column

The argument in case of column reference should be a negative number.

## Examples

{% hint style="warning" %}
Relative reference will not work correctly if columns are reordered. Column references from the original layout will be used. Also, it is applicable only when inserting visual measures and not columns.
{% endhint %}

### **Relative cell reference**

Consider ship mode cost for each month. To increase the cost of ship mode by the month's total, you can use the 'Relative' function and select the cell as shown in the below image.

<figure><img src="../../.gitbook/assets/Formula relative cell.png" alt=""><figcaption><p>Relative cell reference</p></figcaption></figure>

Total cost in April = 126.46k

Increased cost for Bookcases -> First Class = 1.06k +126.46k =127.53k

Note that even though we have used the reference to April's total in the formula, it applies the corresponding month's total for the calculation. That is, for Bookcases -> First Class -> January, the updated cost is 0.72k +97.67k, 97.67k being January's total.&#x20;

### Relative column reference

Consider an example where you want to calculate the variance between the current month's sales and the prior month's sales. The prior month's sales can be calculated using 'Relative' as shown below.

<figure><img src="../../.gitbook/assets/Formula relative column.png" alt=""><figcaption><p>Relative column reference</p></figcaption></figure>

This column can be used to calculate variance using the formula shown in the image. Note that IFNA has been used to assign 0 in case of calculation errors.

<figure><img src="../../.gitbook/assets/Formula relative column 2.png" alt=""><figcaption><p>Using calculated column in downstream calculations</p></figcaption></figure>
