# Advanced Settings

### 1. Writeback column validation

In the advanced settings tab, you can enforce constraints on the data being written back. You can either use a formula to evaluate the data or use a null check.

#### 1.1. Cannot be empty

Only the cells that are not null for the specified field will be written back to the destination.

<figure><img src="../../../.gitbook/assets/image (901).png" alt=""><figcaption><p>Cannot be empty option</p></figcaption></figure>

**1.2. Enter formula**

You can specify a formula that should evaluate to true for the cells to be written back. The cells that do not satisfy the validation rule will be excluded during writeback.&#x20;

In the sample report, for the Cumulative Revenue measure, notice how only the data cells with values greater than 500 million were written back.&#x20;

<figure><img src="../../../.gitbook/assets/image (902).png" alt=""><figcaption><p>Cumulative revenue &#x3C; 500m not written back</p></figcaption></figure>

With this option, you can also apply cross-filters. Let's use the same validation rule, but this time in the Sum of COGS measure. The COGS cells that don't meet the cumulative revenue condition will not be written back.

<figure><img src="../../../.gitbook/assets/image (903).png" alt=""><figcaption><p>COGS cells are excluded from writeback when Cumulative Revenue &#x3C; 500m</p></figcaption></figure>

Whenever a writeback is triggered, Inforiver will display a preview of the excluded cells.

<figure><img src="../../../.gitbook/assets/image (904).png" alt=""><figcaption><p>Preview of excluded data</p></figcaption></figure>

**1.3. Prevent writeback when validation fails**

Turn on the **Prevent writeback when validation fails** toggle to stop writeback when empty fields are detected.&#x20;

An exception notification is generated during writeback that gives details of empty measures/columns or rows that do not meet the validation condition.&#x20;

<figure><img src="../../../.gitbook/assets/image (18) (1) (1) (1).png" alt=""><figcaption><p>Empty fields error</p></figcaption></figure>

### 2. Writeback column rename

You need not use the column names from the dataset while writing back, you can specify a custom column name. For instance, if the column name in the data set is PY, you can rename it to PreviousYear for writeback. To rename columns, navigate to Writeback settings > Advanced tab > Writeback column rename and click the <img src="../../../.gitbook/assets/image (905).png" alt="" data-size="line">icon.

In the example, we have renamed <mark style="color:green;">Segment</mark> to <mark style="color:orange;">Category</mark> and <mark style="color:green;">Product</mark> to <mark style="color:orange;">Brand</mark>. <mark style="color:green;">COGS</mark> has been expanded to <mark style="color:orange;">Cost of goods sold</mark>.

<figure><img src="../../../.gitbook/assets/image (906).png" alt=""><figcaption><p>Renaming WB fields</p></figcaption></figure>
