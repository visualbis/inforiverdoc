# HAS\_SOME

Checks whether some of the searchValues are part of the list

## Syntax

```javascript
HAS_SOME(value1,”searchValue”)
HAS_SOME(value1,value2…”,searchValues”)
```

## **Example**

```javascript
HAS_SOME(Column1,[“ABC”,”DEF”)]
```

&#x20;  If Column1 contains both “ABC” and “DEF” returns TRUE

```javascript
HAS_SOME(Column1, Column2,Column3 [“ABC”,”DEF”)]
```

&#x20;  If any of the columns has “ABC” and “DEF” as value, returns TRUE
