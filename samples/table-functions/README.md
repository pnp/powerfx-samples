# Table Utility Functions

## Summary

This is a `TableUtils` PowerApp Component containing Custom Functions that allow to manipulate PowerFx Table 

 
Short summary on functionality and used technologies.

> Please provide a high-quality screenshot of your web parts below. It should be stored in a folder called `assets`.
> If possible, use a resolution of 1920x1080.
> You can add as many screen shots as you'd like to help users understand your sample without having to download it and install it.
> DELETE THIS PARAGRAPH BEFORE SUBMITTING

![picture of the sample](assets/preview.png)

## Applies to

* [Microsoft Power Fx](https://docs.microsoft.com/en-us/power-platform/power-fx/overview)
* [Canvas App](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/)

## Compatibility

![Power Apps Source File Pack and Unpack Utility 0.20](https://img.shields.io/badge/PSAopa-0.20-green.svg)

## Solution

Solution|Author(s)
--------|---------
folder name | [bsorrentino](https://github.com/settings/profile) ([@bsorrentinoJ](https://twitter.com/bsorrentinoJ)), Company

## Version history

Version|Date|Comments
-------|----|--------
1.0|August 2, 2021|Initial release


## Prerequisites


## Minimal Path to Awesome

* [Download](solution\table-functions.msapp) the `.msapp` from the `solution` folder
* Use the `.msapp` file using **File** > **Open** > **Browse** within Power Apps Studio.

## Using the Source Code

  You can also use the [Power Apps Source Code tool](https://github.com/microsoft/PowerApps-Language-Tooling) to the code using these steps:
* Clone the repository to a local drive
* Pack the source files back into `.msapp` file:
  * [Power Apps Tooling Usage](https://github.com/microsoft/PowerApps-Language-Tooling)
* Use the `.msapp` file using **File** > **Open** > **Browse** in Power Apps Studio.

## Features

This sample includes following features:

* JsonToTable(Transform a JSON Object in an equivalent PowerFx Table)
 > This function could be very useful for detecting fields that have changed before submitting form

## Functions

### JsonToTable

Transform a JSON Object representing a single record in an equivalent PowerFx Table

#### Syntax

```
JsonToTable(json)
```

Parameter | Description | Required | Type
---|---|---|--
json | JSON Object representing a single record | Yes | Text


#### Output

Table - `[ { Name:Text, Value:Text },{ Name:Text, Value:Text }, ... ]`

#### Example

Considering the JSON below as input
```json
  {
    "bsc_field1": "value1",
    "bsc_field2": "value2",
    "bsc_field3": "value3"
  }
```

after call of `JsonToTable` it will be transformed in the following **PoweFx Table**

>  Name | Value 
> ---- | ---- 
> bsc_field1 | value1 
> bsc_field2 | value2 
> bsc_field3 | value3 
 

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

## Help

> Note: don't worry about this section, we'll update the links.

We do not support samples, but we this community is always willing to help, and we want to improve these samples. We use GitHub to track issues, which makes it easy for  community members to volunteer their time and help resolve issues.

If you encounter any issues while using this sample, [create a new issue](https://github.com/pnp/powerfx-samples/issues/new?assignees=&labels=Needs%3A+Triage+%3Amag%3A%2Ctype%3Abug-suspected&template=bug-report.yml&sample=YOUR-SOLUTION-NAME&authors=@YOURGITHUBUSERNAME&title=YOUR-SOLUTION-NAME%20-%20).

For questions regarding this sample, [create a new question](https://github.com/pnp/powerfx-samples/issues/new?assignees=&labels=Needs%3A+Triage+%3Amag%3A%2Ctype%3Abug-suspected&template=question.yml&sample=YOUR-SOLUTION-NAME&authors=@YOURGITHUBUSERNAME&title=YOUR-SOLUTION-NAME%20-%20).

Finally, if you have an idea for improvement, [make a suggestion](https://github.com/pnp/powerfx-samples/issues/new?assignees=&labels=Needs%3A+Triage+%3Amag%3A%2Ctype%3Abug-suspected&template=suggestion.yml&sample=YOUR-SOLUTION-NAME&authors=@YOURGITHUBUSERNAME&title=YOUR-SOLUTION-NAME%20-%20).

<img src="https://telemetry.sharepointpnp.com/powerfx-samples/samples/readme-template" />
