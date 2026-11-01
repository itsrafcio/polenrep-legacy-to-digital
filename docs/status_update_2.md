# Sprint 1 Status Update #2

Date: 2026-10-31

## Overall Status

The PAD prototype is ready for Sprint Review. Its notification
function has been configured and tested.

## Progress

Since the previous update, PolenRep Approval Demo (PAD) has been
configured with a sample additional-work request, a photo, separate
subcontractor cost and customer-facing price, and decision statuses.
The request list can be filtered to show pending decisions.

An automation sends an email when a task's status changes to
Zaakceptowana (Accepted) or Odrzucona (Rejected).

The 48-hour reminder was approved in the change-control simulation
and added to the backlog as PLD-12. It remains unimplemented.

## Test Results

Tests used fictional data in PAD-1 and the project owner's email
address as the workshop's test inbox.

- Acceptance: an email arrived with the correct task key,
  summary and accepted status.
- Rejection: an email arrived with the correct task key,
  summary and rejected status.
- Pending decision: returning PAD-1 to Oczekuje na decyzję
  (Pending decision) did not send a decision email.

## Risks / Issues

No defects were observed in these three notification checks.
Customer decisions are recorded manually, and notifications go
to a fixed test inbox. Customer submission and routing to actual
workshops remain outside the tested scope.

## Forecast / Decisions

The prototype can be demonstrated at Sprint Review. A delivery date
for the complete digital process requires a separate scope and
scheduling decision.

## Next Steps

Review the demonstrated result against the Sprint Goal, record the
retrospective and complete the case study.

Keep PLD-6–9 and PLD-12 in the backlog.
