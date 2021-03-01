
# Regex User Defined Functions Library

## Summary
Functions that performs regex match on currency, percent & time formats
* [RegexUtils](https://github.com/GSiVed/customfunctions-samples/tree/main/samples/regex-functions#Regex-Utils)

The following image shows the custom function (component) properties and a sample implementation of RegexUtils when added to Power App:

<img src="assets/regexutilsfunc.PNG" width="30%" height="50%">

<img src="assets/regexiscurrencyfunc.PNG" width="60%" height="50%">

</br></br>


## Solution

Solution|Author(s)
--------|---------
RegexUtils  | Geetha Sivasaiam

## Version history

Version|Date|Comments
-------|----|--------
1.0|Mar 1, 2021|Initial Release


## Disclaimer
*THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON_INFRINGEMENT.*

---
## Minimal Path to Awesome

* Go to the solution folder and download the .MSAPP file
* Use the .msapp file using File > Open > Browse in Power Apps Studio.
  
## Using the Soure Code
  You can also use the Power Apps Source Code tool to unpack the code using these steps:
* Clone the repository to a local drive
* Pack the source files back into .msapp file:
  * [Power Apps Tooling Usage](https://github.com/microsoft/PowerApps-Language-Tooling)
* Use the .msapp file using File > Open > Browse in Power Apps Studio.

## RegexUtils Features
Functions that perform operations on a date value
* [IsCurrency](https://github.com/GSiVed/customfunctions-samples/tree/main/samples/regex-functions#IsCurrency)
* [IsPercent](https://github.com/GSiVed/customfunctions-samples/tree/main/samples/regex-functions#IsPercent)
* [IsTime](https://github.com/GSiVed/customfunctions-samples/tree/main/samples/regex-functions#IsTime)
</br></br>

## IsCurrency
Regex to validate currency format (US)
### Syntax
IsCurrency(CurrencyTxt)
* CurrencyTxt: Required
### Output
* Boolean
</br></br>


## IsPercent
Regex to validate percent format
### Syntax
IsPercent(PercentTxt)
* PercentTxt: Required
### Output
* Boolean
</br></br>


## IsTime
Regex to validate time format [hh:mm:ss]/[hr:min:sec]/[mm:ss]/[m:s]/[ss]/[s]
### Syntax
IsTime(TimeTxt)
* TimeTxt: Required
### Output
* Boolean
</br></br>
