# CURRENT\_PERIOD

The CURRENT\_PERIOD identifier dynamically refers to each period in the report. It can be used with date-based functions like SHIFT or MOVING\_AVERAGE.

### Example <a href="#example" id="example"></a>

1. The AGGREGATE function has been used with the CURRENT\_PERIOD identifier to find the minimum sales 3 months prior to each month in the report.

<figure><img src="../../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption><p>AGGREGATE with CURRENT_PERIOD</p></figcaption></figure>

2. We've used SHIFT function with the CURRENT\_PERIOD identifier to shift each month by 2 months. For example, for January, the SHIFT function returns March 01st.

<figure><img src="../../.gitbook/assets/image (1373).png" alt=""><figcaption><p>SHIFT function with CURRENT_PERIOD</p></figcaption></figure>

3. We've used MOVINGSUM with the CURRENT\_PERIOD identifier to calculate the rolling sum of the profit for each month and 2 months after that month. For example, the MOVINGSUM for January would be the sum of the profits for January, February, and March.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1).png" alt=""><figcaption><p>MOVINGSUM with CURRENT_PERIOD</p></figcaption></figure>
