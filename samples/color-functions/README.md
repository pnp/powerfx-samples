
# Color Functions

## Summary

Functions that calculate the contrast between two colors. 

* [Color Functions](https://github.com/pnp/powerfx-samples/tree/main/samples/color-functions)

The following image shows a sample implementation of Color Functions component to create a color contrast cshecker when added to Power App:

![Contrast Checker](assets/ContrastChecker.PNG)

## Applies to

* Power Apps Canvas app

## Compatibility

![Power Apps Source File Pack and Unpack Utility 0.20](https://img.shields.io/badge/PSAopa-0.20-green.svg)

## Prerequisites

None


## Solution

Solution|Author(s)
--------|---------
Color Functions  | [P3N](https://github.com/P3N-101)

## Version history

Version|Date|Comments
-------|----|--------
1.0|May 8, 2021|Initial Release


## Disclaimer

*THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON_INFRINGEMENT.*

---
## Minimal Path to Awesome

* [Download](https://github.com/pnp/powerfx-samples/raw/main/samples/color-functions/solution/color-functions.msapp) the `.msapp` from the `solution` folder
* Use the `.msapp` file using **File** > **Open** > **Browse** within Power Apps Studio.

## Using the Source Code

  You can also use the [Power Apps Source Code tool](https://github.com/microsoft/PowerApps-Language-Tooling) to the code using these steps:

* Clone the repository to a local drive
* Pack the source files back into `.msapp` file:
  * [Power Apps Tooling Usage](https://github.com/microsoft/PowerApps-Language-Tooling)
* Use the `.msapp` file using **File** > **Open** > **Browse** in Power Apps Studio.

## Functions 

Functions that perform operations on colors

* [sRGBtoLIn](#sRGBtoLIn)
* [getLuminance](#getLuminance)
* [chkContrast](#IsCurrency)

### sRGBtoLIn

Linerizes an R G or B value,using the following formula:

```Excel
If(
    Sum(colorChannel / 255) <= 0.03928,
    Sum(colorChannel / 255) / 12.92,
    Power(
        ((Sum(colorChannel / 255) + 0.055) / 1.055),
        2.4
    )
)
```

#### Syntax

```excel
sRGB(colorChannel)
```

Parameter | Description|Required | Type
---|---|---|---
`colorChannel` | Linerizes an R G or B value |Yes | Number

#### Output

* Number

### getLuminance

Calclulates the relative luminance of linerized RGB colors using the following formula:

```excel
Sum(
    ('color-functions'.sRGBtoLIN(R) * 0.2126) + 
    ('color-functions'.sRGBtoLIN(G) * 0.7152) + 
    ('color-functions'.sRGBtoLIN(B) * 0.0722)
)
```

#### Syntax

```excel
getLuminance(R,G,B)
```

Parameter | Description|Required | Type
---|---|---|---
`R` | Linerized R Value |Yes | Number
`G` | Linerized G Value |Yes | Number
`B` | Linerized B Value |Yes | Number

#### Output

* Number between 0 and 1

### chkContrast

Calclulates the contrast between two colors using the following formula:

```excel
If(
    // Check which Value is higher, calculation then is (darkColor+0.05) / (lightColor+0.05)
    LightColor >DarkColor,
    Text(
        Sum((LightColor + 0.05) / (DarkColor + 0.05)),
        "[$-en-GB]#.000"
    ),
    Text(
        Sum((DarkColor + 0.05) / (LightColor + 0.05)),
        "[$-en-GB]#.000"
    )
)
```

#### Syntax

```excel
chkContrast(DarkColor,LightColor)
```

Parameter | Description|Required | Type
---|---|---|---
`DarkColor` | Dark color relative luminance |Yes | Number
`LightCOlor` | Light color relative luminance |Yes | Number

#### Output

* Number between 1 and 21

<img src="https://telemetry.sharepointpnp.com/powerfx-samples/samples/color-functions" />
