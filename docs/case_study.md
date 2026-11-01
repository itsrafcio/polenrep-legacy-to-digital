# PolenRep Legacy-to-Digital Case Study

## Business Context

PolenRep manages international vehicle repair and restoration
projects. During an active project, a workshop may identify
additional work that was not included in the previously approved scope.

The additional work must be explained, priced and approved by
the customer before it can proceed.

## AS-IS Process

The existing process works through email, WhatsApp and phone calls.

The workshop reports the problem, proposed repair, evidence and
estimated cost to the PolenRep project manager. The project manager
reviews the information, prepares a customer-facing proposal and
sends it to the customer.

The customer can approve, reject or request more information.
Questions and answers pass through the project manager until the
customer makes a final decision. The project manager records the
decision and communicates it to the workshop.

The process works, but repetitive follow-up and information transfer
are handled manually.

## Requirements Analysis

The proposed digital process needed to support:
- registration of additional work for a specific vehicle project;
- photos and supporting evidence;
- separate subcontractor cost and customer-facing price;
- presentation of the proposal to the customer;
- approval, rejection or further questions;
- recording the customer’s decision;
- communication of the decision to the correct workshop.

Invoicing, parts procurement, workshop scheduling and complete
customer project management were outside the project scope.

## Target Process

The target process connects the workshop, PolenRep project manager
and customer in one structured flow:
1. The workshop registers the additional work and evidence.
2. The project manager reviews the request and prepares the
   customer-facing quotation.
3. The customer receives the proposal.
4. The customer approves, rejects or asks a question.
5. The decision or question is recorded against the correct request.
6. The workshop receives the final decision.

## Backlog and Sprint

The requirements were divided into an Epic and user stories in Jira.

Sprint 1 contained six core stories covering registration, evidence,
quotation preparation, customer approval request, recording the
decision and informing the workshop.

Sprint Goal:

> Create a usable end-to-end flow for handling additional work
> requests from subcontractor submission to communicating the
> customer’s final decision.

PLD-6–9, covering the customer question-and-answer loop, remained
in the Product Backlog.

## Implemented and Tested Result

The Sprint 1 workflow was completed as a training simulation.

A thin Jira prototype covering part of the target process was
configured separately in the PolenRep Approval Demo (PAD) Jira space. 
PAD-1 used fictional data for an additional brake-hose replacement 
and contained:
- vehicle and customer information;
- problem and proposed repair;
- photo evidence;
- subcontractor cost;
- separate customer-facing price;
- schedule impact;
- decision statuses;
- a filtered list of requests awaiting a decision.

In this prototype, the project manager manually records the
customer’s decision by changing the PAD-1 status. A Jira automation
then sends the recorded decision to the workshop’s test inbox when
the status changes to accepted (Zaakceptowana) or rejected
(Odrzucona).

Smart values insert the issue key, summary and current status into
the message.

This prototype tests the final handoff only. It does not implement
the customer-facing submission and decision capture.

## Test Results

Three notification scenarios were checked:
1. Acceptance — the email arrived with PAD-1, the correct summary
   and the status Zaakceptowana.
2. Rejection — the email arrived with PAD-1, the correct summary
   and the status Odrzucona.
3. Pending decision — changing the status to Oczekuje na decyzję
   did not send a decision email.

No defects were observed in these checks.

The tests used fictional data and the project owner’s email address
as the workshop’s test inbox.

## Scope Change

A request for an automatic reminder after 48 hours without a customer
response was analysed during the training scenario.

The change was approved and added to the backlog as PLD-12.
It was not implemented or tested.

## Risks and Issues

An attachment-access problem was identified during the Sprint 1
simulation. PLD-3 was reopened, corrected and retested before being
returned to Done.

The assumption that subcontractors will adopt the digital workflow
remains open and would require validation during a pilot or UAT.

## Actual Result and Limitations

The PAD prototype demonstrates structured recording of additional
work and automated notification after a manually recorded decision.

It does not implement customer submission, automatic recording of
the customer’s response, the complete question-and-answer loop or
notification routing to actual subcontractors.

Therefore, the prototype does not demonstrate the complete
end-to-end implementation described by the Sprint Goal.

## Backlog Decision

PLD-6–9 should be considered together as the next functional area
because they cover one question-and-answer flow between the customer,
PolenRep and the workshop.

PLD-12 remains a later enhancement.

## Lessons Learned

The implementation scope, covered requirements and test evidence
must be agreed before configuration begins.

A Jira status alone does not prove that a business function works.
The demonstrated result must be separated from simulated work and
unsupported assumptions.