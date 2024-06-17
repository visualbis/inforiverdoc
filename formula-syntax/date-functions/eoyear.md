# EOYEAR

The EOYEAR function takes the date as input and returns the ending date of the year. Node references and measures are also accepted as input arguments. Use [DATE.SET()](https://docs.inforiver.com/\~/changes/mS6jwvARNLHpKqBa4cT9/formula-syntax/date-functions/date.set) to set the format of the output date.

Optionally, you can specify an offset for the return date, which may be a positive or negative number. Additional years are added to or subtracted from the end date depending on the offset value.

## Syntax <a href="#syntax" id="syntax"></a>

```java
EOYEAR(date)
EOYEAR(date,offset)
```

## Arguments <a href="#arguments" id="arguments"></a>

date - The date which is passed as an input to the function. Required.

offset - Number of years to be added to or subtracted from the end date of the month. Optional.

## Return value <a href="#return-value" id="return-value"></a>

Date representing the end of the year.

## Example <a href="#example" id="example"></a>

```java
EOYEAR("05/29/2024")
//Returns 31/12/2024
EOYEAR("5/29/2024",1)
//Returns 31/12/2025, adding 1 year to 31/12/2024
```

<figure><img src="../../.gitbook/assets/image (730).png" alt=""><figcaption><p>EOYEAR</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (731).png" alt=""><figcaption><p>EOYEAR with offset</p></figcaption></figure>
