# PolenRep Legacy-to-Digital

A portfolio project based on the additional-work approval process
I manage at PolenRep, coordinating vehicle repair and restoration
projects for international customers.

The process already works through email, WhatsApp and phone calls.
This project explores how to reduce manual follow-up and information
transfer while preserving the existing approval logic.

**Start with the [case study](docs/case_study.md)** for the business
problem, approach, screenshots and tested result.

## What This Project Demonstrates

- Translating an existing business process into an Epic, 11 user
  stories with acceptance criteria, a Sprint Goal and Definition of Done.
- Practising delivery decisions through a simulated sprint, a RAID log,
  a change request, two status updates, a Sprint Review and a retrospective.
- Configuring a Jira prototype and testing automated decision emails
  against three scenarios.

## Project Scope

**PLD — PolenRep Legacy to Digital** contains the requirements and
one simulated Scrum sprint. Its story statuses represent progress
through the simulation.

**PAD — PolenRep Approval Demo** is a working Jira prototype of the
final communication step: the project manager manually records the
customer's decision, and an automation emails a test inbox representing
the workshop.

The prototype covers this final handoff, not the full process described
by the PLD stories. Customer submission, automatic decision capture,
the question-and-answer loop and routing to actual workshops remain
outside the implemented scope.

## Working Result

PAD-1 contains a fictional additional-work request with vehicle and
customer information, a photo, separate subcontractor cost and
customer-facing price, and schedule impact.

Changing its status to accepted or rejected sends an email containing
the task key, summary and status. Three checks were completed:

- Accepted — the expected email arrived.
- Rejected — the expected email arrived.
- Pending decision — no decision email was received.

## My Contribution

I documented the existing process, defined the requirements and backlog,
prepared the delivery artefacts, configured the Jira prototype and
performed its notification tests. The business process comes from my
own work at PolenRep; the prototype uses fictional request data.

## Project Documentation

- [Project brief](docs/project_brief.md) — scope, stakeholders and Definition of Done
- [AS-IS process](docs/as_is_process.md) — the existing approval process
- [Product backlog](docs/backlog.md) — original Jira stories, acceptance criteria and sprint scope
- [RAID log](docs/raid_log.md) — assumptions, risks, issues and dependencies
- [Change log](docs/change_log.md) — the 48-hour reminder change-control scenario
- [Status update 1](docs/status_update_1.md) — sprint simulation progress
- [Status update 2](docs/status_update_2.md) — prototype results and remaining scope
- [Sprint Review](docs/sprint_review.md) — demonstrated result against the Sprint Goal
- [Retrospective](docs/sprint_retrospective.md) — lessons and improvements
- [API troubleshooting notes](docs/api_troubleshooting_notes.md) — a checklist from separate API exercises

## Remaining Backlog

PLD-6–9 cover the customer question-and-answer flow and are the next
functional area to consider together. PLD-12 covers a reminder after
48 hours without a customer response and remains a later enhancement.

## Tools

Jira Cloud, Jira Automation, Git and GitHub.
