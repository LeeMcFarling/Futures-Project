---
id: industrial-permitting-shot-clock
title: Industrial Permitting Shot Clock Framework
sidebar_label: Permitting Shot Clock
sidebar_position: 2
slug: /manufacturing/permitting-shot-clock
domain: Manufacturing
subdomain: Manufacturing
policy_type: Procedural Enforcement Framework
status: Draft
version: 0.2
author: Futures Project
dependencies:
  - manufacturing-regulatory-modernization-sandbox
  - regulatory-modernization-corps
  - unified-law-regulation-repository
  - execution-corps-industrial-deployment-model
  - department-of-data-and-accountability
related_initiatives:
  - industrial-siting-compact
  - industrial-demand-coordination-system
  - manufacturing-pca-instruments-framework
tags:
  - manufacturing
  - permitting
  - regulation
  - execution
  - throughput
last_updated: 2026-04-07
---

# Industrial Permitting Shot Clock Framework

## What This Is

The Industrial Permitting Shot Clock is a time enforcement architecture that operates across all stages of industrial permitting within a manufacturing corridor. It ensures that no permitting stage can stall indefinitely — every delay must be classified, visible, and resolved through a defined pathway.

The shot clock does not replace the Regulatory Modernization Corps (RMC), which tracks and manages processes proactively. It is the backstop that activates when proactive management is not sufficient. In a well-functioning system, the shot clock rarely fires — because the RMC has already intervened.

This document should be read alongside the RMC Industrial Deployment Model, which describes the proactive layer, and the ULRR architecture, which describes how process steps are mapped and stored.

---

## Purpose

The shot clock framework ensures that:

- regulatory processes progress within defined time bounds
- delays are classified, observable, and resolved
- no stage of permitting can stall indefinitely
- industrial deployment timelines are predictable and compressible

This framework operates in conjunction with the Manufacturing Regulatory Modernization Sandbox (RMS), which defines **how** permitting occurs.
The shot clock defines **how fast it must occur**.

---

## Core Principle — Continuous Time Accountability

The permitting system operates under a continuous clock model:

> Time is always accounted for.

There are no unmeasured intervals between stages.
Every stage must be:

- advancing
- blocked (with classification)
- or escalated

Undefined "pending" states are not permitted.

---

## Stage Architecture

The industrial permitting lifecycle is divided into five standardized stages.

---

### Stage 0 — Pre-Application Validation

**Objective:**
Ensure submissions are complete and eligible for RMS processing.

**Scope:**
- completeness verification
- eligibility confirmation
- template alignment

**Clock Type:** Deterministic (short duration)

**Rule:**
Post-stage information requests must be formally classified as blocking conditions.

---

### Stage 1 — Intake & Pathway Assignment

**Objective:**
Assign the project to a defined RMS procedural pathway.

**Scope:**
- module selection
- lead agency designation
- interagency coordination structure

**Clock Type:** Deterministic (very short duration)

**Rule:**
Process architecture is locked at stage completion.

---

### Stage 2 — Parallel Review Execution

**Objective:**
Conduct all regulatory reviews concurrently under a unified administrative record.

**Scope:**
- environmental review
- zoning confirmation
- grid interconnection initiation
- technical and safety analysis

**Clock Type:** Analytical (primary system clock)

**Rules:**
- all reviews proceed in parallel
- blocking conditions must be immediately classified
- sequential review is not permitted

---

### Stage 3 — Determination & Conditional Approval

**Objective:**
Issue approval, conditional approval, or required modifications.

**Scope:**
- final determinations
- conditional approvals
- compliance adjustments

**Clock Type:** Deterministic (decision-bound)

---

### Stage 4 — Pre-Construction Authorization

**Objective:**
Authorize construction initiation for approved components.

**Scope:**
- permit issuance
- phased construction authorization
- inspection coordination

**Clock Type:** Deterministic (execution-bound)

---

## Clock Types

### Type I — Deterministic Clocks
- fixed duration
- minimal variance
- used for administrative and decision stages

---

### Type II — Analytical Clocks
- bounded duration
- support escalation pathways
- used for review and evaluation

---

### Type III — Safety-Bound Clocks
- no auto-advance
- escalation-only progression
- used for safety-critical determinations

---

## Stage Transition Rules

### Automatic Advancement
If no blocking condition exists at clock expiry:

→ the system advances immediately

---

### Conditional Advancement
If a blocking condition exists:

→ advancement occurs only upon resolution

---

### Partial Advancement

Where permissible:

- approved components advance
- blocked components remain

This enables construction to begin without full-system completion.

---

## Blocking Condition Framework

All delays must be classified under a closed set of categories.

- **A — Safety-Critical Uncertainty**
- **B — Statutory Non-Compliance**
- **C — Information Deficiency**
- **D — Analytical Conflict**
- **E — Capacity Constraint**
- **F — Legal Ambiguity**

Unclassified delays are invalid.

---

## Blocking Condition Routing — Schema 1 vs Schema 2

When a blocking condition is classified, the RMC performs a secondary diagnostic to determine whether the delay originates in the process (Schema 2) or in the underlying law (Schema 1). This distinction determines the resolution pathway.

The ULRR maintains two linked schemas. Schema 1 is the legal and regulatory reference tree — what the law requires. Schema 2 is the execution process map derived from it — how the law actually runs, step by step, with owners, timelines, and dependencies.

**Schema 2 blocking conditions — process problems**

The legal authority permits a faster or more efficient process, but current practice does not achieve it. Examples include an agency taking longer than its statutory deadline because of staffing, a dataset not being pre-loaded when it could be, or two steps running sequentially when the law permits parallelization.

These are resolved through RMC coordination and DoDA automation. No law needs to change.

Resolution pathways by condition type:

- **C (Information Deficiency)** — almost always Schema 2. Data exists and could be pre-loaded via DoDA API. Resolution: automation or data pre-loading.
- **D (Analytical Conflict)** — usually Schema 2. Agencies are using different models or datasets. Resolution: forced convergence on shared inputs.
- **E (Capacity Constraint)** — always Schema 2. The law does not require slow staffing. Resolution: resource deployment.

**Schema 1 blocking conditions — legal problems**

The statutory framework requires a timeline, sequence, or process that cannot be improved without changing the underlying law or regulation. These cannot be fixed through process optimization within the sandbox.

Resolution pathways by condition type:

- **A (Safety-Critical Uncertainty)** — may be Schema 1 if the safety review requirement is statutory and no acceleration is legally permitted. No auto-advance. Escalate to appropriate authority.
- **B (Statutory Non-Compliance)** — by definition Schema 1. The project does not comply with a legal requirement. The path is compliance, not optimization.
- **F (Legal Ambiguity)** — frequently Schema 1. The ambiguity is in the statute or regulation itself, not in how it is being executed. Resolution: temporary authoritative interpretation logged for reform routing, plus escalation to the legislative or rulemaking channel.

**Why this distinction matters**

Schema 2 problems should be resolved rapidly through RMC and DoDA. Treating them as Schema 1 problems (requiring legislative action) is a failure of process management — it is slower and unnecessary.

Schema 1 problems cannot be resolved through process optimization. Treating them as Schema 2 problems (fixable through coordination) is a failure of legal analysis — it produces workarounds that don't hold or reforms that overclaim their authority.

All Schema 1 blocking conditions are documented and routed to the appropriate reform channel while the process advances on all other steps not affected by the legal constraint.

---

## Escalation Routing

Each blocking condition triggers immediate escalation into a defined resolution pathway.

- Safety → priority escalation, no advancement
- Compliance → bounded corrective loop
- Information → applicant-dependent resolution or DoDA pre-loading
- Conflict → forced interagency convergence on shared inputs
- Capacity → automatic resource augmentation
- Ambiguity → temporary authoritative interpretation + Schema 1 reform routing + system logging

Escalation converts delay into a structured, time-bound problem.

---

## Escalation Clocks

All escalations operate under secondary clocks.

- resolution timelines are predefined
- escalation cannot be indefinite
- all outcomes must resolve to:
  - cleared
  - reclassified
  - elevated

---

## Dual Consequence Enforcement

At shot clock expiry:

1. **Procedural auto-advance** (non-safety cases)
2. **Mandatory escalation and logging**

No clock expiry is silent.

---

## The Shot Clock as Diagnostic Instrument

The shot clock is not primarily an enforcement mechanism. It is a diagnostic instrument.

Clock expiry is a signal that something in the system failed to move as expected. The first question is not "who missed the deadline" — it is "why did this step exceed its expected duration, and is that a Schema 2 problem we can fix or a Schema 1 constraint we need to route?"

This framing is important for how the RMC operates. The RMC does not wait for clock expiry to intervene. It monitors leading indicators — time-in-stage relative to expected duration, missing inputs, interagency coordination gaps — and intervenes before the clock fires. When the shot clock does trigger, it means the RMC's proactive intervention was not sufficient, and the system escalates to a more formal resolution pathway.

A well-functioning corridor will have few shot clock events — not because timelines were padded, but because problems were caught and resolved before they became failures.

---

## Anti-Gaming Safeguards

- repeated blocking triggers review
- safety classifications require justification
- information requests must be complete and non-iterative
- capacity constraints trigger resource deployment, not delay
- Schema 1 vs Schema 2 classification is logged and auditable
- all events are publicly logged via DoDA

---

## System Integration

The shot clock framework is synchronized with:

- RMS procedural modules
- ULRR Schema 2 process map (step-level clock attribution)
- RMC live process tracking
- DoDA performance dashboards and telemetry
- Execution Corps sequencing authority
- PCA capital deployment thresholds
- industrial demand coordination system

---

## Time Compression Mechanisms

The framework achieves compression through:

- parallel review execution
- early pathway lock-in
- continuous clocking
- partial advancement
- forced resolution of delays
- Schema 2 automation and parallelization (reduces expected durations before clocks are set)

---

## Summary Principle

> Delays are permitted. Indefinite delays are not.

Every delay must:

- be classified
- be identified as a Schema 2 process problem or a Schema 1 legal constraint
- be visible
- be time-bounded
- resolve through a defined pathway

Regulatory process becomes:

> a deterministic system with bounded execution time
rather than
> an open-ended constraint on industrial deployment

Schema 1 constraints are real. They are documented, routed to the reform pipeline, and do not block the entire project.
Schema 2 constraints are fixable. They are resolved through RMC coordination and DoDA automation, not through legislation.

---

## Known Gaps — Pending Rewrite

*The following gaps are documented for the next version of this document, to be addressed after labor system and industrial siting compact are formalized.*

**Gap 1 — Labor pipeline integration.**
Shot clock stages currently govern regulatory and permitting timelines only. The relationship between permitting stage completion and workforce readiness milestones is not yet defined. The next version should clarify whether labor readiness thresholds create blocking conditions or run as a parallel track.

**Gap 2 — Siting compact interaction.**
The industrial siting compact will define how corridor-level coordination integrates with surrounding communities and infrastructure systems. The next version should clarify where shot clock authority applies and where siting compact coordination takes precedence.
