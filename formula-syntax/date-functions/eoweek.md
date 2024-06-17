# EOWEEK

The EOWEEK function takes the date as input and returns the ending date of the week. Node references and measures are also accepted as input arguments. Use [DATE.SET()](https://docs.inforiver.com/\~/changes/mS6jwvARNLHpKqBa4cT9/formula-syntax/date-functions/date.set) to set the format of the output date.

Optionally, you can specify an offset for the return date, which may be a positive or negative number. Additional weeks are added to or subtracted from the end date depending on the offset value.

## Syntax <a href="#syntax" id="syntax"></a>

```java
EOWEEK(date)
EOWEEK(date,offset)
```

## Arguments <a href="#arguments" id="arguments"></a>

date - The date which is passed as an input to the function. Required.

offset - Number of weeks to be added to or subtracted from the end date of the week. Optional.

## Return value <a href="#return-value" id="return-value"></a>

Date representing the end of the week.

## Example <a href="#example" id="example"></a>

```java
EOWEEK("05/29/2024")
//Returns 2/6/2024
EOWEEK("05/29/2024",3)
//Returns 23/6/2024, adding 3 more weeks to 2/6/2024
```

<figure><img src="../../.gitbook/assets/image (5) (1).png" alt=""><figcaption><p>EOWEEK</p></figcaption></figure>

If you wish to add one or two more weeks to the ending date, you can use 1 or 2 as offset values respectively.

<figure><img src="../../.gitbook/assets/image (726).png" alt=""><figcaption><p>EOWEEK with offset </p></figcaption></figure>
