# COPI — Problem Definition

## Problem

When a new product enters an organization, the information needed to onboard it is often incomplete, inconsistent, or unavailable.

The resulting work is frequently handled through a combination of spreadsheets, email, manual review, and follow-up.

The problem is not simply that information is missing.

The larger problem is that there may be no consistent process for determining:

* What information is actually required
* What is missing or invalid
* Who is responsible for providing it
* What has already been requested
* Whether a response actually resolves the issue
* When the product can be considered complete

## Current-State Challenges

From a Product Operations perspective, the process can involve a lot of repetitive work:

**Identify → Email → Follow up → Receive → Review → Update → Check again**

Some common issues include:

* Requirements vary by product type
* Missing information may be identified manually
* Vendor requests may not be consistent
* Follow-ups can be difficult to track
* Responses may be partial or unclear
* The same information may be requested more than once
* It may be difficult to see exactly what remains outstanding
* The history of decisions and communications can be fragmented

## Who Is Affected?

### Product Operations

Needs a manageable way to identify and resolve outstanding product requirements without manually coordinating every step.

### Product Data / Master Data

Needs product information to be complete and usable before it moves into downstream systems.

### Vendors and Other Information Owners

Need clear requests that explain exactly what information is required and how to provide it.

### Downstream Users and Systems

Depend on product information being sufficiently complete and accurate for their use.

## Business Impact

An inefficient onboarding process can contribute to:

* Longer product onboarding times
* More manual operational effort
* Repeated communication
* Delays to downstream processes
* Inconsistent product information
* Limited visibility into onboarding status
* Difficulty reconstructing what happened

The impact will vary by organization and product type, so these areas would need to be validated with actual users and operational data.

## Opportunity

COPI could provide a consistent workflow around the problem without requiring every product type to follow exactly the same requirements.

The opportunity is to separate:

**What the business requires**

from

**How COPI manages the work required to satisfy those requirements.**

This would allow requirements and validation rules to change without rebuilding the core onboarding workflow.

## Potential Role of AI

AI could reduce some of the manual effort involved in the process, particularly where information is unstructured.

Potential opportunities include:

* Interpreting vendor responses
* Extracting information from documents
* Identifying potential inconsistencies
* Drafting requests and follow-ups
* Suggesting what additional information may be needed
* Helping match responses to outstanding requirements

AI should support the process while keeping requirements, decisions, and outcomes traceable.

## Initial Product Boundary

The initial problem being addressed is:

> **How can we move a new product from incomplete intake to a defined state of completeness through a repeatable, traceable process?**

The first COPI module will focus on this onboarding problem.

Broader product lifecycle management is a future opportunity rather than part of the initial problem definition.

## Assumptions to Validate

Several assumptions should be tested with users and stakeholders:

* Product requirements can be defined clearly enough to evaluate.
* Different product types can use configurable requirements.
* Missing or invalid information can be identified consistently.
* Responsibility for outstanding information can be determined.
* Vendors or other owners can provide responses through an appropriate process.
* A meaningful definition of "complete" can be established.
* Users will benefit from having the process and history in one place.
