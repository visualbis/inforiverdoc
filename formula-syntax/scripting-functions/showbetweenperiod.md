# SHOWBETWEENPERIOD

Displays the data between the time frame specified. Can be used to display months, quarters, and year periods.

<table><thead><tr><th width="369">NAME</th><th>DESCRIPTION</th></tr></thead><tbody><tr><td><a href="showbetweenperiod.md#id-1.-showbetweenperiod-monthperiod">SHOWBETWEENPERIOD(MONTHPERIOD)</a></td><td>Shows the months between the specified periods</td></tr><tr><td><a href="showbetweenperiod.md#id-2.-showbetweenperiod-qtrperiod">SHOWBETWEENPERIOD(QTRPERIOD)</a></td><td>Shows the quarters between the specified periods</td></tr><tr><td><a href="showbetweenperiod.md#id-3.-showbetweenperiod-yearperiod">SHOWBETWEENPERIOD(YEARPERIOD)</a></td><td>Shows the years between the specified periods</td></tr><tr><td><a href="showbetweenperiod.md#id-4.-showbetweenperiod-lastnday">SHOWBETWEENPERIOD(LASTNDAY)</a></td><td>Returns data for last n days</td></tr><tr><td><a href="showbetweenperiod.md#id-5.-showbetweenperiod-lastnmonth">SHOWBETWEENPERIOD(LASTNMONTH)</a></td><td>Returns data for last n months</td></tr><tr><td><a href="showbetweenperiod.md#id-6.-showbetweenperiod-lastnyear">SHOWBETWEENPERIOD(LASTNQTR)</a></td><td>Returns data for last n quarters</td></tr><tr><td><a href="showbetweenperiod.md#id-7.-showbetweenperiod-nextnday">SHOWBETWEENPERIOD(LASTNYEAR)</a></td><td>Returns data for last n years</td></tr></tbody></table>

### 1. SHOWBETWEENPERIOD(MONTHPERIOD)

The SHOWBETWEENPERIOD(MONTHPERIOD) function can be used to display data for a particular month or a range of months.&#x20;

### Syntax

```javascript
SHOWBETWEENPERIOD(MONTHPERIOD(year, from_month, to_month))
```

## Arguments

year – The year for which data has to be fetched. Required.

from\_month – The month for which data has to be fetched or the start month if a range is specified. Values can be between 1 and 12. Required.

to\_month - The end month when a range of data has to be fetched. Values can be between 1 and 12. Optional.

### Example

```
SHOWBETWEENPERIOD(MONTHPERIOD(2023,2,8)) #Displays the 2023 data between Feb and August
SHOWBETWEENPERIOD(MONTHPERIOD(2023,10)) #Displays the data for 2023 October
```

<figure><img src="../../.gitbook/assets/image (407).png" alt=""><figcaption><p>SHOWBETWEENPERIOD - MONTHPERIOD</p></figcaption></figure>

### 2. SHOWBETWEENPERIOD(QTRPERIOD)

The SHOWBETWEENPERIOD(QTRPERIOD) function can be used to display data for a particular quarter or a range of quarters.&#x20;

### Syntax

```javascript
SHOWBETWEENPERIOD(QTRPERIOD(year, from_qtr, to_qtr))
```

## Arguments

year – The year for which data has to be fetched. Required.

from\_qtr – The quarter for which data has to be fetched or the starting quarter if a range is specified. Values can be between 1 and 4. Required.

to\_qtr - The end quarter when a range of data has to be fetched. Values can be between 1 and 4. Optional.

### Example

```
SHOWBETWEENPERIOD(QTRPERIOD(2023,2,4)) #Displays the 2023 data between the 2nd and 4th quarter
SHOWBETWEENPERIOD(QTRPERIOD(2023,3)) #Displays the data for the 3rd quarter of 2023
```

<figure><img src="../../.gitbook/assets/image (408).png" alt=""><figcaption><p>SHOWBETWEENPERIOD - QTRPERIOD</p></figcaption></figure>

### &#x20;3. SHOWBETWEENPERIOD(YEARPERIOD)

The SHOWBETWEENPERIOD(YEARPERIOD) function can be used to select data for a particular year or a range of years.&#x20;

### Syntax

```javascript
SHOWBETWEENPERIOD(YEARPERIOD(start_year, end_year))
```

## Arguments

start\_year – The year for which data has to be fetched or the starting year if a range is specified. Values should be in YYYY format. Required.

end\_year- The end year when a range of data has to be fetched. Values should be in YYYY format. Optional.

### Example

```
SHOWBETWEENPERIOD(YEARPERIOD(2021,2023)) #Displays the data between 2021 and 2023
SHOWBETWEENPERIOD(YEARPERIOD(2023)) #Displays the data for 2023
```

<figure><img src="../../.gitbook/assets/image (409).png" alt=""><figcaption><p>SHOWBETWEENPERIOD - YEARPERIOD</p></figcaption></figure>

### 4. SHOWBETWEENPERIOD(LASTNDAY)

The SHOWBETWEENPERIOD(LASTNDAY) function can be used to display data for a specified number of days preceding the current day.

### Syntax

```javascript
SHOWBETWEENPERIOD(LASTNDAY, number_of_days)
```

## Arguments

number\_of\_days – The number of days for which to fetch data. Required.

### Example

```
SHOWBETWEENPERIOD(LASTNDAY, 15) #Displays data for the past two weeks
```

### 5. SHOWBETWEENPERIOD(LASTNMONTH)

The SHOWBETWEENPERIOD(LASTNMONTH) function can be used to select data for a specified number of months preceding the current month.

### Syntax

```javascript
SHOWBETWEENPERIOD(LASTNMONTH, number_of_months)
```

## Arguments

number\_of\_months – The number of months for which to fetch data. Required.

### Example

```
SHOWBETWEENPERIOD(LASTNMONTH, 5) #Displays data for the past 5 months
```

<figure><img src="../../.gitbook/assets/image (410).png" alt=""><figcaption><p>SHOWBETWEENPERIOD - LASTNMONTH</p></figcaption></figure>

### 6. SHOWBETWEENPERIOD(LASTNYEAR)

The SHOWBETWEENPERIOD(LASTNYEAR) function can be used to select data for a specified number of years preceding the current year.

### Syntax

```javascript
SHOWBETWEENPERIOD(LASTNYEAR, number_of_years)
```

## Arguments

number\_of\_years – The number of years for which to fetch data. Required.

### Example

```
SHOWBETWEENPERIOD(LASTNYEAR, 2) #Displays data for the past 2 years
```

<figure><img src="../../.gitbook/assets/image (412).png" alt=""><figcaption><p>SHOWBETWEENPERIOD - LASTNYEAR</p></figcaption></figure>

### 7. SHOWBETWEENPERIOD(NEXTNDAY)

The SHOWBETWEENPERIOD(NEXTNDAY) function can be used to select data for a specified number of days after the current day.

### Syntax

```javascript
SHOWBETWEENPERIOD(NEXTNDAY, number_of_days)
```

## Arguments

number\_of\_days – The number of days for which to fetch data. Required.

### Example

```
SHOWBETWEENPERIOD(NEXTNDAY, 8) #Displays data for 8 days from current date
```
