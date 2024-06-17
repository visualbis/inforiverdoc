# NETWORKDAYS

The NETWORKDAYS function returns the number of workdays between two dates. It accepts two dates as inputs.&#x20;

## Syntax <a href="#syntax" id="syntax"></a>

```java
NETWORKDAYS(fromDate,toDate)
```

## Arguments <a href="#arguments" id="arguments"></a>

fromDate - Starting date in the range. Required. This can be a date, a node reference or a measure that includes the date.

toDate- Ending date in the range. Required. This can be a date, a node reference or a measure that includes the date.

## Return value <a href="#return-value" id="return-value"></a>

Number.

## Example <a href="#example" id="example"></a>

```java
NETWORKDAYS("05/31/2024","06/30/2024")
//Returns 22
```

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption><p>NETWORKDAYS</p></figcaption></figure>
