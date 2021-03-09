# Financial Functions
functions that are used by accounting & finance

![Preview](assets/preview.png)

* [FV](#FV)
* [PV](#PV)
* [NPER](#NPER)
* [PMT](#PMT)

## Applies to

* [Microsoft Power Fx](https://docs.microsoft.com/en-us/power-platform/power-fx/overview)

## Prerequisites

None

## Solution

Solution|Author(s)
--------|---------
date-functions | [Matthew Devaney](https://github.com/matthewdevaney) ([@mattbdevaney](https://twitter.com/mattbdevaney))

## Version history

Version|Date|Comments
-------|----|--------
1.0|February 8, 2021|Initial release

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

---

## Minimal Path to Awesome

* [Download](solution/powerfx-financial-functions.msapp) the `.msapp` from the `solution` folder
* Use the `.msapp` file using **File** > **Open** > **Browse** within Power Apps Studio.


## Using the Source Code

  You can also use the [Power Apps Source Code tool](https://github.com/microsoft/PowerApps-Language-Tooling) to the code using these steps:
* Clone the repository to a local drive
* Pack the source files back into `.msapp` file:
  * [Power Apps Tooling Usage](https://github.com/microsoft/PowerApps-Language-Tooling)
* Use the `.msapp` file using **File** > **Open** > **Browse** in Power Apps Studio.

## Functions

### FV

Future value: a cash balance you want to attain after the last payment is made.

#### Syntax

```excel
FV(Rate, NPER, PMT [, PV])
```

Parameter | Description | Required | Type
---|---|---|---
`Rate`|The numeric value indicating the rate per period| Yes | Number
`NPER`|The numeric value indicating the total number of payments periods in an annuity.| Yes | Number
`PMT`|The numeric value indicating the amount of the payment made each period| Yes | Number
`PV`|The numeric value indicating the present value of the payments. If omitted, it will be set the default value as 0| No | Number

#### Output

Number


### PV

Present value: the total amount that a series of future payments is worth now

#### Syntax

```excel
PV(Rate, NPER, PMT [, FV])
```

Parameter | Description | Required | Type
---|---|---|---
`Rate`|The numeric value indicating the rate per period| Yes | Number
`NPER`|The numeric value indicating the total number of payments periods in an annuity.| Yes | Number
`PMT`|The numeric value indicating the amount of the payment made each period| Yes | Number
`FV`|The numeric value indicating the  future value or a cash balance you want to attain after the last payment is made. If omitted, it is assumed to be 0. | No | Number

#### Output

Number


### NPER

The total number of payments for a loan

#### Syntax

```excel
NPER(Rate, PMT, PV [, FV])
```

Parameter | Description | Required | Type
---|---|---|---
`Rate`|The numeric value indicating the interest rate per period| Yes | Number
`PMT`|The numeric value indicating the amount of the payment made each period| Yes | Number
`PV`|The numeric value indicating the present value of the payments. | Yes | Number
`FV`|The numeric value indicating the value of the loan/investment at the end of the payments. If  omitted, it will be set the default value as 0 | No | Number

#### Output

Number



### PMT

The payment made each period over the life of an investment.

### Syntax

```excel
PV(Rate, NPER, PV [, FV])
```

Parameter | Description | Required | Type
---|---|---|---
`Rate`|The numeric value indicating the interest rate per period| Yes | Number
`NPER`|The numeric value indicating the total number of payments for the loan.| Yes | Number
`PV`|The numeric value indicating the present value of the payments. | Yes | Number
`FV`|The numeric value indicating the future value or a cash balance to attain after last payment is made. If omitted, it is assumed to be 0 | No | Number

#### Output

Number

<img src="https://telemetry.sharepointpnp.com/powerfx-samples/samples/financial-functions" />
