# SETRAGGEDHIERARCHY

SETRAGGEDHIERARCHY can be used to hide blank categories when you have uneven/unbalanced hierarchical data.

### Syntax

```javascript
SETRAGGEDHIERARCHY(VALUE)
```

### Arguments

VALUE - Pass a boolean value of TRUE or FALSE.

### Example

```
SETRAGGEDHIERARCHY(TRUE) //Suppresses blank categories
SETRAGGEDHIERARCHY(FALSE) //Displays blank categories
```

<figure><img src="../../../.gitbook/assets/image (1232).png" alt=""><figcaption></figcaption></figure>

Notice how the blank category rows are suppressed when the EnableRaggedHierarchy button is clicked and displayed again when the DisableRaggedhierarchy button is clicked. The buttons use the SETRAGGEDHIERARCHY script internally to hide and display blank categories.

<figure><img src="../../../.gitbook/assets/Untitled Project (17).gif" alt=""><figcaption><p>SETRAGGEDHIERARCHY function in action</p></figcaption></figure>
