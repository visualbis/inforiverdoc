# FROMEXCELDATE

Excel stores dates as sequential serial numbers so that they can be used in calculations. The FROMEXCELDATE function converts an excel recognized serial number to the equivalent date in DD/MM/YYYY format. Node references are also accepted as arguments.

## Syntax

```javascript
fromexceldate(value)
```

## Arguments

value- The numeric excel date value.

## Return value

Date

## Example

```javascript
fromexceldate(39457)
```

Returns 10/1/2008.

<figure><img src="../../.gitbook/assets/image (219).png" alt=""><figcaption><p>Fromexceldate function</p></figcaption></figure>
