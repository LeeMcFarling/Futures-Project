---
id: principal-budget-autonomy-counterfactual
title: Principal Budget Autonomy — Counterfactual Detection Examples
sidebar_label: Budget Autonomy Counterfactuals
sidebar_position: 9
slug: /education/principal-budget-counterfactual
domain: Education
subdomain: K12_Reform
policy_type: Companion Walkthrough
status: Draft
phase: 2
version: 0.1
author: Futures Project
dependencies:
  - principal-budget-autonomy-pilot
  - principal-budget-autonomy-walkthrough
  - immutable-government-ledger
  - government-outflow-integrity-framework
  - des-trigger-thresholds-and-intervention-protocol
tags:
  - education
  - school-governance
  - budget-autonomy
  - fraud-detection
  - walkthrough
  - counterfactual
last_updated: 2026-04-05
---

## Purpose

The Carmen walkthrough shows what the principal budget autonomy system looks
like when it works as designed: a competent principal identifies a problem,
makes a legitimate spending decision quickly, and students benefit. The
ledger records it. The fraud detection layer clears it. DES validates the
outcome. The system learns.

This document shows what the system looks like when something is wrong. Two
scenarios — one that generates an immediate flag, one that surfaces over time
— illustrate how the triangulation model catches misuse through financial
signals, activity patterns, and outcome divergence. Neither scenario requires
catching a principal in the act. Both rely on the permanent record and the
causal structure of the system itself.

The core insight is simple: real interventions leave traces in learning.
Fraudulent or non-performing ones do not. The system is built to see the
difference.

---

## How Fraud Detection Works in This System

Before the scenarios, it is worth naming the three layers the system
triangulates across.

The **financial layer** tracks every transaction through SSI-attributed UPI
payments recorded on the immutable ledger. It compares each transaction
against peer benchmarks, vendor history, timing patterns, and spending
concentration. Anomalies here generate immediate flags.

The **activity layer** tracks vendor presence and interaction patterns across
the system. A legitimate specialist contractor who works with multiple schools
generates a cross-system activity record. A vendor that appears in one
program's ledger, collects payment, and has no presence anywhere else in
the system generates a different pattern.

The **outcome layer** tracks student competency trajectories through spine
telemetry, read by DES continuously. A legitimate intervention produces a
causal footprint — a measurable change in trajectory following a defined
temporal sequence. Spending that produces no corresponding outcome effect,
especially when repeated, is a different kind of signal.

Fraud must survive scrutiny from all three layers. The permanent ledger means
it must survive that scrutiny indefinitely, not just at the moment of
transaction. And because detection capability improves over time while the
record never changes, patterns that are invisible today may be identifiable
next year.

---

## Scenario 1 — Immediate Detection

### The Setup

Marcus is the principal of Lakeview Arts Program on the same co-location
campus as Eastbrook. He has been in the role for eighteen months. His program
has a smaller discretionary budget than Carmen's — approximately $180,000
for the year — and his stated operational plan priorities are arts
infrastructure, guest artist residencies, and student showcase events.

In the third week of November — the same week Carmen is arranging the
specialist engagement for her sixth-grade cohort — Marcus initiates a payment
of $22,000 to a vendor listed as "Educational Resource Partners LLC" for
what his operational notes describe as "curriculum development services."

### What the Financial Layer Sees

Within hours of the transaction, the fraud detection model processes the
ledger record. Several signals converge.

The vendor's SSI credential is new to the system. Educational Resource
Partners LLC has no prior transaction history with any school program on
any campus in the network. A $22,000 first transaction with a vendor that
has no system presence is an anomaly relative to peer benchmarks — comparable
programs initiating new vendor relationships typically start with smaller
engagements.

The amount represents approximately 12% of Marcus's total annual discretionary
budget in a single transaction in November, well ahead of the periods when
showcase events and residencies typically generate large expenditures. The
timing is inconsistent with the operational plan priorities he filed in
September.

The payment structure is unusual. The full $22,000 settles in a single
transaction rather than in milestones consistent with a curriculum development
engagement. Standard service contracts of this type typically involve phased
payment tied to deliverables.

Three anomaly signals — new vendor with no system presence, large single
payment inconsistent with operational plan timing, and unusual payment
structure — combine above the composite threshold. A flag is generated and
routed to the human investigation queue.

### What the Activity Layer Adds

While the flag is being routed, the activity layer processes the vendor's
SSI credential against the cross-system interaction record. Educational
Resource Partners LLC has no logged interactions with any other educational
institution. No other schools have engaged them. No professional networks
connect their credential to recognized educational service providers. The
vendor exists in the system only as a payment recipient.

A legitimate specialist who provides curriculum development services to
schools typically has a history of interactions — other programs they have
worked with, professional relationships that are visible in the system's
activity patterns. The absence of any such history does not prove fraud, but
it deepens the anomaly signal considerably.

### The Investigation

An investigator receives the flagged record within two business days. They
contact Marcus through a documented inquiry process, requesting the contract
documentation, a description of the deliverables, and the basis for selecting
this vendor. Marcus provides a one-page description of the services and a
contract signed by himself and the vendor.

The investigator requests a deliverable — a curriculum document, a session
plan, any output attributable to $22,000 in curriculum development services.
Nothing is produced that could not have been generated without a vendor
engagement. The vendor's SSI credential resolves to a recently formed LLC
with no public presence, no professional history, and no other clients.

The investigation concludes that the transaction is not consistent with
legitimate curriculum development services. The determination is referred
for recovery and appropriate administrative action. The case enters the fraud
detection model's training pipeline as a confirmed fraud case. Every future
transaction with similar patterns — new vendor, large first payment, single-
settlement structure, no system activity history — is detected more reliably
as a result.

Marcus loses access to the budget autonomy program. His discretionary budget
reverts to standard categorical controls pending the outcome of the
administrative process.

### What the Ledger Preserved

The transaction is permanent in the immutable ledger. The investigation
documentation is appended as a correction record referencing the original
transaction. The confirmation of fraud is permanently associated with the
original ledger entry. The vendor's SSI credential is flagged in the activity
layer.

If Marcus had waited — if the investigation had not occurred in November but
had been triggered by a model improvement two years later — the record would
still be there, unaltered, carrying the same evidentiary weight. The risk of
exposure did not decay. It was always going to be as high next year as it
was the day after the transaction.

---

## Scenario 2 — Latent Detection

### The Setup

This scenario is more subtle — and more important, because it represents
the failure mode that front-door friction cannot catch and that most
accountability systems miss entirely.

Diane is the principal of Westfield STEM Program, a different campus in the
same regional network. She has been in her role for four years and has a
reputation as a capable administrator. Her program produces solid DES outcome
signals — not exceptional, but consistently meeting expected trajectories.
Her financial records over three years show no immediate anomaly flags. She
has used her discretionary budget on a range of services, all within peer
benchmarks, all with vendors that have reasonable system activity histories.

In her second year under the autonomy pilot, Diane begins allocating
approximately $30,000 annually — roughly 15% of her discretionary budget —
to a professional development firm, "Learning Horizons Consulting," for what
she describes as facilitator coaching and instructional design support.

Learning Horizons has a plausible system history. They have worked with three
other schools in the network, their fees are within benchmark ranges, and
their payment structures are standard. The financial layer generates no flag.
The activity layer shows normal patterns. Year two passes without incident.

Year three shows the same allocation. Year four the same.

### What the Outcome Layer Eventually Sees

In year four, DES's system-level analysis identifies a pattern. Westfield
STEM Program has allocated approximately $120,000 to facilitator coaching
and instructional design over three years. The program's outcome trajectories
— delta mastery, retention, transfer — have remained flat relative to the
expected trajectory for comparable programs, and have not improved relative
to programs that did not make similar investments.

This is not immediately a fraud signal. Some professional development spending
produces weak outcomes. That is a normal failure mode, not a criminal one.
DES generates a demand-outcome diagnostic request: the program's spending
on instructional support is not producing visible trajectory improvement.
Diane is asked to account for the pattern.

### What the Activity Layer Then Surfaces

As part of the investigation triggered by the diagnostic request, the
cross-system analysis of Learning Horizons' activity record is reviewed in
detail. Over four years of system presence, the firm has collected
approximately $340,000 across four school programs. In three of those
programs, the engagement pattern is similar to Westfield's: multi-year
annual allocations, standard payment structures, no deliverables logged in
the system beyond session attendance records.

None of the three programs show trajectory improvement attributable to the
period of the consulting engagement. The firm has collected $340,000 across
four programs over four years and produced no measurable outcome effect in
any of them.

The activity layer now shows something that was invisible at the transaction
level: a vendor with system presence but no causal footprint in learning
outcomes, operating across multiple programs at material scale.

### The Investigation

The investigation that follows is not about a single transaction. It is about
a pattern across time, across programs, and across a vendor relationship that
looks legitimate at the transaction level and reveals itself only through
the combination of financial history and outcome divergence.

The investigation examines what Learning Horizons actually delivers. Session
attendance records exist. Invoices exist. The financial trail is clean. But
the sessions themselves — when reviewed — are generic, non-specific to the
programs engaging them, and disconnected from the competency domains where
the spine's trajectory data shows the greatest gaps.

The investigation distinguishes between several possible conclusions, and
the distinction matters enormously for what happens next. Diane may have
made a genuine but poor judgment call — trusting a vendor who delivered
sessions that sounded reasonable but produced nothing measurable. That is
an accountability problem, not a criminal one. The appropriate response is
constraint of future discretionary authority, required redesign of her
professional development approach, and a documented record of the pattern.
Alternatively, the investigation may find evidence of a structured arrangement
in which fees were paid for services not genuinely delivered — a kickback
arrangement, a personal relationship with the vendor, or deliberate misuse
of public funds. That is a criminal matter and is handled accordingly.

The system's immediate response is the same regardless of which conclusion
the investigation reaches: the spending pattern warrants scrutiny, the
program's discretionary authority is constrained pending the investigation's
conclusion, and the students enrolled in Westfield are protected from
continued allocation of funds to an intervention that is not helping them.
What differs is the endpoint — administrative consequence versus criminal
referral — and that determination is made by human investigators, not by
the automated detection layer.

This distinction is important for principals operating in good faith. The
system is not designed to criminalize poor decisions. It is designed to catch
patterns that harm students and misuse public funds, and to respond
proportionately to what the investigation actually finds. A principal who
tries something that doesn't work, documents their reasoning, and adjusts
when the outcome data shows it isn't working is not at risk from this system.
A principal who repeatedly allocates funds to the same non-performing
relationship without adjustment, especially when the outcome data is clear,
generates a pattern the system is built to surface — and the investigation
determines whether that pattern reflects bad judgment or bad faith.

Whether the outcome is confirmed fraud, confirmed ineffectiveness, or
something in between — the spending pattern enters the detection model's
training pipeline. Future programs that allocate large fractions of their
discretionary budget to vendors with no measurable outcome effect across
multiple programs will be identified earlier.

### What the System Learned

The Westfield scenario does not generate a fraud conviction. It generates
something equally important: evidence that a particular vendor relationship
produces no educational value across multiple engagements. That evidence
changes how the system evaluates similar patterns in the future.

It also demonstrates something about the system's fundamental property:
the absence of outcome improvement is not, by itself, evidence of misuse —
some interventions fail, and that is normal. But the absence of outcome
improvement that persists across repeated allocations, combined with a vendor
activity pattern that shows the same result across multiple programs, becomes
a signal worth acting on. The threshold is not one failure. It is a pattern
that distinguishes legitimate but ineffective spending from something that
warrants investigation.

---

## The Triangulation Model in Summary

The two scenarios illustrate the same core architecture operating at
different timescales.

In Scenario 1, the financial and activity layers identify the anomaly
immediately. A new vendor with no system history, a large single payment,
and a timing inconsistency with the operational plan combine to generate
a flag that routes to human investigation within days. The investigation
surfaces the fraud quickly. The permanent ledger preserves the evidence
regardless of when the investigation happens.

In Scenario 2, the financial layer never flags anything. The activity layer
shows a plausible vendor. The anomaly only becomes visible when the outcome
layer's continuous measurement is combined with the financial history over
multiple years — spending that produces no causal footprint in learning,
repeated at scale, across multiple programs, from the same vendor.

Both cases require the same infrastructure: a permanent, attributable
financial record; a cross-system activity layer that tracks vendor patterns
beyond individual transactions; and a continuous outcome measurement system
that can identify the absence of expected effects. None of those three
components alone is sufficient. Together, they create a detection system
that improves over time and that fraud must survive indefinitely, not just
at the moment of transaction.

Real interventions leave traces in learning. Fraudulent and non-performing
ones do not. The system is built to see the difference — immediately when
the anomaly is visible, and eventually when it only becomes visible through
the accumulation of evidence that a permanent record makes possible.

---

## What This Means for Principals Operating in Good Faith

The counterfactual scenarios are designed to show what the system catches.
They are equally designed to show what it does not catch and should not catch.

Carmen's specialist engagement in the Eastbrook walkthrough produced a
measurable trajectory improvement for eleven students. That outcome is the
causal footprint that distinguishes her decision from Scenario 1's fraudulent
vendor payment and Scenario 2's ineffective consulting relationship. The
system validated her decision not because she followed a prescribed process
but because the students actually learned.

A principal who makes an unusual spending decision — one that doesn't fit
the standard pattern, that uses a vendor nobody else in the system has worked
with, that doesn't show up in DES trajectory data for several months — is
not at risk from this system as long as they are genuinely trying to improve
outcomes for students. The record of their decision exists permanently, and
when the outcome data arrives, it either validates the decision or it doesn't.
Validation through outcomes is the standard, not conformity to conventional
spending patterns.

This is the trade the autonomy model offers and the counterfactual scenarios
make concrete: more discretion, permanent transparency, outcome-based
validation. A principal who uses their discretion to genuinely serve students
has nothing to fear from a system that measures whether students are learning.
A principal who uses their discretion for anything else cannot hide from a
record that does not change and detection that only improves.
