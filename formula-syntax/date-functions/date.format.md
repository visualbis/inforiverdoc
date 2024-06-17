# DATE.FORMAT

The DATE.FORMAT() function returns the date in the user-specified string format. If the format is not specified the date is converted to the format based on the user's browser locale.&#x20;



## Syntax

```java
DATE.FORMAT("format")
//returns the current date in the specified string format
```



## Arguments

format -  String. This specifies the format in which the current date should be displayed. Optional.



## Return Value

Date as a string.



## Example

```java
DATE.FORMAT()
//returns 11/6/24 (current date in the format based on the user's browser locale)
DATE.FORMAT("DD MM YY")
//returns 11 06 24
```

<figure><img src="../../.gitbook/assets/image (725).png" alt=""><figcaption><p>DATE.FORMAT</p></figcaption></figure>
