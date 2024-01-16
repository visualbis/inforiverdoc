# SHOWCLOSEDFORECAST

With Inforiver, you can create  forecasts using manually entered values, data from previous periods or apply formulae to generate the forecast. The forecast is generated for previous periods as well. For example, if you are creating a forecast for 2024 based on data from 2023, the forecast measure will be created even for the 2023 columns. You can choose to show or hide the forecast columns for previous periods using the SHOWCLOSEDFORECAST function.

### Syntax

```javascript
SHOWCLOSEDFORECAST(BOOLEAN_ARG)
```

### Arguments

BOOLEAN\_ARG - Set to TRUE to show forecasts for closed periods. Set to FALSE to hide forecasts for closed periods.

### Example

```
SHOWCLOSEDFORECAST(TRUE) #Displays the forecast measure for previous periods
SHOWCLOSEDFORECAST(FALSE) #Hides the forecast measure for previous periods
SHOWCLOSEDFORECAST(THIS) #Use with a toggle variable to show or hide forecasts for closed periods
```

