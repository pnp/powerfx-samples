# Date Functions
Functions that perform operations on a date value
* [EndOfQuarter](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#EndOfQuarter)
* [EndOfMonth](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#EndOfMonth)
* [EndOfWeek](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#EndOfWeek)
* [EndOfYear](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#EndOfYear)
* [IsBetweenDates](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsBetweenDates)
* [IsLeapYear](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsLeapYear)
* [IsInCurrentDay](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsInCurrentDay)
* [IsInCurrentMonth](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsInCurrentMonth)
* [IsInCurrentQuarter](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsInCurrentQuarter)
* [IsInCurrentWeek](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsInCurrentWeek)
* [IsInCurrentYear](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsInCurrentYear)
* [IsInNextNDays](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsInNextNDays)
* [IsInNextNMonths](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsInNextNMonths)
* [IsInNextNQuarters](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsInNextNQuarters)
* [IsInNextNWeeks](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsInNextNWeeks)
* [IsInNextNYears](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsInNextNYears)
* [IsInPreviousNDays](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsInPreviousNDays)
* [IsInPreviousNMonths](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsInPreviousNMonths)
* [IsInPreviousNQuarters](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsInPreviousNQuarters)
* [IsInPreviousNWeeks](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsInPreviousNWeeks)
* [IsInPreviousNYears](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#IsInPreviousNYears)
* [NetWorkDays](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#NetWorkDays)
* [StartOfQuarter](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#StartOfQuarter)
* [StartOfMonth](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#StartOfMonth)
* [StartOfWeek](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#StartOfWeek)
* [StartOfYear](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#StartOfYear)
* [WeekOfMonth](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#WeekOfMonth)
* [WeekOfYear](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#WeekOfYear)
* [YearFraction](https://github.com/yourekittenme/powerapps-custom-functions/tree/main/custom_functions_devaney#YearFraction)
</br></br>

## EndOfQuarter
Get the last day of a quarter.
### Syntax
StartOfQuarter(StartDate [, AddQuarters])
* StartDate: Required
* AddQuarters: Optional
</br></br>


## EndOfMonth
Get the last day of a month.
### Syntax
EndOfMonth(StartDate [, AddMonths])
* StartDate: Required
* AddMonths: Optional
</br></br>


## EndOfWeek
Get the last day of a week.
### Syntax
EndOfWeek(StartDate [, AddWeeks, DayWeekStart])
* StartDate: Required
* AddWeeks: Optional
* DayWeekStart: Optional
</br></br>


## EndOfYear
Get the last day of a year.
### Syntax
EndOfYear(StartDate [, AddYears])
* StartDate: Required
* AddYears: Optional
</br></br>


## IsBetweenDates
Checks if a date is within a specified date range 
### Syntax
IsBetweenDates(EvaluateDate, StartDate, EndDate)
* EvaluateDate: Required
* StartDate: Required
* EndDate: Required
</br></br>


## IsLeapYear
Checks if a date belongs to a leap year.
### Syntax
IsLeapYear(EvaluateDate)
* EvaluateDate: Required
</br></br>


## IsInCurrentDay
Checks if a date occurs within the current day
### Syntax
IsInCurrentDay(EvaluateDate)
* EvaluateDate: Required
</br></br>


## IsInCurrentMonth
Checks if a date occurs within the current month
### Syntax
IsInCurrentMonth(EvaluateDate)
* EvaluateDate: Required
</br></br>


## IsInCurrentQuarter
Checks if a date occurs within the current quarter
### Syntax
IsInCurrentQuarter(EvaluateDate)
* EvaluateDate: Required
</br></br>


## IsInCurrentWeek
Checks if a date occurs within the current week
### Syntax
IsInCurrentWeek(EvaluateDate, DayWeekStart)
* EvaluateDate: Required
</br></br>


## IsInCurrentYear
Checks if a date occurs within the current year
### Syntax
IsInCurrentYear(EvaluateDate)
* EvaluateDate: Required
</br></br>


## IsInNextNDays
Checks if a date occurs within the next number of days. Start date defaults to the current date.
### Syntax
IsInNextNDays(EvaluateDate, NumberOfDays [, StartDate])
* EvaluateDate: Required
* NumberOfDays: Required
* StartDate: Optional
</br></br>


## IsInNextNMonths
Checks if a date occurs within the next number of months. Start date defaults to the current date.
### Syntax
IsInNextNMonths(EvaluateDate, NumberOfMonths [, StartDate])
* EvaluateDate: Required
* NumberOfMonths: Required
* StartDate: Optional
</br></br>


## IsInNextNQuarters
Checks if a date occurs within the next number of quarters. Start date defaults to the current date.
### Syntax
IsInNextNQuarters(EvaluateDate, NumberOfQuarters [, StartDate])
* EvaluateDate: Required
* NumberOfQuarters: Required
* StartDate: Optional
</br></br>


## IsInNextNWeeks
Checks if a date occurs within the next number of weeks. Start date defaults to the current date.
### Syntax
IsInNextNWeeks(EvaluateDate, NumberOfWeeks [, StartDate])
* EvaluateDate: Required
* NumberOfWeeks: Required
* StartDate: Optional
</br></br>


## IsInNextNYears
Checks if a date occurs within the next number of years. Start date defaults to the current date.
### Syntax
IsInNextNYears(EvaluateDate, NumberOfYears [, StartDate])
* EvaluateDate: Required
* NumberOfYears: Required
* StartDate: Optional
</br></br>


## IsInPreviousNDays
Checks if a date occurs within the previous number of days. Start date defaults to the current date.
### Syntax
IsInPreviousNDays(EvaluateDate, NumberOfDays [, StartDate])
* EvaluateDate: Required
* NumberOfDays: Required
* StartDate: Optional
</br></br>


## IsInPreviousNMonths
Checks if a date occurs within the previous number of months. Start date defaults to the current date.
### Syntax
IsInPreviousNMonths(EvaluateDate, NumberOfMonths [, StartDate])
* EvaluateDate: Required
* NumberOfMonths: Required
* StartDate: Optional
</br></br>


## IsInPreviousNQuarters
Checks if a date occurs within the previous number of quarters. Start date defaults to the current date.
### Syntax
IsInPreviousNQuarters(EvaluateDate, NumberOfQuarters [, StartDate])
* EvaluateDate: Required
* NumberOfQuarters: Required
* StartDate: Optional
</br></br>


## IsInPreviousNWeeks
Checks if a date occurs within the previous number of weeks. Start date defaults to the current date.
### Syntax
IsInPreviousNWeeks(EvaluateDate, NumberOfWeeks [, StartDate])
* EvaluateDate: Required
* NumberOfWeeks: Required
* StartDate: Optional
</br></br>


## IsInPreviousNYears
Checks if a date occurs within the previous number of years. Start date defaults to the current date.
### Syntax
IsInPreviousNYears(EvaluateDate, NumberOfYears [, StartDate])
* EvaluateDate: Required
* NumberOfYears: Required
* StartDate: Optional
</br></br>


## NetWorkDays
Find the number of work days between two dates.
### Syntax
NetWorkDays(StartDate, EndDate)
* StartDate: Required
* EndDate: Required
</br></br>


## StartOfMonth
Get the first day of a month.
### Syntax
StartOfMonth(StartDate [, AddMonths])
* StartDate: Required
* AddMonths: Optional
</br></br>


## StartOfQuarter
Get the first day of a quarter.
### Syntax
StartOfQuarter(StartDate [, AddQuarters])
* StartDate: Required
* AddQuarters: Optional
</br></br>


## StartOfWeek
Get the first day of a week.
### Syntax
StartOfWeek(StartDate [, AddWeeks, DayWeekStart])
* StartDate: Required
* AddWeeks: Optional
* DayWeekStart: Optional
</br></br>


## StartOfYear
Get the first day of a year.
### Syntax
StartOfYear(StartDate [, AddYears])
* StartDate: Required
* AddYears: Optional
</br></br>

## WeekOfMonth
Takes a date and returns a week number (1-6) that corresponds to the week of the month.
### Syntax
WeekNumber(StartDate [,DayWeekStart])
* StartDate: Required
* DayWeekStart: Optional
</br></br>

## WeekOfYear
Takes a date and returns a week number (1-54) that corresponds to the week of the year.
### Syntax
WeekNumber(StartDate [,DayWeekStart])
* StartDate: Required
* DayWeekStart: Optional
</br></br>


## YearFraction
Calculates a decimal number representing the fraction of a year between two dates.
### Syntax
YearFraction(StartDate, EndDate [,Basis])
* StartDate: Required
* EndDate: Required
* Basis: Optional
