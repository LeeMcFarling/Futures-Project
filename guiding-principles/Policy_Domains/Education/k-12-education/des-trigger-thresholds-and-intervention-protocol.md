---
id: des-trigger-thresholds-and-intervention-protocol
title: DES Trigger Thresholds & Intervention Protocol
sidebar_label: DES Triggers
sidebar_position: 4
slug: /education/des-trigger-thresholds
domain: Education
subdomain: K12_Reform
policy_type: Standards and Accountability Framework
status: Draft
phase: 3
version: 0.4
author: Futures Project
dependencies:
  - education-reform-overview
  - national-competency-framework
  - department-of-education-standards-reform
  - personalized-education-reform
  - principal-budget-autonomy-pilot
related_initiatives:
  - book-recommendation-pilot
  - book-rating-system
  - student-based-funding-and-campus-colocation
tags:
  - education
  - standards
  - accountability
  - mastery-learning
  - intervention
  - evaluation
  - causal-inference
last_updated: 2026-04-05
---

## Purpose

This document defines the rules by which the Department of Education Standards
identifies meaningful deviations in school and program performance, determines
when and how to respond, and distinguishes signals that warrant action from
noise that does not.

DES does not manage schools. It monitors validated outcome signals and
intervenes only when pre-specified conditions are met. The framework is built
to preserve the experimentation that a decentralized system depends on while
preventing low-quality or extractive programs from persisting or scaling. The
goal is calibration, not control — a system that catches genuine failure early,
recognizes genuine success and propagates it, and stays out of the way of
programs that are doing their job.

---

## The Measurement Principle

DES evaluates performance derivatives, not static performance levels. The
core question is not whether a school is producing high absolute outcomes —
it is whether learning is materializing at the expected rate given where each
student started.

This distinction matters enormously in practice, and it exposes a failure mode
that the old system was structurally incapable of detecting. Under a GPA-based
model, a student who moves from a rigorous school to a school with lax grading
standards might see their average rise from a 3.0 to a 4.0 while their actual
learning trajectory flattens or declines. The grade signal and the learning
signal point in opposite directions, and nothing in the old system catches the
divergence. Under the spine model, measurement is constant across environments.
When that student moves schools, DES continues reading their competency
trajectory from the same standardized infrastructure. The grade change is
invisible to DES. The trajectory change is not.

Intervention is triggered by material, sustained deviation from expected
trajectory — not by rankings, not by comparisons to elite programs, not by
single-period fluctuations that may reflect noise rather than genuine
performance change. Material deviation is defined as statistically significant
divergence from expected trajectory beyond calibrated confidence intervals,
with thresholds published, versioned, and updated by DES through formal
revision processes. The definition is quantitative, not discretionary — DES
cannot arbitrarily decide what constitutes sufficient deviation, because the
threshold is public and its changes are auditable.

---

## What DES Measures

Each student is evaluated against an expected learning trajectory derived
from their prior mastery state, matched cohort comparisons, historical program
distributions, and retention and transfer performance. The trajectory is the
baseline. Deviation from it is the signal.

The primary outcome signals are delta mastery — the rate at which students
are developing new competencies relative to expectation — retention of
competencies over time, transfer of competencies to novel contexts, and
variance across student subgroups within a program. That last signal matters
because a program that produces strong average outcomes by concentrating
benefits on advantaged students while leaving others behind is a different
kind of failure than one producing uniformly weak outcomes, and the system
needs to detect both.

Secondary signals — attendance, engagement, program demand — inform diagnosis
but do not independently trigger intervention. A school with declining
attendance that is producing strong learning trajectories is a different
situation from one with declining attendance and degrading outcomes. Secondary
signals provide context; primary signals determine action.

Intervention decisions prioritize patterns that are both statistically robust
and directionally consistent across multiple signals. A program that shows
weakening delta mastery, declining retention, and increasing subgroup variance
simultaneously is producing a different quality of signal than one that shows
weakness on a single metric while holding steady on others. The composite
requirement is the primary defense against reacting to noise.

---

## System Learning Through Natural Variation

The portability of the competency record creates something the old system
could not produce: a continuous, real-world causal inference engine embedded
in the system's normal operation.

Because competency measurement is standardized and remains constant as
students move between schools, programs, and specializations, DES observes
comparable learning trajectories across different environments without needing
to design separate experiments. When a student transfers from one program to
another, DES has a before-and-after record under a constant measurement
framework. When a cohort of students enters a new specialization program at
a co-location campus, DES can compare their subsequent trajectories to matched
peers who did not. When a school implements a new facilitation approach, the
spine continues measuring the same competency signals, and the effect of the
change becomes visible in the data.

This structure enables formal causal inference methods as part of routine
system operation. Difference-in-differences analysis becomes possible when
students move between programs while measurement holds constant —  the
pre-transition trajectory is the counterfactual, and the post-transition
deviation is the effect estimate. Regression discontinuity designs emerge
naturally at program entry thresholds, admission cutoffs, and intervention
trigger points — students just above and just below a boundary are comparable
in expectation, and their diverging trajectories after the boundary identify
the effect of the program or intervention. Matched cohort analysis is possible
at scale because the standardized record creates a common comparison currency
across every student in the system.

The system does not require separate experimental programs to learn what works.
It generates causal knowledge as a byproduct of its own operation. DES's
system learning function is therefore not just the accumulation of descriptive
evidence about what programs are performing well — it is the ongoing production
of credible estimates of what educational interventions are actually causing
improved outcomes, which interventions are correlated with outcomes but not
causing them, and which apparent successes are artifacts of favorable intake
rather than genuine program effect.

This is what separates outcome validation from genuine system learning. The
trigger and intervention framework catches failure and rewards success. The
causal inference layer explains why — and that explanation is what allows
successful models to be replicated with fidelity rather than cargo-culted in
ways that preserve the surface features while losing the mechanism.

---

## Cohort Adjustment

All evaluations are relative to comparable baselines. DES adjusts for prior
mastery distribution, age band, specialization type, learning accommodations,
language context, and access constraints before drawing any conclusions about
program performance. The purpose of adjustment is to isolate program effect —
what the school is contributing to student development — from the characteristics
students bring with them.

Cohort adjustment is not a mechanism for excusing poor outcomes. It is a
mechanism for measuring the right thing. A program that consistently
underperforms its adjusted cohort is failing its students regardless of whether
those students face significant challenges. The adjustment makes that failure
visible rather than masking it behind favorable intake characteristics — or
obscuring genuine success behind unfavorable ones.

---

## Trigger Classes

Four categories of signal can activate DES response, each with different
implications and different response logic.

**Performance degradation** is the primary negative trigger. It activates
when delta mastery falls materially below expected trajectory, when retention
declines across multiple measurement periods, when transfer performance
weakens, or when outcome variance increases in ways that indicate uneven
benefit distribution within a program. This trigger carries the highest
intervention authority because it represents the clearest evidence that
students are not learning what the program is supposed to be producing.

**Demand-outcome divergence** activates in two directions with opposite
implications. When a program is growing in enrollment while outcomes are flat
or declining, the system is rewarding popularity rather than learning — a
market distortion that, if left unchecked, concentrates students in programs
that are not serving them. This is treated as a system risk and triggers
constraint logic. When outcomes are strong but enrollment is declining, the
program may be underrecognized, poorly communicated, or facing access barriers
rather than suffering from genuine preference failure. This direction triggers
diagnosis and potential scaling support rather than constraint.

**Anomalous performance** triggers structured review in both directions. A
program that significantly outperforms comparable cohorts, that shows rapid
improvement beyond expected bounds, or that produces unexplained performance
volatility warrants investigation regardless of whether the deviation is
positive or negative. Positive outliers enter the positive intervention
pathway — DES investigates what is producing the result, documents it, and
supports propagation. Negative outliers enter failure-mode investigation.
Both are treated with equal seriousness. A system that only investigates
failure and treats success as self-managing is leaving its most important
learning opportunity unused.

**System-level drift** activates when average delta mastery declines across
regions, when inequality between campuses increases, when demand concentrates
in low-outcome programs system-wide, or when retention and transfer degrade
across the system rather than in isolated programs. This trigger is
categorically different from the others — it indicates a problem with the
standards, the incentives, or the measurement framework itself rather than
with individual programs. The response is standards or incentive redesign,
not school-level intervention.

---

## Persistence Requirements

A single period of deviation does not trigger intervention. The system is
operating on real outcome data that contains genuine noise — a program that
has one weak measurement period may be experiencing a legitimate anomaly
rather than a genuine performance change, and responding to every fluctuation
would produce exactly the kind of instability and risk-aversion that destroys
the experimentation the system is designed to enable.

A single-period deviation flags the program for internal monitoring — DES
watches more closely, looks for corroborating signals, and prepares to act
if the pattern continues. Two to three periods of sustained deviation activate
a diagnostic request, asking the school to account for the pattern it is
producing. Persistent deviation across multiple periods activates formal
intervention. The persistence requirement is the primary defense against
over-intervention, and it must be calibrated carefully — too short and the
system becomes reactive and destabilizing, too long and genuine failure
compounds for years before the system responds.

---

## Intervention Tiers

The intervention system is tiered to match response intensity to signal
severity, and to give programs the opportunity to self-correct before
escalation. Negative and positive intervention pathways are deliberately
parallel in structure — success is treated with the same formal seriousness
as failure, because replication without understanding the causal mechanism
is as wasteful as failure without diagnosis.

**Tier 1 — Passive Flag.** Internal monitoring only. No school-facing action.
DES is watching; the school does not yet know it is being watched more closely.
This tier exists to accumulate signal before acting on it.

**Tier 2 — Diagnostic Request.** The school is asked to explain the pattern
DES is observing. This is not an accusation — it is a structured request for
context. The school may have information that explains the deviation: a cohort
with unusual characteristics, a program transition in progress, an external
event affecting outcomes. The diagnostic request distinguishes between programs
that understand what is happening and are managing it and programs that cannot
explain their own performance.

**Tier 3 — Targeted Review.** DES deploys field personnel to the program on
a time-bounded, hypothesis-driven basis. The deployment has a defined question
it is trying to answer and a defined endpoint. Personnel have observation
authority but no operational authority — they investigate; they do not manage.
The deployment produces a formal output that becomes the basis for any further
action.

**Tier 4 — Constraint and Probation.** Enrollment caps limit the program's
ability to expand while underperforming. Required redesign establishes a
specific improvement plan with defined milestones. Expansion rights are
suspended until the program demonstrates recovery. This tier is designed to
protect students from being enrolled in a program that the evidence indicates
is not serving them, while giving the program a structured path to recovery
rather than immediate termination.

**Tier 5 — Sunset and Decertification.** The program loses DES certification,
loses funding eligibility, and student transition to alternative programs is
required and supported. This is not a failure of the intervention framework —
it is the framework working. Programs that cannot recover under Tier 4
conditions are not serving students, and the funding and enrollment they
consume should flow to programs that do. Student transition is managed, not
abrupt.

---

## The Positive Intervention Pathway

Programs that significantly outperform comparable cohorts enter a structured
positive intervention pathway with defined eligibility thresholds and scaling
support criteria, parallel in formality to the negative intervention tiers.
Reference campus designation triggers formal study and documentation of what
is producing the result — using the causal inference methods available through
the system's natural variation — replication support for programs seeking to
adopt the model, and standards integration review to determine whether the
practices driving the performance should inform the broader framework.

The causal inference layer is particularly important here. Replicating a
program's surface features without understanding the mechanism that produces
its outcomes is unlikely to transfer the outcomes. DES's positive intervention
pathway therefore emphasizes identifying *why* a program is outperforming —
which design elements, which facilitation practices, which structural features
are causally responsible — before supporting replication. This is what
distinguishes propagation that raises system performance from cargo-culting
that produces apparent adoption without real effect.

---

## Demand and the Limits of Market Signal

Demand is a useful signal, but it requires careful interpretation. Low demand
for a program is not automatically evidence of failure, and high demand is
not automatically evidence of success.

When a program has low enrollment, DES diagnoses the cause before drawing
conclusions. The program may face access constraints — geographic,
informational, or economic barriers that limit who can reach it. It may have
a communication problem — genuine quality that is not legible to families
making enrollment decisions. It may have a design problem — real barriers to
engagement that are correctable. Or it may reflect genuine preference: families
have evaluated the program and chosen alternatives. Only confirmed preference
failure — where access, information, and design explanations have been ruled
out — justifies contraction based on low demand alone.

High demand is treated with equal caution. A program that is growing rapidly
without corresponding outcome improvement is producing popularity, not
learning. The student-based funding model means that enrollment growth without
outcome growth concentrates resources in a program that is not converting them
into student capability. High demand does not justify scaling. Strong outcomes
do.

---

## The Spine and Specialization Boundary

The trigger framework applies differently to the spine layer and the
specialization layer, and the distinction matters.

The spine — the core competency development that occupies approximately two
hours of each school day — is governed strictly by outcome signals and
protected from demand distortion. No program, regardless of its popularity
or its specialization quality, is permitted to degrade spine mastery
trajectories. The trigger framework monitors this boundary continuously.
A specialization program that produces exceptional outcomes in its domain
but suppresses spine competency development has failed on the terms that
matter most, regardless of how much students or families value what it offers.

The specialization layer above the spine is more permissive. Demand informs
what programs explore. Outcomes determine which programs survive and scale.
A specialization program that students and families find compelling, that
produces strong domain outcomes, and that leaves spine trajectories intact
is doing exactly what the system is designed to enable.

---

## Teacher Attribution Safeguard

DES evaluates outcomes at the program and system level. Spine telemetry is
not used as a mechanism for direct punitive individual teacher evaluation.

This boundary matters for two reasons. The first is methodological: student
outcome trajectories reflect the combined effect of the spine, the facilitation
quality, the student's prior state, the program's specialization, and factors
outside school entirely. Attributing trajectory outcomes to an individual
teacher requires causal isolation that program-level data cannot support
without significant additional analysis. The second is behavioral: a system
that uses student trajectories as direct teacher performance metrics creates
defensive teaching behavior — facilitators optimizing for their individual
DES signal rather than for student development. The teacher reskilling
framework establishes separate, facilitation-specific evaluation criteria
that operate alongside but independently of program-level DES outcomes.

---

## Governance and Transparency

The trigger logic is versioned, auditable, public at the framework level, and
protected from ad hoc override. All trigger criteria, threshold definitions,
and intervention procedures are published in both technical documentation and
plain-language summaries accessible to schools, families, and the public.
The expert layer and the public layer must both exist — a system that is
technically transparent but practically opaque has not achieved the
accountability it claims.

Threshold changes require formal revision processes. DES cannot quietly adjust
what triggers intervention or what constitutes sufficient deviation without
that change being documented, reviewed, and publicly recorded. A trigger
system that can be modified without visibility is discretionary judgment with
a technical facade. Field deployments produce formal outputs. Intervention
decisions are documented with the evidence that supported them. Decertification
decisions are published with the trajectory data that preceded them.

---

## Failure Modes

Over-intervention is the failure mode that destroys the system's value
proposition. If triggers fire on noise, if persistence requirements are
inadequate, if cohort adjustment is insufficient, schools learn that deviation
from the mean is dangerous regardless of whether students are learning. The
result is convergence toward safe mediocrity. The persistence requirements,
composite trigger logic, and cohort adjustment rules are all defenses against
this failure, and they must be treated as non-negotiable even under political
pressure to respond more aggressively to perceived underperformance.

Under-detection is the opposite failure mode. If thresholds are set too high,
if persistence requirements are too long, if the measurement framework is too
coarse to catch genuine failure early, programs can persist for years producing
inadequate outcomes before the trigger system responds. The cost is borne by
the students enrolled during the detection gap. Calibration of threshold
sensitivity is a continuous responsibility, informed by the causal inference
layer's ongoing analysis of what the system is and is not catching.

Evaluator gaming emerges when schools understand the trigger logic well enough
to optimize against it rather than for student outcomes. The composite trigger
design, which requires deviation across multiple signals rather than a single
metric, and the transfer-based validation model, which resists optimization
against any specific format, are the primary defenses. Neither is sufficient
indefinitely. DES's responsibility to evolve the framework in response to
observed gaming behavior is a permanent operational requirement — and the
causal inference layer is the mechanism that makes gaming detectable, because
programs that are gaming metrics rather than producing outcomes will eventually
show divergence between their measured signals and the transfer and retention
outcomes that are hardest to fake.

---

## Conclusion

A decentralized education system requires explicit rules for when to observe,
when to intervene, when to constrain, and when to scale. Without those rules,
accountability is discretionary — which means it is political, inconsistent,
and ultimately not credible to the schools and families operating within it.

This protocol makes those rules explicit. But it does something beyond
accountability: because measurement is constant and portable while students
and programs vary, the system generates causal knowledge about what works as
a byproduct of its own operation. DES does not just evaluate the system. It
learns from it — continuously, rigorously, and in ways that allow successful
models to be understood deeply enough to be replicated faithfully.

That combination — calibrated intervention rules and embedded causal learning
— is what makes this a governance system capable of improving over time rather
than one that merely holds the line.
