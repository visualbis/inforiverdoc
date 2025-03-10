# Filter rows

Add filters to retain only rows required in the target visuals. You can specify filter conditions, only the rows that satisfy the conditions will be available in the query.

Let's consider the sample report below to demonstrate how to filter data.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1).png" alt=""><figcaption><p>Sample data</p></figcaption></figure>

We can use the filter configuration shown below to retain only the rows with "Domestic" or "North America" as the global market and COGS > 200k.

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1).png" alt=""><figcaption><p>Filter config</p></figcaption></figure>

You need to specify the options listed below to configure a filter:

* **Column name:** The measure or dimension on which the filter is based.
* **Operator**: This can change depending on the data in a column. For text data, use conditions are is/is not/in/not in. For numeric data, use conditions like is/is not/less than/greater than/less than or equal to/greater than or equal to etc.
* **Value:** Either key in the string/number or select from the dropdown.
* **Add Filter:** Click the link to add multiple and/or conditions.

Notice how the rows have been filtered out from the report based on the filter conditions specified.

<figure><img src="../../.gitbook/assets/image (1296).png" alt=""><figcaption><p>Filtered data</p></figcaption></figure>
