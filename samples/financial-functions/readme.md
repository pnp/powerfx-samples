# Financial Functions
functions that are used by accounting & finance
* [FV](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#FV)
* [PV](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#PV)
* [NPER](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#NPER)
* [PMT](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#PMT)
</br></br>



## FV
future value: a cash balance you want to attain after the last payment is made.
### Syntax
PV(Rate, NPER, PMT [, PV])
* Rate: Required
* NPER: Required
* PMT: Required
* PV: Optional
</br></br>


## PV
present value: the total amount that a series of future payments is worth now
### Syntax
PV(Rate, NPER, PMT [, FV])
* Rate: Required
* NPER: Required
* PMT: Required
* FV: Optional
</br></br>


## NPER
the total number of payments for a loan
### Syntax
NPER(Rate, PMT, PV [, FV])
* Rate: Required
* PMT: Required
* PV: Required
* FV: Optional
</br></br>


## PMT
the payment made each period over the life of an investment.
### Syntax
PV(Rate, NPER, PV [, FV])
* Rate: Required
* NPER: Required
* PV: Required
* FV: Optional
</br></br>
