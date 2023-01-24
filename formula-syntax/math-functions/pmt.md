# PMT

The PMT function calculates the payment for a loan based on constant payments and a constant interest rate.

## Syntax

```javascript
pmt(rate:number, nper:number, pv:number, fv:number, type:number)
```

## Arguments

rate – Required. The interest rate per period.

nper – Required. The total number of periods.

pv – Required. The present value or initial investment. Cash outflows are considered negative and cash inflows as positive.

fv – The future or residual value. This is an optional argument and if omitted, it is considered to be zero.

type – Indicates when the payments are made. The type is zero if payments are made at the end of the period and non-zero if payments are made at the start of the period. This is an optional argument and when omitted, it is considered to be zero.

## Example

```javascript
pmt(0,1,10,1000,0,0)
```

Returns 100.0000000000001

## Excel equivalent

[PMT](https://support.microsoft.com/en-us/office/pmt-function-0214da64-9a63-4996-bc20-214433fa6441)
