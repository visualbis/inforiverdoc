# Text functions

## 1. Extract

Reports may often contain concatenated values that need to be split. Use the **Extract** option to extract a string or character from a text field or split a text field.&#x20;

You can choose different options, such as range, length, first/last character, or splitting the string based on a delimiter.

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

