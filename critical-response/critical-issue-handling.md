# Critical issue Checklist

The critical issue checklist has as it's goal to provide a list of actions and contacts that must be taken so, in case of
an issue that is critical, can be taken with proper timinig and handling.

## Definition of a critical issue

It is important to understand that a critical issue is not an emergency. A critical issue can block a part of the application
but it doesn't mean that the whole application came to a halt. Without a clear definition of what is critical, every issue
will become critical in a business perspective.

In summary a critical issue is a issue that:
*  blocks the functionality of a module or part of the application
*  can result in profit or sensitive data loss (sensitive as important data to business and not credit card information)

Example:
* A new promotion to give out 10% discount on a e-commerce site was rolled out but, when applied, the
promotion doesn't provide the expected 10% discount and that generated a large amount of carts being dropped and
a large amount of calls received by customer support informing that the discount is not working.

## Goal

Identify and fix the issue in the least amount of time possible.

## Checklist

* 1 - Create a small task force to handle the issue (developers, qa, dev-ops and maybe managers)
* 2 - Identify the issue
* 3 - Find the best solution for the issue
* 4 - Agree upon the solution
* 5 - Determine when the solution can be safely applied to production
* 6 - Test the solution
* 7 - Apply the solution to:
 * 7.1 - next build
 * 7.2 - hot fix (treat as emergency)
* 8 - Communicate affected people / clients that the issue has been solved
* 9 - Do a post-mortum meeting to document all information from the issue and define effective ways to avoid it on the future
