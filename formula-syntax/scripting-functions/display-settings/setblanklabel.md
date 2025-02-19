# SETBLANKLABEL

SETBLANKLABEL can be used to replace blank row or column categories with custom text.

### Syntax

```javascript
SETBLANKLABEL.<ROW/COLUMN>(VALUE)
```

### Arguments

VALUE - Pass the custom value to use instead of blank categories.

### Example

```
SETBLANKLABEL.ROW('row_label')
SETBLANKLABEL.COLUMN('col_label')
```

<figure><img src="../../../.gitbook/assets/image (1242).png" alt=""><figcaption><p>SETBLANKLABEL function used in a variable</p></figcaption></figure>

Notice how the blank row and column categories are replaced with the custom text "DESC". The buttons use the SETBLANKLABEL script internally.

<figure><img src="../../../.gitbook/assets/Untitled Project (24).gif" alt=""><figcaption><p>SETBLANKLABEL function in action</p></figcaption></figure>
