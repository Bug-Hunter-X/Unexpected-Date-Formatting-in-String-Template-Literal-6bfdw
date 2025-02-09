# Unexpected Date Formatting in String Template Literal

This repository demonstrates a common but subtle bug in TypeScript related to string template literals and Date objects. The problem arises from how the Date object is implicitly converted to a string within a template literal. The default string representation of a Date object might not always match the desired format.

The `bug.ts` file contains the erroneous code, while `bugSolution.ts` provides a corrected version.

## Bug
The `greet` function takes a person's name and a Date object as input and returns a greeting string. However, the default string representation of the Date object in the template literal might lead to an unexpected output format.

## Solution
The solution involves explicitly formatting the Date object using `toLocaleDateString()` or similar methods to ensure consistent and expected output.