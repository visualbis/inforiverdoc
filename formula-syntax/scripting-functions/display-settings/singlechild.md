# SINGLECHILD

Use SINGLECHILD options to select which nodes to display when a parent hierarchy has only one child. [Learn more about single-child options for hierarchies.](../../../display-settings/hierarchy-settings.md#id-4.2.-single-child)

### Syntax

```javascript
SINGLECHILD.<SINGLECHILD OPTIONS>
```

### Arguments

SINGLECHILD OPTIONS - Can be ALL, PARENTONLY, PARENTMULTILEVEL, LEVELASPARENT,  ASPARENT depending on how you want to display your hierarchy.

### Example

```
SINGLECHILD.ALL // Displays all single children
SINGLECHILD.PARENTONLY // Displays the parent Only
SINGLECHILD.PARENTMULTILEVEL //Displays the parent for multi-level hierarchies with single children
SINGLECHILD.LEVELASPARENT // Displays the single child level as the parent
SINGLECHILD.ASPARENT // Displays the single child at the lowest level as the parent
```

<figure><img src="../../../.gitbook/assets/image (1233).png" alt=""><figcaption><p>Single child functions used in variables</p></figcaption></figure>

Notice how the single child nodes are displayed depending on the button clicked. The buttons use the SINGLECHILD script options internally to display single-child row categories.

<figure><img src="../../../.gitbook/assets/Untitled Project (18).gif" alt=""><figcaption><p>Single child options for unbalanced hierarchies</p></figcaption></figure>
