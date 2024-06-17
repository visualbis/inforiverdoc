# SOQTR

The SOQTR function takes the date as input and returns the starting date of the quarter. Node references and measures are also accepted as input arguments. Use [DATE.SET()](https://docs.inforiver.com/\~/changes/mS6jwvARNLHpKqBa4cT9/formula-syntax/date-functions/date.set) to set the format of the output date.

## Syntax <a href="#syntax" id="syntax"></a>

```java
SOQTR(date)
```

## Arguments <a href="#arguments" id="arguments"></a>

date - The date which is passed as an input to the function. Required.

## Return value <a href="#return-value" id="return-value"></a>

Date representing the start of the quarter.

## Example <a href="#example" id="example"></a>

```java
SOQTR("05/29/2024")
//Returns 1/4/2024
```

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption><p>SOQTR</p></figcaption></figure>
