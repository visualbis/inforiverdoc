# RELATIVE

Provide reference to previous or next values in a column (This will work with all operators +,- ,/ ,\*) **Limitation:** This will not work correctly if reorder columns are used, it will still use the same column reference from the initial dataset. it is mainly designed to work for visual measure.

## Example

IFNA((Sales.RELATIVE(-1) - Sales.RELATIVE), Sales.RELATIVE)

When Months in the columns, formula returns Sales of Previous month - Current Month Sales, i.e. - Variance except when there is an error, then it returns the Sales of Current Month.
