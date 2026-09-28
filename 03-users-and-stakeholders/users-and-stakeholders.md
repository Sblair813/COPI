# COPI — Users & Stakeholders

## Purpose

COPI involves multiple participants in the product onboarding process.

Not every participant is a direct user of the COPI platform. Some interact with the workflow externally, while others consume the resulting product information.

Understanding these roles helps define product requirements without assuming that every stakeholder needs the same experience.

---

## Primary Users

### Product Operations

**Role:** Primary operational user of COPI.

Product Operations is responsible for ensuring that new product records are properly onboarded and ready for downstream use.

**Needs:**

* Visibility into new products entering onboarding
* Clear identification of missing information
* Visibility into outstanding vendor requests
* Ability to understand current onboarding status
* Visibility into vendor responses
* Ability to determine why an item is not complete
* Access to onboarding history
* Confidence that completion criteria have been satisfied

**Primary outcome:**

Reduce manual coordination while maintaining control and visibility over product onboarding.

---

## Secondary Users

### Product Data or Master Data Teams

**Role:** Maintains or governs product information.

**Needs:**

* Consistent product-data requirements
* Data validation
* Visibility into data-quality issues
* Clear ownership of missing information
* Traceability of changes
* Consistent completion criteria

**Primary outcome:**

Improve the consistency and reliability of product information.

---

### Business or Product Administrators

**Role:** Defines or manages the rules that determine what is required for different types of products.

**Needs:**

* Ability to define required information
* Ability to configure validation rules
* Ability to establish responsible parties
* Ability to manage requirements by product type or context
* Visibility into rule effectiveness

**Primary outcome:**

Maintain the business rules that determine product completeness without changing the core onboarding process.

---

## External Participants

### Vendors

**Role:** External source of product information.

Vendors may provide information needed to complete a product record.

**Needs:**

* Clear requests
* Specific identification of missing information
* Understanding of required formats or documentation
* Ability to provide responses efficiently
* Visibility into outstanding requests
* Reduced duplicate requests

**Primary outcome:**

Provide the required information with minimal ambiguity and unnecessary back-and-forth.

---

## Downstream Consumers

### Downstream Systems

**Role:** Consume completed product records.

These may include enterprise applications, catalogs, operational systems, reporting systems, or other data consumers.

**Needs:**

* Reliable product information
* Consistent data structures
* Defined completion criteria
* Appropriate data quality
* Timely availability of completed records

**Primary outcome:**

Receive product information that is sufficiently complete and reliable for its intended use.

---

### Business Users

**Role:** Use product information after onboarding.

Depending on the organization, these may include operations, sales, purchasing, customer service, clinical, administrative, or other business functions.

**Needs:**

* Accessible product information
* Confidence in data quality
* Appropriate product attributes
* Timely availability

**Primary outcome:**

Use product information without having to resolve the original onboarding problems themselves.

---

## Stakeholder Summary

| Stakeholder                      | Relationship to COPI     | Primary Need                              |
| -------------------------------- | ------------------------ | ----------------------------------------- |
| Product Operations               | Primary user             | Manage onboarding efficiently             |
| Product Data / Master Data       | Operational / governance | Maintain data quality                     |
| Business / Product Administrator | Configuration            | Define requirements and rules             |
| Vendor                           | External participant     | Provide missing information               |
| Downstream Systems               | Consumer                 | Receive complete product records          |
| Business Users                   | Consumer                 | Use reliable product information          |
| Management                       | Oversight                | Understand process status and performance |

---

## Stakeholder Principle

COPI should not be designed around a single user's workflow.

The product must balance:

* Operational efficiency
* Data integrity
* Vendor usability
* Business requirements
* Downstream reliability
* Traceability
* Governance

Improving one part of the process should not create unnecessary burden or risk elsewhere in the product lifecycle.

---

## Key Product Question

One of the most important questions to resolve during further product discovery is:

> Who owns the definition of "complete"?

COPI can identify whether a record satisfies defined requirements, but the organization must establish the authority and governance behind those requirements.

This distinction separates the **COPI engine** from the **business rules it executes**.
