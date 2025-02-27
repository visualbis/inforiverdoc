# GETMEASURE

The GETMEASURE function can be used to select data from a native measure based on its index. It should be used with an aggregate function like SUM or AVERAGE.&#x20;

## Syntax

```javascript
GETCOLBETWEENPERIODS(index, type)
```

## Arguments

index– Order of the native measure in the AC/PY/PL/FC bucket. Required.

type– Can be AC/PY/PL or FC. Required.

## Example

```javascript
GETMEASURE(1, "AC")
//Returns the first native measure in the AC bucket

GETMEASURE(2, "PY")
//Returns the second native measure in the PY bucket
```

<figure><img src="../../.gitbook/assets/image (1274).png" alt=""><figcaption><p>GETMEASURE</p></figcaption></figure>
