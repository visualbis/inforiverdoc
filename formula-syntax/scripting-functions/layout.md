# LAYOUT

Layout functions can be used to set the layout, set a theme, enable/disable rails, or expand the hierarchy to a particular level. Let's take a look at the various options.



<table><thead><tr><th width="300">NAME</th><th>DESCRIPTION</th></tr></thead><tbody><tr><td><a href="layout.md#id-1.-layout.hierarchical">LAYOUT.HIERARCHY</a></td><td>Sets the layout to hierarchy</td></tr><tr><td><a href="layout.md#id-2.-layout.outline">LAYOUT.OUTLINE</a></td><td>Sets the layout to outline</td></tr><tr><td><a href="layout.md#id-3.-layout.table">LAYOUT.TABLE</a></td><td>Sets the layout to table</td></tr><tr><td><a href="layout.md#id-4.-layout.stepped">LAYOUT.STEPPED</a></td><td>Sets the layout to stepped</td></tr><tr><td><a href="layout.md#id-5.-layout.drilldown">LAYOUT.DRILLDOWN</a></td><td>Sets the layout to drilldown</td></tr><tr><td><a href="layout.md#id-6.-layout.lighttheme">LAYOUT.LIGHTTHEME</a></td><td>Applies a light canvas</td></tr><tr><td><a href="layout.md#id-7.-layout.darktheme">LAYOUT.DARKTHEME</a></td><td>Applies a dark canvas</td></tr><tr><td><a href="layout.md#id-8.-layout.autofit">LAYOUT.AUTOFIT</a></td><td>Fits the maximum possible data in the available space</td></tr><tr><td><a href="layout.md#id-9.-layout.setruler">LAYOUT.SETRULER</a></td><td>Enable or disable the ruler</td></tr><tr><td><a href="layout.md#id-10.-layout.gotocolumnlevel">LAYOUT.GOTOCOLUMNLEVEL</a></td><td>Expands the column hierarchy to the specified level</td></tr><tr><td><a href="layout.md#id-11.-layout.gotorowlevel">LAYOUT.GOTOROWLEVEL</a></td><td>Expands the row hierarchy to the specified level</td></tr></tbody></table>



## 1. LAYOUT.HIERARCHICAL

Sets the layout option to hierarchy and displays the data in a hierarchical format.

### Syntax

```javascript
LAYOUT.HIERARCHICAL
```

<figure><img src="../../.gitbook/assets/image (383).png" alt=""><figcaption><p>Layout hierarchical</p></figcaption></figure>

## 2. LAYOUT.OUTLINE

Sets the layout option to outline.

### Syntax

```javascript
LAYOUT.OUTLINE
```

<figure><img src="../../.gitbook/assets/image (384).png" alt=""><figcaption><p>Setting the layout to outline</p></figcaption></figure>

## 3. LAYOUT.TABLE

Sets the layout option to table.

### Syntax

```javascript
LAYOUT.TABLE
```

<figure><img src="../../.gitbook/assets/image (385).png" alt=""><figcaption><p>Setting the layout to table</p></figcaption></figure>

## 4. LAYOUT.STEPPED

Sets the layout option to stepped.

### Syntax

```javascript
LAYOUT.STEPPED
```

<figure><img src="../../.gitbook/assets/image (386).png" alt=""><figcaption><p>Setting the layout to stepped</p></figcaption></figure>

## 5. LAYOUT.DRILLDOWN

Sets the layout option to drilldown.

### Syntax

```javascript
LAYOUT.DRILLDOWN
```

<figure><img src="../../.gitbook/assets/image (387).png" alt=""><figcaption><p>Setting the layout to drilldown</p></figcaption></figure>

## 6. LAYOUT.LIGHTTHEME

Sets a light background for the canvas.

### Syntax

```javascript
LAYOUT.LIGHTTHEME
```

<figure><img src="../../.gitbook/assets/image (388).png" alt=""><figcaption><p>Setting a light canvas</p></figcaption></figure>

## 7. LAYOUT.DARKTHEME

Sets a light background for the canvas.

### Syntax

```javascript
LAYOUT.DARKTHEME
```

<figure><img src="../../.gitbook/assets/image (389).png" alt=""><figcaption><p>Setting a dark background</p></figcaption></figure>

## 8. LAYOUT.AUTOFIT

Fits the maximum possible data in the available space.

### Syntax

```javascript
LAYOUT.AUTOFIT
```

<figure><img src="../../.gitbook/assets/image (390).png" alt=""><figcaption><p>Autofit layout</p></figcaption></figure>

## 9. LAYOUT.SETRULER

Fits the maximum possible data in the available space.

### Syntax

```javascript
LAYOUT.SETRULER(TRUE) #Enables the ruler
LAYOUT.SETRULER(FALSE) #Disables the ruler
LAYOUT.SETRULER(THIS) #Control the 'THIS' parameter using a toggle variable button
```

<figure><img src="../../.gitbook/assets/image (391).png" alt=""><figcaption><p>Ruler enabled using set ruler</p></figcaption></figure>

## 10. LAYOUT.GOTOCOLUMNLEVEL

Expands the column hierarchy to the specified level. The highest level of the hierarchy is denoted by '0'.&#x20;

### Syntax

```
LAYOUT.GOTOCOLUMNLEVEL(1) #Expands to the second level of the column hierarchy
LAYOUT.GOTOCOLUMNLEVEL(THIS) #Expands to the specified level which can be set using a numerical stepper variable
```

<figure><img src="../../.gitbook/assets/image (392).png" alt=""><figcaption><p>Expanding the column hierarchy</p></figcaption></figure>

## 11. LAYOUT.GOTOROWLEVEL

Expands the row hierarchy to the specified level. The highest level of the hierarchy is denoted by '0'.&#x20;

### Syntax

```
LAYOUT.GOTOROWLEVEL(2) #Expands to the third level of the column hierarchy
LAYOUT.GOTOROWLEVEL(THIS) #Expands to the specified level which can be set using a numerical stepper variable
```

<figure><img src="../../.gitbook/assets/image (393).png" alt=""><figcaption><p>Expanded row hierarchy</p></figcaption></figure>

