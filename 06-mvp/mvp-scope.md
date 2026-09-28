# COPI Onboarding — MVP Requirements

## Purpose

This document captures the **working draft of the initial product requirements** for the COPI Onboarding MVP.

These requirements represent the current product thinking and are intended to establish the product behavior and outcomes needed for an initial version.

They are **not final technical or implementation requirements**. In a real product environment, these would be reviewed and refined collaboratively with engineering, design, Product Operations, and other relevant stakeholders.

## Working Draft

The requirements in this document are intended to provide a starting point for product and engineering discussions.

Some details are intentionally left open because the right solution would depend on:

* Existing systems and data
* Technical constraints
* Business rules
* User workflows
* Integration requirements
* Security and compliance considerations
* Feedback from users and stakeholders

The goal at this stage is to define **what the product needs to accomplish**, rather than prescribe exactly **how it should be built**.

---

# MVP Requirement Areas

## 1. Product Intake

COPI needs to accept a new product into the onboarding process.

**The MVP should:**

* Create or receive a product record.
* Establish a unique product identifier.
* Start an onboarding process for the product.
* Capture the information available at intake.
* Record the initial onboarding status.

**Questions for collaboration:**

* What information is required at intake?
* Where does the product originate?
* Which existing systems are involved?

---

## 2. Applicable Requirements

COPI needs to determine what requirements apply to a product.

**The MVP should:**

* Support configurable requirements.
* Associate requirements with applicable product characteristics or contexts.
* Identify the requirements being used to evaluate a product.
* Keep requirement definitions separate from the onboarding workflow.

**Questions for collaboration:**

* Who owns the requirements?
* Where should they be maintained?
* How are changes to requirements governed?

---

## 3. Product Evaluation

COPI needs to evaluate the product against its applicable requirements.

The MVP should be able to identify:

* Missing information
* Incomplete information
* Invalid information
* Missing required documentation

The specific validation rules would be defined with the appropriate business stakeholders and engineering.

**Questions for collaboration:**

* Which validations can be deterministic?
* Where might AI be useful?
* Which situations require human review?

---

## 4. Gap Management

COPI needs to make outstanding requirements visible and actionable.

For each outstanding requirement, the MVP should provide enough information to understand:

* What is missing or incorrect
* Which requirement is affected
* Who is responsible for providing or resolving it
* What action or information is needed

**Question for collaboration:**

What information does a Product Operations user need in order to act on a gap without additional investigation?

---

## 5. Vendor Communication

COPI needs to support requests for outstanding information.

**The MVP should:**

* Generate a request based on outstanding requirements.
* Identify the product.
* Identify what information is needed.
* Provide appropriate response instructions.
* Record that the request was made.

AI may assist with drafting or organizing requests, but the requirement behind the request should remain visible.

**Questions for collaboration:**

* Which requests should be automated?
* Which require human review?
* What communication channel should be supported first?

---

## 6. Communication Tracking

COPI needs to maintain enough communication history to understand the onboarding process.

The MVP should capture, where appropriate:

* What was requested
* Who received the request
* When it was sent
* Which requirements were involved
* Whether a response was received

The exact communication model would be refined during solution design.

---

## 7. Response Processing

COPI needs to process information received in response to an outstanding requirement.

The MVP should support:

* Complete responses
* Partial responses
* Responses that fail validation
* Responses that do not resolve the original requirement

Receiving a response should not automatically mark a requirement as complete.

**Questions for collaboration:**

* How should unstructured responses be handled?
* Where could AI assist?
* When should a person review a response?

---

## 8. Revalidation

COPI needs to evaluate the product again after relevant information changes.

The MVP should:

* Re-evaluate applicable requirements.
* Recognize requirements that are now satisfied.
* Keep unresolved requirements active.
* Identify newly discovered issues when appropriate.

**Question for collaboration:**

What events should trigger revalidation?

---

## 9. Completion

COPI needs to determine when a product has satisfied its applicable onboarding requirements.

A product should only be marked complete when:

* Applicable requirements have been evaluated.
* Required information satisfies the relevant validation criteria.
* Required documentation has been satisfied where applicable.
* No unresolved required requirements remain.

The definition of "complete" must be established by the business owner of the applicable requirements.

**Key product question:**

> Who owns the definition of "complete"?

---

## 10. Status & History

COPI needs to provide basic visibility into the current onboarding state and what has happened.

The MVP should provide visibility into:

* Current onboarding status
* Outstanding requirements
* Requests and responses
* Relevant status changes
* Completion

A more detailed audit and reporting model can evolve beyond the MVP.

---

# MVP Workflow

The requirements support the following core loop:

**Receive → Evaluate → Identify → Request → Receive Response → Revalidate → Complete**

If requirements remain unresolved, the process continues rather than prematurely marking the product complete.

---

# Non-Functional Considerations

These are areas to discuss with engineering rather than finalized technical requirements.

### Traceability

Users should be able to understand why a requirement is outstanding or considered satisfied.

### Accountability

Actions and decisions should be attributable to the appropriate user, process, or system.

### Configurability

Requirements should be changeable without redesigning the core onboarding workflow.

### Auditability

Important onboarding events should be retained so the history of the process can be understood.

### AI Transparency

Where AI contributes to evaluating or processing information, users should be able to understand the role AI played and retain appropriate human oversight.

---

# Open Product Questions

These questions would be explored through discovery and collaboration rather than assumed in the initial requirements:

* Where should product requirements be maintained?
* Who owns requirement changes?
* What constitutes a valid response?
* Which validations can be automated?
* Where should human review be required?
* Which communication channel should be supported first?
* How should conflicting information be handled?
* What happens when a vendor does not respond?
* Who can approve an exception?
* What information must be retained for audit purposes?
* Where can AI reduce manual effort without creating unacceptable risk?

---

# MVP Boundary

The MVP is intended to prove the core onboarding process, not solve every product-information problem.

### In Scope

* Product intake
* Configurable requirements
* Product evaluation
* Gap identification
* Vendor requests
* Communication tracking
* Response processing
* Revalidation
* Completion
* Basic status and history

### Not Yet Defined for MVP

* Advanced AI automation
* Complex integrations
* Multiple communication channels
* Advanced analytics
* Predictive capabilities
* Full product lifecycle management
* Automated conflict resolution

These may become future product opportunities as the core workflow is validated.
