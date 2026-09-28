# COPI Onboarding — Product Workflow

## Purpose

The COPI Onboarding workflow defines how a new product moves from initial intake to a completed product record.

The workflow is designed to continuously evaluate the product record, identify outstanding requirements, coordinate resolution, and determine when the product is ready for downstream use.

---

## End-to-End Workflow

```text
NEW PRODUCT
     |
     v
RECEIVE PRODUCT RECORD
     |
     v
DETERMINE APPLICABLE REQUIREMENTS
     |
     v
VALIDATE PRODUCT RECORD
     |
     v
ARE REQUIREMENTS SATISFIED?
     |
   /   \
 YES    NO
 |       |
 v       v
COMPLETE  IDENTIFY GAPS
           |
           v
      DETERMINE OWNER
           |
           v
      CREATE REQUEST
           |
           v
      SEND REQUEST
           |
           v
    LOG COMMUNICATION
           |
           v
     AWAIT RESPONSE
           |
           v
    RECEIVE RESPONSE
           |
           v
     PROCESS RESPONSE
           |
           v
      UPDATE RECORD
           |
           v
        REVALIDATE
           |
           +------------------+
                              |
                    Requirements satisfied?
                              |
                         NO   |   YES
                         |    |
                         |    v
                         |  COMPLETE
                         |
                         +----> IDENTIFY REMAINING GAPS
```

---

# Workflow Stages

## 1. New Product

A new product is submitted for onboarding.

The initial submission may contain a complete set of information, a partial set of information, or information requiring validation.

**COPI responsibility:**

Create or receive the product onboarding record and initiate evaluation.

---

## 2. Determine Applicable Requirements

COPI determines which requirements apply to the product.

Requirements may depend on factors such as:

* Product type
* Product category
* Business context
* Intended use
* Market or geography
* Organizational rules
* Industry-specific requirements

The core COPI workflow should remain independent of these rules.

---

## 3. Validate Product Record

COPI evaluates the product record against its applicable requirements.

Validation should identify more than simply empty fields.

Potential findings include:

* Missing information
* Incomplete information
* Invalid values
* Incorrect format
* Conflicting information
* Missing documentation
* Information requiring verification

---

## 4. Determine Completion

COPI determines whether the product record satisfies all applicable requirements.

### If complete:

The product proceeds to completion.

### If incomplete:

COPI identifies the outstanding requirements.

---

## 5. Identify Gaps

COPI creates a structured list of outstanding requirements.

Each gap should identify, where applicable:

* Requirement
* Product
* Current value
* Expected value or format
* Reason the requirement is outstanding
* Responsible party
* Priority
* Supporting documentation needed
* Validation criteria

The goal is to convert a vague condition such as "product information incomplete" into actionable work.

---

## 6. Determine Responsible Party

For each outstanding requirement, COPI determines who is responsible for providing or resolving the information.

Potential responsible parties may include:

* Vendor
* Internal product team
* Data steward
* Business owner
* Other designated source

Responsibility should be associated with the requirement rather than assumed to be the same for every missing field.

---

## 7. Create Vendor Request

COPI creates a communication containing the outstanding requirements.

The request should clearly communicate:

* Product identification
* Outstanding information
* Specific requirements
* Required format
* Examples where useful
* Supporting documentation requirements
* Response instructions
* Requested response timing
* Reference to prior requests when applicable

The communication should be actionable rather than simply notifying the vendor that information is missing.

---

## 8. Send and Log Communication

The request is sent to the responsible party.

COPI records the communication as part of the onboarding history.

The log should capture information such as:

* Date and time
* Recipient
* Product
* Requirements requested
* Communication type
* Request status
* Related onboarding event

---

## 9. Await Response

The product remains in an active onboarding state while outstanding requirements are unresolved.

COPI should maintain visibility into:

* Outstanding requests
* Age of requests
* Responsible party
* Follow-up status
* Previous communications

---

## 10. Receive and Process Response

When a response is received, COPI evaluates the information provided.

A response may:

* Fully resolve a requirement
* Partially resolve a requirement
* Provide invalid information
* Introduce conflicting information
* Require additional clarification
* Provide documentation requiring review

COPI should not assume that receiving a response means the requirement has been satisfied.

---

## 11. Update Product Record

Validated information is applied to the product record.

The system should preserve appropriate history of the update, including the source of the information and the associated onboarding event.

---

## 12. Revalidate

After the product record is updated, COPI evaluates the record again against the applicable requirements.

This is a critical part of the workflow.

The system does not simply mark individual fields as resolved.

It reassesses the product as a whole.

---

## 13. Continue or Complete

### If requirements remain outstanding:

COPI identifies the remaining gaps and continues the workflow.

### If all requirements are satisfied:

COPI marks the onboarding process complete.

---

# Completion Principle

COPI should determine completion based on defined requirements rather than the number of communication cycles.

A product may require:

* One request
* Multiple requests
* Partial responses
* Clarification
* Multiple vendors
* Internal resolution

The number of interactions should not determine completion.

The product is complete when its applicable requirements have been satisfied.

---

# Exception Considerations

The standard workflow must eventually account for scenarios such as:

* Vendor does not respond
* Vendor provides only partial information
* Vendor provides conflicting information
* Required information cannot be obtained
* Information fails validation
* Multiple parties provide conflicting information
* A requirement changes while onboarding is in progress
* A product is withdrawn before completion
* A product is intentionally approved with an exception
* A previously completed product becomes incomplete

These scenarios are outside the basic happy-path workflow and should be addressed through separate business rules and exception requirements.

---

# Workflow Principle

COPI is designed as a continuous evaluation loop rather than a one-time data-entry process.

The central workflow is:

**Evaluate → Identify → Communicate → Receive → Validate → Re-evaluate**

The loop continues until the product satisfies its defined completion criteria.
