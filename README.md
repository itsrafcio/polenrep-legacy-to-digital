# PolenRep Legacy-to-Digital

A portfolio project based on a real PolenRep process: obtaining
customer approval for additional vehicle repair work.

The existing process uses email, WhatsApp and phone calls.
The project explores how to structure requests, decisions and
communication while reducing repetitive manual work.

## Project Scope

The project combines two parts:

- **PLD — PolenRep Legacy to Digital:** requirements analysis,
  user stories with acceptance criteria and one simulated Scrum
  sprint covering the additional-work approval process.
- **PAD — PolenRep Approval Demo:** a working Jira prototype
  demonstrating manual recording of a customer's decision and
  automated notification to a test inbox representing the workshop.

Completing stories in the PLD simulation does not mean that their
functionality was implemented in PAD.

## Working Prototype and Tests

PAD contains a sample additional-work request with fictional vehicle
and customer information, photo evidence, subcontractor cost,
customer-facing price and schedule impact.

The project manager records the customer's decision by changing
the request's status. Jira Automation sends an email when the status
becomes accepted or rejected. The message includes the task key,
summary and status.

Three notification scenarios were checked:

- Accepted — the expected email arrived.
- Rejected — the expected email arrived.
- Pending decision — no decision email was received.

The prototype does not implement the complete end-to-end process.
Customer-facing submission, automatic capture of the customer's
response, the question-and-answer loop and notification routing
to actual workshops were not implemented or tested.

## Project Documentation

Start with the [case study](docs/case_study.md) for the business
context, approach, tested result and limitations.

- [Project brief](docs/project_brief.md) — scope, stakeholders and Definition of Done
- [AS-IS process](docs/as_is_process.md) — the existing approval process
- [Product backlog](docs/backlog.md) — original Jira stories, acceptance criteria and sprint scope
- [RAID log](docs/raid_log.md) — assumptions, risks, issues and dependencies
- [Change log](docs/change_log.md) — the proposed 48-hour customer reminder
- [Status update 1](docs/status_update_1.md) — sprint simulation progress
- [Status update 2](docs/status_update_2.md) — prototype results and remaining scope
- [Sprint Review](docs/sprint_review.md) — demonstrated result against the Sprint Goal
- [Retrospective](docs/sprint_retrospective.md) — lessons and improvements
- [API troubleshooting notes](docs/api_troubleshooting_notes.md) — a checklist developed during separate API exercises

## Remaining Backlog

PLD-6–9 cover the customer question-and-answer flow and are the next
functional area to consider.

PLD-12 covers an automatic reminder after 48 hours without a customer
response. It was approved in the training scenario and remains
unimplemented.

## Tools

Jira Cloud, Jira Automation, Git and GitHub.
