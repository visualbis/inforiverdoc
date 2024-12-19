# LOOKUP

The LOOKUP function can look up values from an Infobridge query and load them inside an Inforiver visual. It can fetch measure values directly from Infobridge without creating an integration and importing measures/rows into your report.  

## Syntax

```javascript
LOOKUP(queryIdentifier:string,measure:string,rows:[string],columns:[string])
//fetches data from the specified query and measure
```

## Arguments

queryIdentifier - String. Required. It is used to identify the query from which data has to be fetched.

<figure><img src="../../.gitbook/assets/image (1075).png" alt=""><figcaption><p>Copy the query GUID from Infobridge</p></figcaption></figure>

key- String. Required. It specifies the key whose value is to be extracted.

rows - Array. Optional. Specify specific row dimension category values or use dimension names.

columns- Array. Optional. Specify specific column dimension category values or use dimension names.

## Examples

**Example 1:** Refer to a specific row and column and fetch the measure value from Infobridge.

The bridge contains the quarterly rebate rates for a set of products.

<figure><img src="../../.gitbook/assets/image (1073).png" alt=""><figcaption><p>Bridge to lookup measure values</p></figcaption></figure>

In the target visual, we can pull the rebate rate for the "Velo" product for Q4 using the LOOKUP function as shown.

<figure><img src="../../.gitbook/assets/image (1074).png" alt=""><figcaption><p>LOOKUP function for specific row and column dimension categories</p></figcaption></figure>

**Example 2:** Fetch values when the row and column dimensions are the same in the bridge and the target visual.

The bridge contains the country-wise rebate rates for a set of products.

<figure><img src="../../.gitbook/assets/image (1076).png" alt=""><figcaption><p>Bridge to lookup measure values</p></figcaption></figure>

In the target visual, we can pull the rebate rate without specifying the rows and columns. They are automatically mapped within Inforiver.

<figure><img src="../../.gitbook/assets/image (1077).png" alt=""><figcaption><p>LOOKUP function when the row and column dimensions match in the bridge and target visual</p></figcaption></figure>

You can use the ROW/COLUMN identifiers when the row and column dimensions in the bridge and identical to the target visual.

<figure><img src="../../.gitbook/assets/image (1078).png" alt=""><figcaption><p>Using the ROW and COLUMN identifiers</p></figcaption></figure>

**Example 2:** Fetch values when the row and column dimensions in the bridge and the target visual are not identical.

The bridge contains a flat discount rate for product categories.

<figure><img src="../../.gitbook/assets/image (1079).png" alt=""><figcaption><p>Bridge to lookup measure values</p></figcaption></figure>

In the target visual, we can pull the discount rate although the the bridge does not contain column dimensions and the row dimension hierarchy is different.

<figure><img src="../../.gitbook/assets/image (1080).png" alt=""><figcaption><p>Lookup when dimensions do not match</p></figcaption></figure>

You can also fetch values from a bridge and map them to a visual column.

<figure><img src="../../.gitbook/assets/image (1081).png" alt=""><figcaption></figcaption></figure>
