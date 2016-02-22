# Critical issue Checklist

The critical issue checklist has as it's goal to provide a list of actions and contacts that must be taken so, in case of
an issue that is critical, can be taken with proper timinig and handling.

## Definition of a critical issue

It is important to understand that a critical issue is not an emergency. A critical issue can block a part of the application
but it doesn't mean that the whole application came to a halt. Without a clear definition of what is critical, every issue
will become critical in a business perspective.

In summary a critical issue is a issue that:
*  blocks the functionality of a module or part of the application
*  prevents the client of being able to function entirely or to process transactions
*  can result in profit or sensitive data loss (sensitive as important data to business and not credit card information)

Example:
* A new promotion to give out 10% discount on a e-commerce site was rolled out but, when applied, the
promotion doesn't provide the expected 10% discount and that generated a large amount of carts being dropped and
a large amount of calls received by customer support informing that the discount is not working.

## Goal

Identify and fix the issue in the least amount of time possible.

## Checklist

* 1 - Identify the issue
* 2 - Create a small task force to handle the issue (developers, qa, dev-ops and maybe managers)
* 3 - Find the best solution for the issue
* 4 - Agree upon the solution
* 5 - Determine when the solution can be safely applied to production
* 6 - Test the solution
* 7 - Apply the solution to:
 * 7.1 - next build
 * 7.2 - hot fix (treat as emergency)
* 8 - Communicate affected people / clients that the issue has been solved
* 9 - Do a post-mortum meeting to document all information from the issue and define effective ways to avoid it on the future
 
### Checklist items

1 - Identify

The source of the issue needs to be identified to properly create the response team. For example if a server is not functional the task force should be mainly focused on operations team, while if the issue is software related the task force should be focused to the development team.

The identification of the issue will also help determine how critical it is to be applied as hot fix or not.

2 - Create a small task for to handle the issue:

It is important that we define the persons and roles that are required on the task force to properly solve the issue. The list bellow shows a task force for a software development issue.

* who will be the software engineer responsible to troubleshoot the issue and provide the fix
* who will be the quality engineer responsible to test the fix provided
* who will be responsible to deploy the fix to production
* who will be the communication endpoint for the client about the status of the issue

3 - Find the best solution for the issue

This might be as simple as doing a change on the database that would make the client to function for a period of time until a proper fix is done or a more elaborated fix that requires software development, testing, etc.

4 - Agree on the solution

Once the solution is defined all roles of the task force must be in conformity that the solution to be applied will suffice to solve the issue. If there is no agreement there is no reasonable way to correctly determine that the patch will work.

5 - Determine when the solution can be safely applied to production

It all depends on the client. If the cient is a retail store and you are applying a patch that will interrupt it services during a period of time that will also reflect in loss of money from the client side therefore the patch should be applied after hours.

6 - Test the solution

Every patch should be throughly tested even if it requires regression testing. Obviously integration tools that runs unit tests helps on cases like these but if that is not available for your application the quality engineer responsible on the task force should define
what will be needed as tests to safely apply the patch in production.

7 - Apply the solution to either next release or as a hotfix

This is not simple but it goes back to step 1. Is the issue critical enough that it will require a hot fix or is it something that can be done in the next release.

8 - Communication

It is important to communicate to all parties involved that a fix has been done and when it will be deployed. This will help dimishing expectations from all parties involved.

9 - Post Mortum

A meeting is required to document the issue and all steps required to fix and what are the next steps required to apply the fix in the existing codebase, etc. The concept of the meeting is that issues like these can be avoided completely in next releases.
