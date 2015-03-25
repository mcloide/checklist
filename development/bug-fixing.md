# Bug fixing checklist

Software isn't perfect and therefore bugs will exist. Bug fixing relies a lot on identifying and troubleshooting. The
bug fixing checklist goes into a simplified troubleshooting guide so a bug can fixed with less hassle and more quality.

## Defining a bug
A bug is a flaw on the system as it is not generating the defined expected result. A bug is not a miss-interpretation of
a feature / functionality.

Example:
* When entering values on the form the input field for amount is accepting non numeric characters and that is being allowed
to be saved on the database. In this scenario we have 2 distinct issues:
** The form accepts non numeric values for amount to be entered
** The application accepts non numeric values for amount to saved

## Goal
Identify and correct the bug ensuring that it wont happen again.

## Checklist
(developer perspective)

1 - create a well defined and explained documentation explaining the bug and the expected behavior proving images
and screencast if possible
2 - using the revision or the latest revision on your development environment try to replicate the bug
3 - using logs and debug tools track what piece(s) of code is responsible for generating the bug
4 - determine what is best solution to correct the issue
5 - apply correction
6 - re-test the issue with the correction applied on development machine
7 - verify if unit tests must be run / updated
8 - document the solution applied
9 - assign to QA for further testing.