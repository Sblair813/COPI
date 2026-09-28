# COPI Onboarding — Workflow

## Purpose

The onboarding workflow describes the current product hypothesis for how COPI could move a new product from initial intake to a defined state of completeness.

The goal is not simply to collect information. The goal is to determine whether the product satisfies the requirements that apply to it.

## Working Draft

This is a working draft of the COPI Onboarding workflow.

It represents the current product hypothesis and would be refined collaboratively with engineering, design, Product Operations, and other subject-matter experts.

In a real product environment, I would initially use a high-level workflow to establish a shared understanding of the problem, then work through the details collaboratively using a whiteboarding tool such as Mural.

The questions and exception scenarios in this document are intentionally included as topics for team discussion rather than decisions that have already been finalized.

## Core Loop

```text
New Product
    ↓
Receive Product Record
    ↓
Determine Applicable Requirements
    ↓
Evaluate Product
    ↓
Are Requirements Satisfied?
    │
    ├── Yes → Complete
    │
    └── No
          ↓
      Identify Gaps
          ↓
      Determine Owner
          ↓
      Create Request
          ↓
      Send Request
          ↓
      Track Communication
          ↓
      Receive Response
          ↓
      Process Response
          ↓
      Update Product Information
          ↓
      Revalidate
          ↓
      Continue or Complete
```

## Workflow Stages

### 1. Receive Product

A new product enters the onboarding process.

COPI creates or receives the information needed to establish an onboarding record.

**Questions to explore with the team:**

* What information is required at intake?
* Where does the product originate?
* How is the product uniquely identified?
* What happens if the initial information is incomplete?

---

### 2. Determine Applicable Requirements

COPI determines which requirements apply to the product.

Requirements may depend on characteristics such as product type, business context, or other configured criteria.

The workflow should remain separate from the rules that determine what is required.

**Questions to explore with the team:**

* Where do requirements come from?
* Who owns them?
* How are requirements associated with a product?
* How often do requirements change?

---

### 3. Evaluate Product

The product is evaluated against the applicable requirements.

COPI should be able to identify situations such as:

* Required information is missing
* Information is incomplete
* Information fails validation
* Required documentation is missing
* Information conflicts with another source

The specific validation approach would be defined with engineering and the relevant business stakeholders.

---

### 4. Identify Gaps

If the product does not satisfy all applicable requirements, COPI identifies the outstanding gaps.

Each gap should provide enough information to understand:

* What is missing or incorrect
* Which requirement is affected
* Who is responsible for resolving it
* What i
