# EOQTR

The EOQTR function takes the date as input and returns the ending date of the quarter. Node references and measures are also accepted as input arguments. Use [DATE.SET()](https://docs.inforiver.com/\~/changes/mS6jwvARNLHpKqBa4cT9/formula-syntax/date-functions/date.set) to set the format of the output date.

Optionally, you can specify an offset for the return date, which may be a positive or negative number. Additional quarters are added to or subtracted from the end date depending on the offset value.

## Syntax <a href="#syntax" id="syntax"></a>

```java
EOQTR(date)
EOQTR(date,offset)
```

## Arguments <a href="#arguments" id="arguments"></a>

date - The date which is passed as an input to the function. Required.

offset - Number of quarters to be added to or subtracted from the end date of the month. Optional.

## Return value <a href="#return-value" id="return-value"></a>

Date representing the end of the quarter.

## Example <a href="#example" id="example"></a>

```java
EOQTR("05/29/2024")
//Returns 30/6/2024
EOQTR("05/29/2024",1)
//Returns 30/9/2024, adding 1 more quarter to 30/6/2024
```

<figure><img src="../../.gitbook/assets/image (729) (2).png" alt=""><figcaption><p>EOQTR</p></figcaption></figure>

