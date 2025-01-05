# CSS `calc()` Errors
This repository demonstrates common errors related to the `calc()` function in CSS and how to fix them.

## Bug 1: Missing Spaces in `calc()`
Incorrect use: `width:calc(100%-10px);`
Correct use: `width:calc(100% - 10px);`

## Bug 2: Inconsistent Units in `calc()`
Avoid mixing units without conversion. For example:
Incorrect: `height:calc(50% + 20px);` (Better to convert px to % or vice versa)
Correct (converting to %): `height:calc(50% + 200% / 10);` (If `10` is the base size)