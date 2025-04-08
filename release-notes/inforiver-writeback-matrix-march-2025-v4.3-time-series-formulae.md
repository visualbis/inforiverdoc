# Inforiver Writeback Matrix March 2025 - v4.3 - Time series formulae

In this release, explore the new range of time series formulas to gather business insights from your time-based data. We've also made Inforiver Writeback Matrix more secure with internal software version upgrades and API updates.

## New time series formulae

We've introduced a range of easy-to-use formulas for manipulating time series data. Whether you are tracking financial trends, analyzing sales performance, or identifying anomalies, these formulas enable you to filter and compare data efficiently.

<table><thead><tr><th width="178">FUNCTION NAME</th><th>DESCRIPTION</th></tr></thead><tbody><tr><td>VALUEAT</td><td>Returns the value of a measure for a specified date or a date shift relative to the current column</td></tr><tr><td>MOVINGSUM</td><td>Returns the sum of a measure over a specified date range</td></tr><tr><td>MOVINGAVERAGE</td><td>Returns the average of a measure over a specified date range</td></tr><tr><td>SHIFT</td><td>Shifts a date by a specified time period like a month, quarter or year</td></tr><tr><td>AGGREGATE</td><td>Performs a specific aggregation like min/max/avg/sum on a measure over a specified time range</td></tr><tr><td>PERIOD_RANGE</td><td>Returns a date range array between two specified dates</td></tr><tr><td>FILTER</td><td>Returns the measure values over a time range, only values satisfying the filter condition will be returned</td></tr></tbody></table>



Let's look at a monthly sales report. The VALUEAT function can be applied to return the value of the sales measure for a particular month(s) preceding or after the current month. This is useful in evaluating the financial performance relative to other periods. In this case, for February, the VALUEAT function returns the sales for January. Similarly, for March, the VALUEAT function returns the sales for February.

The SHIFT function returns the date after shifting the current month by a specified number of months. For January, the SHIFT function returns March 01st.&#x20;

{% hint style="info" %}
We have used months in these examples for demonstration purposes. Year and quarter are also supported in time series formulas.
{% endhint %}

<figure><img src="../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption><p>SHIFT and VALUEAT</p></figcaption></figure>

In the same sales report, we can use the FILTER function with an aggregation formula like MIN/MAX/SUM to aggregate only the cells that satisfy a certain condition. In this scenario, we are summing up the sales only when the sales is greater than 1000. The FILTER measure is blank for the "Fasteners" row as none of the cells have sales > 1000.

The AGGREGATE function has been used to find the minimum sales between 6 and 3 months before the current date.&#x20;

<figure><img src="../.gitbook/assets/image (1365).png" alt=""><figcaption><p>FILTER and AGGREGATE</p></figcaption></figure>

We've used the MOVINGSUM and MOVINGAVERAGE to calculate the rolling sum and average of the sales measure over a defined period of time - in this case, 2 months. For January, the moving sum is the sum of the sales across January, February, and March. A similar calculation is used for moving average as shown below.

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption><p>MOVINGSUM and MOVINGAVERAGE</p></figcaption></figure>

## Other enhancements and bug fixes

* As part of our commitment to security, we have identified and resolved high-priority vulnerabilities, strengthening the overall security of the Inforiver Writeback Matrix.
* The LastUpdatedAt and LastUpdatedBy housekeeping columns did not reflect changes made in slicer selections. This issue has been resolved.

{% hint style="info" %}
In this example, we've used the Power BI-certified Inforiver SuperFilter visual to filter the regions.
{% endhint %}

<figure><img src="../.gitbook/assets/Untitled Project.gif" alt=""><figcaption><p>Context awareness for housekeeping columns</p></figcaption></figure>

* When the cell value is deleted in the source report for a formula measure referencing a data input number field, the Infobridge preview was throwing an error.  This issue has been rectified, and the updated null values are displayed correctly in the bridge.

