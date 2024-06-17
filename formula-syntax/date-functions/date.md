# DATE

The DATE function takes date as input, in the form of a string or as a tuple and returns it in the specified format. If the format is not specified it returns the date in the user's browser locale format.&#x20;

## Syntax

```java
DATE(date,format)
//returns the date in the specified format

DATE(year,month,date)
//returns the date in the browser locale format
```

## Arguments

date - The input date in the form of a string. It can also be a node reference or a measure that contains the date. Required.

format - The desired format in which the input date should be displayed. Optional.

(or)

year - number.

month - number.

date - number.

## Return Value

Date.

## Example

```java
DATE("05/29/2024")
//returns 29/5/2024

DATE(2024,05,24)
//returns 24/5/2024
```

<figure><img src="../../.gitbook/assets/image (6) (1).png" alt=""><figcaption></figcaption></figure>
