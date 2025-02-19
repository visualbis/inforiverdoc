# SEPARATOR

Use the SEPARATOR function to set custom delimiters for decimals and thousands.

### Syntax

```javascript
SEPARATOR.<TYPE>(VALUE)
```

### Arguments

TYPE - DECIMAL or THOUSAND depending on the separator you need to change.

VALUE - The custom separator to use instead of the default ones.

### Example

```
SEPARATOR.DECIMAL('d')
SEPARATOR.THOUSAND('t')
```

<figure><img src="../../../.gitbook/assets/image (1235).png" alt=""><figcaption><p>Separator function in a button variable</p></figcaption></figure>

When we click the buttons, the default '.' separator for decimal and ','  separator for thousands are replaced with 'd' and 't' respectively. The buttons use the SEPARATOR script options internally to change the separator.

<figure><img src="../../../.gitbook/assets/Untitled Project (20).gif" alt=""><figcaption><p>Changing the separator</p></figcaption></figure>
