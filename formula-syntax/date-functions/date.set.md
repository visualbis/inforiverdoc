# DATE.SET()

The DATE.SET() function can be used to change the format of a date. Refer to [Microsoft's date format codes ](https://learn.microsoft.com/en-us/system-center/orchestrator/standard-activities/format-date-time?view=sc-orch-2022)to view all the supported format models. The input date should be in MM/DD/YYYY format.

## Syntax

```javascript
date.set(date, format_model)
```

## Arguments

date - The date which is passed as input to the function.&#x20;

format\_model - The new date format to be applied to the input date

## Return value

Date

## Example

```javascript
DATE.SET('03/01/2023', 'YYYYMMDD')
```

Returns 20230301.

<figure><img src="../../.gitbook/assets/image (224).png" alt=""><figcaption><p>DATE.SET function</p></figcaption></figure>
