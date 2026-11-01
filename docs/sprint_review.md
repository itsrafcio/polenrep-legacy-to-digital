# Sprint 1 Review

Date: 2026-10-31  
Configured sprint dates in Jira: 2026-10-15 to 2026-10-29.  
Sprint status verified on 2026-11-01: closed.

## Sprint Goal

Create a usable end-to-end flow for handling additional work
requests from subcontractor submission to communicating
the customer's final decision.

## Demonstrated Result

The simulated sprint covered six core stories. The working PAD
prototype covers recording additional-work information and sending
a notification after the PM manually records a customer decision.

Three notification checks passed: acceptance, rejection and no decision
email when returning to the pending status. Tests used fictional data
and a test inbox representing the workshop.

See the [case study](case_study.md) for screenshots and test details,
and the [backlog](backlog.md) for the stories and acceptance criteria.

## Goal Assessment

The final notification step was demonstrated. The full end-to-end
Sprint Goal was not achieved by the working prototype: customer
submission, automatic decision capture, the question-and-answer flow
and routing to actual workshops remain outside its implemented scope.

## Backlog Decision

Consider PLD-6–9 together as the next functional area covering questions
and responses between the customer, PolenRep and the workshop.
Resolve their overlap with the question-handling requirement in PLD-10
before planning implementation.

Keep PLD-12, the 48-hour reminder, as a later enhancement.
Its change-control scenario is recorded in [CR-01](change_log.md).

Further implementation requires a scope and scheduling decision.
