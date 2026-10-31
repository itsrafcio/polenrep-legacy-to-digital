# Sprint 1 Status Update #2

Date: 2026-10-31

## Overall Status

The training project is ready for Sprint Review.

A working Jira prototype has been configured and tested.
The complete end-to-end process described in the PLD stories
has not been implemented in PAD.

## Progress

Since the previous update, PolenRep Approval Demo (PAD) has
been configured with a sample additional-work request, a photo,
separate subcontractor cost and customer-facing price,
decision statuses, and a filtered list of pending decisions.

An automation now sends an email when the status changes
to Zaakceptowana or Odrzucona.

The 48-hour customer reminder was approved in the training
scenario and added to the backlog as PLD-12. It has not been
implemented.

## Test Results

Tests used fictional data in PAD-1 and the project owner's
email address as the subcontractor's test inbox.

- Acceptance: an email arrived with the correct issue key,
  summary and accepted status.
- Rejection: an email arrived with the correct issue key,
  summary and rejected status.
- Pending decision: returning PAD-1 to Oczekuje na decyzję
  did not send a decision email.

## Risks / Issues

No defects were observed in these three notification checks.

Customer decisions were entered manually. Customer submission
and notification routing to actual subcontractors were not
tested. These results do not confirm all acceptance criteria
of the six Sprint 1 stories.

## Forecast / Decisions

The tested PAD prototype can be demonstrated at Sprint Review.

A delivery date for the complete digital process cannot yet
be confirmed from this prototype. Further implementation
requires a separate scope and scheduling decision.

## Next Steps

Review the demonstrated result against the Sprint Goal,
record the retrospective, and document the actual implementation
and its limitations in the case study.

Keep PLD-6–9 and PLD-12 in the backlog.