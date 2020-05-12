# Assignment 5

## Middle Name
* Changed blank middle names to `n/a`

## Street Adress
* Cleaned up duplicate addresses
* Changed all homeless variations to `HOMELESS`
* Changed `Department of Corrections` and `Illinois Department of Corrections` to `IL Department of Corrections`
* Changed `HMLS` to `HOMELESS`
* Changed `Out of State` to `n/a`
* Replaced `TO BE DETERMINED` with `n/a`
* Used regex `(^[A-Z]{2}\b)` on Street Address to return state abbreviations for incarcerated individuals, and appended the states to the State column


## City
* Deleted space before `Kissimmee`
* Changed blanks to `n/a`
* Deleted `Washington` from city where State was `DC`

## State
* Changed blanks to `n/a`
* Changed `NB` to `NE`, where cities were in Nebraska
* Removed 1663 rows, where abbreviations under State were not state abbreviations, and there was no city or address to clarify

## Zipe Code
* Changed blanks to `n/a`
* Changed `0.0` to `n/a`
* Used `return value.strip(“.0”)` to remove `.0` added when converting column from number to string
* Used regex `(^\d{4}$)` to change zip codes with four digits to `n/a`
