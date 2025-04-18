# Text functions

## 1. Extract

Reports may often contain concatenated values that need to be split. Use the **Extract** option to extract a string or character from a text field or split a text field.&#x20;

You can choose different options, such as range, length, first/last character, or splitting the string based on a delimiter.

**1.1. Range**

Extracts text based on the start and end position of the string to be extracted. Let's extract the city code from the "AreaCode" column. We need to specify the starting position of the text to be extracted and the number of characters to extract.

<figure><img src="../../.gitbook/assets/image (9) (1) (1).png" alt=""><figcaption><p>Extract a range of data</p></figcaption></figure>

The city code is extracted from the area code and captured as a separate dimension.

<figure><img src="../../.gitbook/assets/image (1305).png" alt=""><figcaption><p>Extracted text using the range option</p></figcaption></figure>

**1.2. Length**

Capture the text length in a separate dimension by choosing the **Length** option.&#x20;

<figure><img src="../../.gitbook/assets/image (1306).png" alt=""><figcaption><p>Extract text length for a selected field in the report</p></figcaption></figure>

The length of the "Category" column has been extracted into a new dimension titled "Category length".

<figure><img src="../../.gitbook/assets/image (1307).png" alt=""><figcaption><p>Length of the Category dimension extracted into a new field</p></figcaption></figure>

**1.3. First characters**

Extract the first n characters from a text field. Let's pull the ID (first 5 characters) from the Customer ID field.

<figure><img src="../../.gitbook/assets/image (1308).png" alt=""><figcaption><p>Customer ID field</p></figcaption></figure>

Extract configuration to pull the first 5 characters from a field.

<figure><img src="../../.gitbook/assets/image (1309).png" alt=""><figcaption><p>Extract ID from the Customer ID field</p></figcaption></figure>

A new dimension containing the ID is created.

<figure><img src="../../.gitbook/assets/image (1310).png" alt=""><figcaption><p>First 5 characters extracted into a new dimension</p></figcaption></figure>

**1.4. Last characters**

Similar to the first characters option, **Last Characters** will pull the last n characters from a string.&#x20;

**1.5. Text before delimiters**

Extracts the text before a specific delimiter. Let's extract the currency code from the "Discount Index" field.

<figure><img src="../../.gitbook/assets/image (1301).png" alt=""><figcaption><p>Sample report to demonstrate the Extract function</p></figcaption></figure>

Select the **Text Before Delimiters** option and enter "-" in the Delimiter text box.

<figure><img src="../../.gitbook/assets/image (1300).png" alt=""><figcaption><p>Extract before delimiter option for delimited text</p></figcaption></figure>

The currency code has been extracted into a separate dimension.&#x20;

<figure><img src="../../.gitbook/assets/image (1302).png" alt=""><figcaption><p>New dimension created with the extracted values</p></figcaption></figure>

**1.6. Text after delimiters**

Extracts the text after a specific delimiter. Let's take the same example to extract the frequency from the Discount Index column. Select the **Text After Delimiters** option and enter "-" in the Delimiter text box.

<figure><img src="../../.gitbook/assets/image (1303).png" alt=""><figcaption><p>Extracting strings after a delimiter</p></figcaption></figure>

You'll see that a new dimension is created containing the text after the specified delimiter.

<figure><img src="../../.gitbook/assets/image (1304).png" alt=""><figcaption></figcaption></figure>

## 2. Format

Use the format option to perform operations like changing the case, trimming or adding a prefix/suffix to your text data.

<figure><img src="../../.gitbook/assets/image (1312).png" alt=""><figcaption><p>Text formatting options</p></figcaption></figure>

#### 2.1. Changing the case

We may need to change the case of source data to ensure data consistency or search accuracy for case-sensitive systems. Let's change the case of the "Category" and "Segment" fields to uppercase.

<figure><img src="../../.gitbook/assets/image (1313).png" alt=""><figcaption><p>Changing the case of text fields</p></figcaption></figure>

Notice how the data in both fields is in uppercase.

<figure><img src="../../.gitbook/assets/image (1314).png" alt=""><figcaption><p>Data after converting to uppercase</p></figcaption></figure>

#### 2.2. Trim

Leading or trailing spaces can cause mismatches in comparisons and can lead to inconsistencies in your data. The Account field has trailing spaces, so we'll use the **Trim** option to remove them.

<figure><img src="../../.gitbook/assets/image (1316).png" alt=""><figcaption><p>Formatting text - trim spaces</p></figcaption></figure>

The trailing spaces in the Account field have now been trimmed:

<figure><img src="../../.gitbook/assets/image (1317).png" alt=""><figcaption><p>Trimmed data</p></figcaption></figure>

#### 2.3. Add prefix/suffix

Adding a prefix or suffix can help in easy identification and categorization of data. They are also used in generating unique identifiers. Let's add a prefix to the Account number.

<figure><img src="../../.gitbook/assets/image (1318).png" alt=""><figcaption><p>Adding a prefix or suffix</p></figcaption></figure>

You'll notice that the account numbers have an "ACC" prefix added.

<figure><img src="../../.gitbook/assets/image (1319).png" alt=""><figcaption><p>Prefix added to the Account field</p></figcaption></figure>

