# Find and Replace

As the name implies, the Find and Replace option searches a particular dimension column for a string or value and replaces it with the given string. Let's consider a Global market report to demonstrate this.

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Sample report</p></figcaption></figure>

We'll look at the inputs required to replace the "Bovespa Index" benchmark with "S\&P 500" in the Benchmark column.

<figure><img src="../../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption><p>Find and Replace configuration</p></figcaption></figure>

* **Target columns:** You can select one or more columns from the dropdowns. These columns will be searched and replaced with the given value if the search string is found.
* **Find**: The string to search for.
* **Match Case:** You can opt for a fuzzy match, exact match or even provide a regular expression. Let's use a regex to replace all the Benchmarks that contain "Bovespa Index".

<figure><img src="../../.gitbook/assets/image (1293).png" alt=""><figcaption><p>Find and replace with regular expressions</p></figcaption></figure>

* **Replace with:** The new string/value that will replace the search string.
