# REPLACE

The REPLACE function replaces an input text string with a given value for a specified index and length. Node references are also accepted as arguments. The index starts at 1 i.e. the first character of the input string will have an index of 1.&#x20;

## Syntax

```javascript
replace(old_string:string, index:number, length:number, replace_text:string)
```

## Arguments

old\_string- Required. A text string.

index- Required. A number indicating the position at which the string should be replaced.

length- Required. A number indicating the number of characters to be replaced in the input string.

replace\_text- Required. A text string that will replace a part/all of the old\_string parameter.

## Example

```javascript
REPLACE('INFORIVER', 1, 4, 'LUMEL')
```

Returns “LUMELRIVER".

<figure><img src="../../.gitbook/assets/image (225).png" alt=""><figcaption></figcaption></figure>
