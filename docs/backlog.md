# Product Backlog — Digital Additional Work Approval

Jira space: PolenRep Legacy to Digital (PLD)  
Epic: PLD-1 — Digital Additional Work Approval  
Source checked: 2026-11-01

Story descriptions and acceptance criteria below were copied from Jira.
Only Markdown formatting was changed.

## Sprint 1

Configured dates in Jira: 2026-10-15 to 2026-10-29.  
Status verified on 2026-11-01: closed.

### Sprint Goal

Create a usable end-to-end flow for handling additional work requests
from subcontractor submission to communicating the customer's final decision.

### Scope

Six stories were marked Gotowe (Done) in the simulated sprint:
PLD-2, PLD-3, PLD-4, PLD-5, PLD-10 and PLD-11.

PLD-10 includes further customer questions, which overlap with PLD-6–9
in the remaining backlog. This overlap needs to be resolved when
planning implementation of the question-and-answer flow.

See the [Definition of Done](project_brief.md#definition-of-done)
and the [case study](case_study.md) for the working prototype and tests.

## Sprint 1 Stories — Done in the Simulation

### PLD-2 — Register additional work

As an external subcontractor, I want to register additional repair work, including description of the problem, proposed repair and estimated subcontractor cost, so that PolenRep can evaluate the additional work before requesting customer approval.

Acceptance Criteria:

- The subcontractor can create an additional work request for a specific vehicle project.
- The request includes a description of the problem, the proposed repair and the subcontractor’s estimated cost.
- The request is saved and becomes available to the PolenRep project manager for review.

### PLD-3 — Attach photos and evidence

As an external subcontractor, I want to attach photos and technical documentation to an additional work request, so that PolenRep can review the problem and provide supporting evidence to the customer.

Acceptance Criteria:

- The subcontractor can attach photos and supporting documents to an additional work request.
- Attachments are linked to the correct vehicle project and additional work request.
- The PolenRep project manager can view the attached photos and documents during review.

### PLD-4 — Review additional work and prepare a customer quotation

As a PolenRep project manager, I want to review the subcontractor’s proposed repair and estimated cost and prepare a separate customer-facing quotation, so that PolenRep can control the commercial terms of the additional work.

The subcontractor cost and customer-facing quotation are kept separate.

Acceptance Criteria:

- The PolenRep project manager can review the subcontractor’s description, proposed repair, supporting evidence and estimated cost.
- The project manager can define a separate customer-facing price, including PolenRep’s margin if applicable.
- The subcontractor’s estimated cost and the customer-facing price are kept separate.

### PLD-5 — Request customer approval

As a PolenRep project manager, I want to send the customer a reviewed additional work proposal, including the repair description, supporting documentation and customer-facing price, so that the customer can make an informed decision.

Acceptance Criteria:

- The PolenRep project manager can send the reviewed additional work proposal to the customer.
- The proposal includes the repair description, supporting evidence and the customer-facing price.
- The customer receives the proposal linked to the correct vehicle project and additional work request.

### PLD-10 — Record customer approval, rejection or further questions

As a customer, I want to approve, reject or ask further questions about proposed additional work.

The system automatically records approval or rejection. If I have further questions, they are sent to the project manager and the question-and-answer process can repeat until I make a final decision.

Acceptance Criteria:

- The customer can approve the proposal, reject it, or submit another question.
- Approval or rejection is automatically recorded against the correct additional work proposal.
- If the customer submits another question, the proposal remains pending and the question is sent back to the PolenRep project manager.

### PLD-11 — Notify the subcontractor of the customer's decision

As an external subcontractor, I want to receive the customer's final decision through the system, so that I know whether my proposed additional work has been approved or rejected.

The system notifies the relevant subcontractor after the customer approves or rejects the proposal.

Acceptance Criteria:

- The relevant subcontractor receives the customer’s final approval or rejection.
- The notification is linked to the correct vehicle project and additional work request.

## Remaining Product Backlog — Not Started

PLD-6–9 are the next functional area to consider together. PLD-12 remains
a later enhancement; see [CR-01](change_log.md).

### PLD-6 — Ask questions about additional work

As a customer, I want to submit questions about the proposed repair or its price to PolenRep, so that I can clarify any concerns before approving or rejecting the additional work.

Questions must be associated with the relevant additional work proposal.

Acceptance Criteria:

- The customer can submit questions about the proposed repair or its price.
- The question is linked to the correct additional work proposal.
- The PolenRep project manager receives the customer’s question for review.

### PLD-7 — Review and route customer questions

As a PolenRep project manager, I want to review customer questions and either answer them directly or forward them to the relevant subcontractor, so that the customer receives accurate information from the appropriate source.

Acceptance Criteria:

- The PolenRep project manager can review the customer’s question.
- The project manager can either answer the question directly or forward it to the relevant subcontractor.
- A forwarded question remains linked to the correct additional work proposal.

### PLD-8 — Respond to technical questions

As an external subcontractor, I want to receive technical questions forwarded by PolenRep and provide my answers, so that the project manager can clarify the proposed repair with the customer.

Acceptance Criteria:

- The subcontractor can view technical questions forwarded by the PolenRep project manager.
- The subcontractor can submit a response to the forwarded question.
- The response is linked to the correct additional work proposal and returned to the PolenRep project manager for review.

### PLD-9 — Review and send subcontractor responses to the customer

As a PolenRep project manager, I want to review technical responses received from subcontractors, make necessary corrections or clarifications and approve them before sending them to the customer, so that customer communication remains accurate and under PolenRep's control.

Acceptance Criteria:

- The PolenRep project manager can review the subcontractor’s response before it is sent to the customer.
- The project manager can edit or clarify the response if needed.
- The approved response is sent to the customer and remains linked to the correct additional work proposal.

### PLD-12 — Automatically remind customers about unanswered proposals

As a PolenRep project manager, I want customers to receive an automatic reminder about unanswered additional work proposals, so that I can reduce delays and manual follow-up.

Acceptance Criteria:

- The customer receives a reminder if they have not responded within 48 hours of proposal delivery.
- The reminder is not sent if the customer has already approved, rejected or asked a question about the proposal.
- The reminder is sent to the correct customer and refers to the relevant additional work proposal.
