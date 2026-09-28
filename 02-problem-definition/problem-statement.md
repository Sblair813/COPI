# COPI — Problem Definition

## Problem Statement

Organizations frequently receive new product records that are incomplete, inconsistent, or missing information required for downstream use.

The process of resolving these gaps is often dependent on manual identification, communication, follow-up, data entry, and status tracking.

As a result, product onboarding can become slow, inconsistent, difficult to monitor, and difficult to audit.

## Current-State Challenges

### 1. Missing Information Is Identified Manually

People may need to inspect product records to determine which required information is absent or incomplete.

This creates repetitive work and increases the possibility that missing requirements will be overlooked.

### 2. Requirements May Not Be Consistently Applied

Different products, product categories, or business situations may have different information requirements.

Without a structured requirements framework, individuals may rely on experience, spreadsheets, documentation, or tribal knowledge to determine what is needed.

### 3. Vendor Communication Is Often Reactive

When information is missing, someone must determine:

* What is missing
* Who should provide it
* What exactly should be requested
* What format is acceptable
* Whether supporting documentation is required

Requests may therefore vary in clarity and completeness.

### 4. Follow-Up Requires Manual Tracking

A vendor response may be incomplete or may resolve only some of the outstanding requirements.

Without a structured process, teams may need to manually track:

* What was requested
* When it was requested
* What was received
* What remains outstanding
* When follow-up is required

### 5. Completion May Be Difficult to Determine

A product record can appear populated while still failing one or more business requirements.

The organization needs a consistent way to determine whether a product is actually ready for downstream use.

### 6. Process History May Be Fragmented

Product onboarding activity may occur across email, spreadsheets, product systems, shared documents, and individual knowledge.

This can make it difficult to reconstruct the history of how a product record was completed.

## Business Impact

An inconsistent onboarding process can contribute to:

* Longer product onboarding cycles
* Increased manual workload
* Repeated vendor communication
* Delayed downstream processes
* Inconsistent product information
* Difficulty identifying responsibility for outstanding data
* Limited visibility into onboarding status
* Increased operational risk
* Difficulty demonstrating how product information was obtained or resolved

The specific impact will vary by organization and industry.

## User Impact

### Product Operations

People responsible for onboarding products may spend significant time identifying gaps, communicating with vendors, tracking responses, and determining completion.

### Vendors

Vendors may receive requests that are unclear, incomplete, duplicated, or difficult to act upon.

### Downstream Users and Systems

Downstream teams and systems depend on product records being sufficiently complete and reliable for their intended use.

### Management

Leaders may lack a consistent view of onboarding volume, status, outstanding work, vendor response activity, and process performance.

## Opportunity

COPI provides an opportunity to transform product onboarding from a primarily manual coordination process into a structured, traceable workflow.

The opportunity is not simply to automate email or data entry.

The opportunity is to create a system that understands:

* What information is required
* What information is missing
* Who is responsible for resolving the gap
* What communication is required
* What has already occurred
* What remains outstanding
* Whether the product record is ready for use

## Problem Boundaries

The initial COPI Onboarding module focuses on the process of bringing a new product record to a defined state of completeness.

The initial scope does not attempt to solve every product-data or product-lifecycle problem.

Potential future capabilities such as ongoing monitoring, change management, and long-term product maintenance are intentionally separated from the initial onboarding problem.

## Key Assumptions

The initial product concept assumes:

1. Product requirements can be represented as configurable rules.
2. A product record can be evaluated against those requirements.
3. Missing or invalid information can be identified.
4. A responsible party can be associated with outstanding information.
5. Vendors or other responsible parties can provide information in response to requests.
6. Product records can be updated as information is received.
7. The product can be re-evaluated after updates.
8. A defined set of requirements can determine when onboarding is complete.

These assumptions should be validated as the product is further defined.

## Desired Future State

A new product enters the onboarding process.

COPI evaluates the product against its applicable requirements and identifies outstanding information.

COPI communicates clear, actionable requests to the appropriate responsible party and records the request.

When information is received, COPI evaluates the response, updates the onboarding state, and identifies any remaining gaps.

The process continues until the product record meets its defined completion criteria.

The organization can then see both the current state of the product record and the history of how it reached that state.
