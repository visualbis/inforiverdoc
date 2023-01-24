# MID

The MID function returns a specific number of characters from a text string, starting at the position you specify, based on the number of characters you specify. When used with a number, the resultant value is stored as text.

## Syntax

```javascript
mid (text, position, length)
```

## Arguments

text/number - Required. The text string containing the characters you want to extract.

position - Required. The position of the first character you want to extract in the text.

length - Required. Specifies the number of characters you want MID to return from the text.

## Example

```javascript
mid([Full Name],0,7)
```

When the field Full Name has the value Johny Rivers, this will return Johny R

## **Excel equivalent**

[MID](https://support.microsoft.com/en-us/office/mid-midb-functions-d5f9e25c-d7d6-472e-b568-4ecb12433028)
