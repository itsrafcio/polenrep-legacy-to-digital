# Sprint 1 Review

Date: 2026-10-31

Configured sprint dates in Jira: 2026-10-15 to 2026-10-29.
Sprint status verified on 2026-11-01: closed.

The configured dates describe the sprint schedule in Jira, not the
dates of every prototype, review or administrative closure activity.

## Sprint Goal

Create a usable end-to-end flow for handling additional work
requests from subcontractor submission to communicating
the customer's final decision.

## Demonstrated Result

The sprint simulation covered the six core stories.

The PAD prototype demonstrates a smaller scope: an additional-work
record with a photo, subcontractor cost, customer-facing price,
decision statuses and automated decision emails.

Three notification checks passed: acceptance, rejection and
no decision email when returning to the pending status.

Tests used fictional data and a test recipient.

See the [case study](case_study.md) for the implementation
and test details, and the [backlog](backlog.md) for the original
story descriptions and Acceptance Criteria.

## Goal Assessment

The simulation is complete.

The PAD prototype does not demonstrate the full end-to-end
implementation described by the Sprint Goal.

PLD-10 includes further customer questions and therefore overlaps
with PLD-6–9. That part of its scope was not implemented in PAD.
Its simulated Done status does not demonstrate completion of
all its Acceptance Criteria.

## Backlog Decision

Prioritize PLD-6–9 together as the customer question-and-answer flow.
This would reduce manual handling of questions and responses
between the customer, PolenRep and the subcontractor.

Keep PLD-12, the 48-hour reminder, as a later enhancement.

The timing of the earlier-testing option approved in the change
scenario remains unresolved against this priority.
See [CR-01 in the change log](change_log.md).

No second sprint is being started as part of this exercise.
An empty, unstarted PLD Sprint 2 exists in Jira.
