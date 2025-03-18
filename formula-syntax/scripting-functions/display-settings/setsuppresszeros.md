# SETSUPPRESSZEROS

SETSUPPRESSZERO can be used to show or hide zero values in reports.

### Syntax

```javascript
SETSUPPRESSZEROS(VALUE)
```

### Arguments

VALUE - Pass a boolean value of TRUE or FALSE.

### Example

```
SETSUPPRESSZEROS(TRUE) //Suppresses zeroes
SETSUPPRESSZEROS(FALSE) //Displays zeroes
```

<figure><img src="../../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Set suppress zeroes</p></figcaption></figure>

Notice how the _Depreciation_ row that only contains zeroes is suppressed when the SuppressZeroes button is clicked and displayed again when the DisplayZeroes button is clicked. The buttons use the SETSUPPRESSZERO script internally to hide and display zero values.

<figure><img src="../../../.gitbook/assets/Untitled Project.gif" alt=""><figcaption><p>Suppress zeroes script in action</p></figcaption></figure>
