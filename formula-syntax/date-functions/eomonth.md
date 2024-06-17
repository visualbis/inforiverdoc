# EOMONTH

The EOMONTH function takes the date as input and returns the ending date of the month. Node references and measures are also accepted as input arguments. Use [DATE.SET()](https://docs.inforiver.com/\~/changes/mS6jwvARNLHpKqBa4cT9/formula-syntax/date-functions/date.set) to set the format of the output date.

Optionally, you can specify an offset for the return date, which may be a positive or negative number. Additional months are added to or subtracted from the end date depending on the offset value.

## Syntax <a href="#syntax" id="syntax"></a>

```java
EOMONTH(date)
EOMONTH(date,offset)
```

## Arguments <a href="#arguments" id="arguments"></a>

date - The date which is passed as an input to the function. Required.

offset - Number of months to be added to or subtracted from the end date of the month. Optional.

## Return value <a href="#return-value" id="return-value"></a>

Date representing the end of the month.

## Example <a href="#example" id="example"></a>

```java
EOMONTH("05/29/2024")
//Returns 31/5/2024
EOMONTH("05/29/2024",3)
//Returns 31/8/2024, adding 3 more months to 31/5/2024
```

<figure><img src="../../.gitbook/assets/image (727).png" alt=""><figcaption><p>EOMONTH</p></figcaption></figure>

If you wish to add one or two more months to the ending date, you can use 1 or 2 as offset values respectively.

<figure><img src="../../.gitbook/assets/image (728).png" alt=""><figcaption><p>EOMONTH with offset</p></figcaption></figure>
