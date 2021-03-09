
# Regex User Defined Functions Library

## Summary

Functions that performs regex match on currency, percent & time formats

* [RegexUtils](https://github.com/pnp/powerfx-samples/tree/main/samples/regex-functions#Regex-Utils)

The following image shows the custom function (component) properties and a sample implementation of RegexUtils when added to Power App:

![Regex Functions](assets/regexutilsfunc.PNG)

![Currency Functions](assets/regexiscurrencyfunc.PNG)

## Applies to

* Power Apps Canvas app

## Compatibility

![Power Apps Source File Pack and Unpack Utility 0.19](https://img.shields.io/badge/PSAopa-0.19-green.svg)

## Prerequisites

None


## Solution

Solution|Author(s)
--------|---------
RegexUtils  | [Geetha Sivasaiam](https://github.com/GSiVed)

## Version history

Version|Date|Comments
-------|----|--------
1.0|Mar 1, 2021|Initial Release


## Disclaimer

*THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON_INFRINGEMENT.*

---
## Minimal Path to Awesome

* [Download](solution/RegexFunctions.msapp) the `.msapp` from the `solution` folder
* Use the `.msapp` file using **File** > **Open** > **Browse** within Power Apps Studio.

> Include any additional steps as needed.
> DELETE THIS PARAGRAPH BEFORE SUBMITTING

## Using the Source Code

  You can also use the [Power Apps Source Code tool](https://github.com/microsoft/PowerApps-Language-Tooling) to the code using these steps:

* Clone the repository to a local drive
* Pack the source files back into `.msapp` file:
  * [Power Apps Tooling Usage](https://github.com/microsoft/PowerApps-Language-Tooling)
* Use the `.msapp` file using **File** > **Open** > **Browse** in Power Apps Studio.

## Functions 

Functions that perform operations on a date value

* [IsCurrency](#IsCurrency)
* [IsPercent](#IsPercent)
* [IsTime](#IsTime)

### IsCurrency

Regex to validate currency format (US)

#### Syntax

```excel
IsCurrency(CurrencyTxt)
```


Parameter | Description|Required | Type
---|---|---|---
`CurrencyTxt` | The text value to evaluate for a currency format|Yes | Text

#### Output

* Boolean



### IsPercent
Regex to validate percent format

#### Syntax

```excel
IsPercent(PercentTxt)
```

Parameter | Description|Required | Type
---|---|---|---
`PercentTxt` |The text value to evaluate for a percent format|Yes | Text



#### Output

* Boolean

### IsTime

Regex to validate time format [hh:mm:ss]/[hr:min:sec]/[mm:ss]/[m:s]/[ss]/[s]

#### Syntax

```excel
IsTime(TimeTxt)
```

Parameter | Description|Required | Type
---|---|---|---
`TimeTxt` |The text value to evaluate for a time format|Yes | Text

#### Output

* Boolean

<img src="https://telemetry.sharepointpnp.com/powerfx-samples/samples/regex-functions" />
