# COLUMN.PARENT

COLUMN.PARENT refers to the column's immediate parent in a column hierarchy. Chaining is possible - COLUMN.PARENT.PARENT refers to the grandparent and so on.

### Example <a href="#example" id="example"></a>

We want to calculate the percentage sales contribution from January to the first quarter.

One way to calculate would be to select the 'Units Sold' column of _January_ and divide it by the 'Units Sold' column under _Qtr1._

Instead, we can use the reference 'COLUMN.PARENT' to refer to _Qtr1_ as it is the immediate parent of _January_. In the below image, you can see that for January in the _Canada_ region, % Contribution is calculated as 14.26/34.43 resulting in 41.40%.

<figure><img src="../../.gitbook/assets/image (725) (1).png" alt=""><figcaption><p>%contribution from January to Quarter1</p></figcaption></figure>

You can calculate the % sales contribution from January to the entire year using COLUMN.PARENT.PARENT.

<figure><img src="../../.gitbook/assets/image (726) (1).png" alt=""><figcaption><p>%contribution from January to the entire year</p></figcaption></figure>
