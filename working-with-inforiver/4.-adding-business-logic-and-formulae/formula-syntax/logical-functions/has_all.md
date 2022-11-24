# HAS\_ALL

Checks whether all the searchValues are part of the list

## Syntax

```javascript
HAS_ALL(value1,”searchValues”)
HAS_ALL(value1,value2…”,searchValues”)
```

## **Example**

* HAS\_ALL(Column1,\[“ABC”,”DEF”)]

&#x20;     If Column1 contains both “ABC” and “DEF” returns TRUE

* HAS\_ALL(Column1, Column2,Column3 \[“ABC”,”DEF”)]

&#x20;     If any of the columns has “ABC” and “DEF” as value, returns TRUE
