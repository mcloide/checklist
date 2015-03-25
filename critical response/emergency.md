# Emergency Checklist

The emergency checklist has as it's goal to provide a list of actions and contacts that must be taken so, in case of an
emergency, the proper handling can be done.

## Definition of an emergency

An emergency is whenever Production cannot operate and by consequence the end user / client can't work.
Example:
* A code deployment was done and with it a syntax error, not detected by the developer or QA went to production.
 As result a core module of the application stopped working and blocked the rest of the application to function.

## Goal

Fix the issue in with the least amount of time possible so the damange caused by it can also be minimal.

## Checklist

1 - Create a task force to handle the issue (developers, qa, dev-ops, managers, product owner)
2 - Identify the issue
3 - Find the best solution for the issue:
3.1 - apply a path
3.2 - revert code
4 - Agree upon the solution
5 - Implement the solution
6 - Test the solution
7 - Deploy to production
8 - Communicate affected people / clients that the issue has been solved
9 - Do a post-mortum meeting to document all information from the issue and define effective ways to avoid it on the future
