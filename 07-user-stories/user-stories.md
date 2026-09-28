# COPI Onboarding — User Stories & Acceptance Criteria

## Purpose

This document captures the **working draft of the initial user stories and acceptance criteria** for the COPI Onboarding MVP.

These stories are intended to help clarify the user outcomes the product needs to support. They are not intended to represent every possible interaction or final system behavior.

In a real product environment, these would be reviewed and refined with engineering, design, Product Operations, and other relevant stakeholders.

---

## Primary User

The primary MVP user is **Product Operations**, responsible for moving products through onboarding and resolving missing or incomplete information.

Other users, including Product Administrators and vendors, interact with the process at specific points.

---

## User Stories

### 1. Receive a Product

**As a Product Operations user,**
I want to bring a new product into COPI,
so that I can begin the onboarding process.

**Acceptance criteria:**

* A product can be created or received in COPI.
* Required product information is identified.
* The product receives an onboarding status.
* The user can see what information is currently available.

---

### 2. Determine What Is Required

**As a Product Operations user,**
I want COPI to determine which requirements apply to a product,
so that I know what needs to be evaluated.

**Acceptance criteria:**

* Requirements can be configured.
* COPI identifies the applicable requirements for the product.
* The user can see the requirements being evaluated.
* Requirements can be updated as product or business rules change.

---

### 3. Evaluate a Product

**As a Product Operations user,**
I want COPI to evaluate the available product information against applicable requirements,
so that I can identify what is complete and what needs attention.

**Acceptance criteria:**

* COPI evaluates available information against applicable requirements.
* Requirements can be identified as satisfied, unsatisfied, or requiring review.
* The user can understand why an item requires attention.

---

### 4. Identify and Manage Gaps

**As a Product Operations user,**
I want COPI to identify missing or invalid information,
so that I know what needs to be resolved.

**Acceptance criteria:**

* Missing or invalid information is identified.
* Outstanding items can be viewed together.
* An owner can be associated with an outstanding item.
* The status of an outstanding item can be tracked.

---

### 5. Request Missing Information

**As a Product Operations user,**
I want to create a request for missing information,
so that the appropriate person or vendor knows what is needed.

**Acceptance criteria:**

* A request can be created from an outstanding requirement.
* The request identifies the information needed.
* The request can be associated with the product and outstanding requirement.
* The user can see whether the request has been sent.

---

### 6. Process a Response

**As a Product Operations user,**
I want to record and process information received in response to a request,
so that COPI can determine whether the outstanding requirement has been addressed.

**Acceptance criteria:**

* A response can be associated with the relevant product and request.
* Information from the response can be captured or updated.
* Partial responses can remain outstanding.
* Responses requiring additional review can be identified.

**AI opportunity:**
AI could assist with interpreting unstructured responses or extracting information from documents, with appropriate human review.

---

### 7. Revalidate the Product

**As a Product Operations user,**
I want COPI to re-evaluate the product after information changes,
so that I know whether outstanding requirements have been resolved.

**Acceptance criteria:**

* Updated information can trigger or support revalidation.
* Previously outstanding requirements are evaluated again.
* New gaps can be identified.
* The product remains in onboarding until applicable requirements are satisfied.

---

### 8. Complete Onboarding

**As a Product Operations user,**
I want COPI to show when a product has satisfied its applicable requirements,
so that I know onboarding is complete.

**Acceptance criteria:**

* COPI determines completion based on applicable requirements.
* The user can see what contributed to completion.
* The product receives a completed status.
* The onboarding history remains available after completion.

---

## Supporting Story — Product Administration

### 9. Configure Requirements

**As a Product Administrator,**
I want to manage the requirements used during onboarding,
so that COPI can support different product types and business rules.

**Acceptance criteria:**

* Requirements can be added or updated.
* Requirements can be associated with applicable product types or conditions.
* Changes to requirements are traceable.
* The product team can distinguish current requirements from previous versions where needed.

---

## Working Notes

These stories intentionally leave some implementation details open.

Questions to refine collaboratively include:

* What constitutes a valid response?
* Which requirements can be evaluated automatically?
* Where is human review required?
* When should AI be used versus deterministic rules?
* What happens when information conflicts?
* Who is authorized to approve an exception?
* What communication methods are supported initially?
* What information must be retained for audit/history?

## MVP Product Loop

The stories support the core COPI onboarding loop:

**Receive → Evaluate → Identify → Request → Receive Response → Revalidate → Complete**

The goal of the MVP is not to automate every step. The goal is to prove that COPI can provide a repeatable and traceable way to move a product through onboarding.
