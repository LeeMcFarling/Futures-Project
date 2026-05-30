---
id: grant-approval-reform
title: Grant Approval Reform
sidebar_label: Grant Approval Reform
sidebar_position: 4
slug: /institutional-modernization/grant-approval-reform
domain: Institutional_Modernization
subdomain: Evidence_and_Accountability
policy_type: Institutional Design
status: draft
version: 0.2
author: Futures Project
last_updated: 2026-05-29
dependencies:
  - department-of-data-and-accountability
  - immutable-government-ledger
  - public-capital-authority
  - upi-privacy-preserving-payment-rail
  - research-integrity-and-methodological-transparency-framework
  - institutional-modernization-corps
  - automated-research-compliance-infrastructure
related_initiatives:
  - supplement-integrity-evidence-and-claims-reform
  - food-nutrition-and-metabolic-research-track
  - pharmaceutical-clinical-trial-infrastructure
  - regional-wage-modernization-pilot
  - heta-revised-charter
non_goals:
  - replacing peer review with algorithmic selection
  - eliminating agency subject-matter authority
  - mandating uniform grant structures across all domains
  - creating a single government research platform
tags:
  - grants
  - public-administration
  - research-funding
  - fraud-detection
  - peer-review
  - adaptive-portfolios
  - public-ledger
  - doda
  - imc
  - replication
  - frontier-research
description: >
  Unbundles the federal grant system into five distinct functions — admissibility
  review, portfolio allocation, financial instrumentation, audit and enforcement,
  and outcome learning — to fund serious work, tolerate legitimate uncertainty,
  reduce procedural friction, and detect fraud earlier without replacing human
  judgment with algorithmic selection.
changelog:
  - v0.2: Full pass. Standardized frontmatter to platform schema. Updated domain
    to Institutional_Modernization. Corrected dependency IDs (RIF replaces old
    research-integrity-and-audit-framework reference; UPI ID corrected). Added
    IMC and automated-research-compliance-infrastructure as dependencies. Updated
    DoDA institutional role to reflect observability layer doctrine. Clarified
    IMC as builder of financial instrumentation infrastructure. Softened
    epsilon-greedy framing for legislative audience. Added RIF integration
    paragraph. Added Evidence Communication connection. Added two-sentence
    Political Argument strengthener.
---

# Grant Approval Reform

## Purpose

The federal grant system should fund serious work, tolerate legitimate uncertainty,
reduce procedural friction, and detect fraud earlier. Today, grant approval asks one
process to do too many jobs at once. Review panels are expected to judge scientific
or program merit, prevent fraud, allocate public resources, manage institutional
risk, and indirectly shape national priorities. The result is a system that is slow,
conservative, paperwork-heavy, and biased toward applicants who already know how to
navigate the bureaucracy.

Grant Approval Reform separates these functions. Human reviewers determine
admissibility. Portfolio rules determine allocation. Delayed outcome measurement
informs future funding weights. Instrumented financial accounts protect public money.
Auditors investigate anomalies and fraud. The goal is not to replace judgment with
algorithms. The goal is to put judgment where it belongs and automate the compliance
work that should not require endless paperwork.

This reform is especially important for research agencies — NIH, NSF, ARPA-H, DOE,
and other grantmaking bodies. The same architecture applies across public-purpose
grants: health pilots, infrastructure demonstrations, education experiments,
manufacturing innovation, climate resilience, and local implementation programs.

---

## Core Problem

Federal grants confuse caution with rigor. The current system rewards applicants
who can write bureaucratically legible proposals, satisfy conventional expectations,
and pass through multiple procedural gates. That does not mean the work is
high-value. It often means the work is familiar.

Fraud prevention is handled through documentation burdens placed on everyone rather
than through modern financial telemetry, anomaly detection, and targeted audit
systems. Honest applicants experience friction. Sophisticated bad actors exploit
gaps in oversight.

The system is simultaneously too conservative toward uncertain but legitimate work,
too burdensome for honest grantees, and not strong enough against actual fraud.

---

## Design Principle

Grant approval should be unbundled into five distinct functions:

**Admissibility review** determines whether the applicant, institution, method,
budget, ethics, and proposed work are real, coherent, and eligible.

**Portfolio allocation** determines how much funding goes to core work, frontier
exploration, replication, validation, digital infrastructure, and other strategic
categories.

**Financial instrumentation** ensures that grant funds move through accountable
accounts, approved categories, tagged transactions, and immutable logs.

**Audit and enforcement** investigates fraud, misuse, conflicts of interest,
fabricated credentials, impossible methods, and spending inconsistent with the
approved work.

**Outcome learning** uses delayed composite metrics to improve future allocation
without reducing public-purpose work to a single metric.

The core doctrine:

**Peer review filters bullshit. It does not pick destiny.**

---

## Admissibility Review

Human review remains essential, but its role should be narrower and clearer. The
admissibility layer asks whether a proposal deserves entry into the fundable pool.
It should not be forced to predict the full future value of the work.

Reviewers certify that the applicant is real, the institution or fiscal sponsor is
legitimate, the proposed work is coherent, the claim is testable or operationally
evaluable, the budget plausibly maps to the work plan, ethics and safety requirements
are satisfied, and the proposal is not obvious fraud, pseudo-science, credential
fabrication, vendor self-dealing, or impossible methodology.

This shifts peer review from "pick the winners" to "protect the gate." Reviewers
remain a human filter against nonsense, but they do not become a veto point against
unusual, interdisciplinary, frontier, or early-stage ideas.

This matters especially in science funding. Many valuable breakthroughs look strange
before they become obvious. A grant system that only funds what reviewers already
recognize will structurally underfund the frontier.

---

## Portfolio Allocation

Once proposals clear admissibility review, funding is allocated through explicit
portfolio rules. Agencies should not pretend every grant competes in a single
universal merit queue. Different grant types have different risk profiles, time
horizons, and public purposes.

### Core Merit Funding

The main funding channel for conventionally strong proposals — clear methods, strong
preliminary evidence, credible teams, well-understood public value.

### Frontier Exploration Funding

A protected share funds high-variance work that is too early, interdisciplinary,
unconventional, or paradigm-challenging to succeed under ordinary review.

The frontier share should not be symbolic. A 0.1 percent allocation is a safety
valve, not a frontier strategy. Congress should establish a statutory exploration
share large enough to alter institutional behavior. For research agencies, a
plausible starting range is 10 to 20 percent of relevant extramural research
funding, adjusted by agency mission and field maturity. Frontier proposals still
pass admissibility review — they simply do not compete against safer, incremental
proposals on the same scoring rubric.

### Replication and Validation Funding

A protected share funds replication, validation, benchmark testing, negative-result
publication, reproducibility checks, clinical validation, implementation validation,
and stress-testing of influential findings.

This prevents the system from becoming a novelty casino. Frontier science requires
a validation substrate. Public grantmaking should reward not only discovery but
truth maintenance. This bucket is the institutional mechanism that makes the
Research Integrity and Methodological Transparency Framework's replication
infrastructure doctrine operational — the RIF defines what independent replication
is and why it is necessary; this protected bucket funds it at scale.

### Digital Infrastructure and Methods Funding

A protected share funds datasets, shared equipment, lab modernization, open methods,
software tools, measurement systems, research platforms, and field-wide digital
infrastructure.

These grants may not generate publications immediately, but they raise the
productivity of entire research ecosystems. This bucket explicitly covers the
digital systems and API infrastructure that support research compliance, data
exchange, and observability — the underlying plumbing that makes scientific work
legible across institutions.

### Translation and Deployment Funding

Separate funding supports the movement from discovery to use: clinical translation,
manufacturing readiness, regulatory pathway work, field pilots, public-health
deployment, and operational scaling.

These grants are evaluated differently from basic research. The relevant questions
are feasibility, cost, adoption, safety, implementation capacity, and public value —
not scientific novelty alone.

---

## Adaptive Allocation Model

Grant allocation becomes adaptive over time. Agencies should learn which categories
of grants, institutions, methods, fields, and risk profiles produce durable public
value.

This does not mean turning research into an algorithmic contest. It means using
delayed composite outcome models to update portfolio weights — informing future
allocation across categories, not mechanically punishing every grant that did not
produce a clean short-term output.

For scientific research, relevant outcome signals may include field-normalized
citation impact, replication success, dataset reuse, method adoption, patent
quality, licensing or commercialization where relevant, clinical trial progression,
regulatory relevance, negative-result usefulness, follow-on research quality,
public-health or public-purpose contribution, training and talent development, and
institutional capacity building.

No single metric should dominate. Citations reward fashion and network effects.
Patents reward commercial strategy, not necessarily public value. Clinical impact
can take decades. Some of the most valuable grants produce tools, datasets, methods,
or failed hypotheses that prevent entire fields from wasting time. The adaptive
model scores at the portfolio level more than the individual level.

---

## Guarded Exploration

The frontier bucket uses structured exploration rather than random allocation. A
fixed exploration share is preserved among admissible proposals. Within that pool,
agencies may use weighted lotteries, rotating thematic calls, field diversity
constraints, early-career allocations, regional balancing, institutional capacity
adjustments, and strategic public-need priorities.

This prevents exploration from becoming chaos while preventing conventional review
from suffocating high-variance work.

The model explicitly protects early-career investigators, non-elite institutions,
interdisciplinary teams, unfashionable but important fields, high-burden
public-health problems, methodological work, replication and negative results, and
proposals that are plausible but not yet consensus-legible.

---

## Financial Instrumentation

Grant funding is paired with instrumented financial accountability. This is a
digital systems build, not a paperwork expansion. The Institutional Modernization
Corps builds the account infrastructure to DoDA-certified specifications. Treasury
coordinates the financial rail and ledger standards. Grantmaking agencies
administer accounts within that framework.

NIH, NSF, DOE, HHS, Treasury, and other grantmaking agencies issue grant-linked
financial accounts through approved financial institutions. Until the Universal
Payment Interface is fully operational, regulated banks serve as administrative
partners for accounts, cards, transaction controls, fraud monitoring, and payment
categorization. The bank is not the policymaker, the scientific reviewer, or the
merit adjudicator. It operates a regulated financial rail under federal rules.

Each grant account supports project-linked accounts, authorized user permissions,
grant cards, approved spend categories, vendor tagging, merchant category controls,
transaction-level metadata, budget-line mapping, immutable ledger logging, automated
anomaly detection, and audit escalation workflows.

The purpose is to instrument compliance rather than proceduralize it. Honest
grantees experience less paperwork, not more. Routine spending flows normally.
The compliance system runs in the background and escalates only when spending
patterns become unusual, risky, or inconsistent with the approved work.

---

## Immutable Ledger Logic

Every grant transaction creates a tamper-resistant record. The ledger does not
expose sensitive research details publicly — it establishes financial chain of
custody.

The ledger records which grant funded the transaction, which authorized user
initiated it, which vendor received payment, what category the transaction fell
under, which budget line it mapped to, whether it was automatically approved,
manually approved, flagged, or denied, and whether it triggered later audit review.

This creates a durable audit trail without forcing every grantee into a manual
reporting burden. The government does not need to micromanage every purchase if it
can verify the financial chain of custody after the fact.

The preregistration records required by the Research Integrity Framework flow
through the same ledger infrastructure. A pre-registered protocol is a timestamped
public record. Non-publication after enrollment closes is a detectable gap in that
record — not a private decision. The grant financial ledger and the research
compliance ledger are distinct record types on shared infrastructure, which is
what makes both the financial audit trail and the protocol-to-publication matching
pipeline operational at scale.

---

## Fraud Detection

Grant fraud detection uses the same logic common in modern financial systems:
anomaly detection, risk scoring, vendor analysis, transaction monitoring, and
human escalation.

The system flags patterns such as unusual vendor relationships, related-party
transactions, repeated split purchases, round-number invoice patterns, budget
shifts late in the project, equipment purchases inconsistent with the stated method,
payments to vendors with weak or suspicious histories, foreign transfers inconsistent
with grant terms, spending patterns that sharply diverge from comparable labs or
projects, duplicate billing across grants, high-risk subcontracting behavior, and
sudden spending surges before grant expiration.

Fraud models are calibrated before enforcement. Agencies run models in silent mode,
compare flags against auditor judgment, measure false positives and false negatives,
and publish performance summaries. Formal enforcement requires human review.

The system never becomes a punitive black box.

---

## Audit Model

Audits are risk-tiered. Most grants face light-touch monitoring. Some are selected
for random audit to preserve deterrence. Grants with suspicious financial patterns
receive targeted review. High-risk cases receive full investigation.

Auditors understand the domain they are auditing. A lab, clinic, machine shop,
field site, software team, and local government pilot do not spend money the same
way. Audit teams evaluate whether spending plausibly maps to the approved plan and
actual project progress.

The audit question is: does the financial behavior make sense given the work being
performed?

Not: can the grantee survive a paperwork obstacle course?

---

## Research Progress Review

For research grants, field auditors or technical reviewers may periodically evaluate
progress. Their role is limited. They assess whether the project exists, the team
is doing the work, the methods resemble the approved plan or an explained
adaptation, the data, equipment, personnel, and procedures are plausibly in place,
and the project is failing honestly, adapting legitimately, or behaving suspiciously.

Failure is not fraud. Frontier work often fails. The system distinguishes honest
failure from fabrication, misuse, and nonperformance.

A research grant is not punished because the hypothesis was wrong. It is punished
if the work was fake, the funds were misused, the institution lied, or the
investigators concealed material nonperformance.

---

## Delayed Composite Reward Model

Grant outcomes are evaluated on time horizons appropriate to the field and grant
type. A three-year horizon may suit some implementation pilots. A ten-year horizon
may be necessary for basic biomedical research. Some discoveries do not show their
value for twenty years.

The reward model is delayed, composite, and field-normalized.

For basic science, intermediate signals may include replication, method adoption,
dataset reuse, field influence, or strong follow-on inquiry.

For translational science: preclinical milestones, IND-enabling studies, clinical
trial progression, manufacturability, regulatory pathway clarity, or care-delivery
improvement.

For digital infrastructure grants: usage rates, cost reductions, time savings,
cross-institution access, research throughput, or downstream publication support.

For public-sector pilots: outcome improvement, implementation cost, operational
feasibility, equity effects, user uptake, and measurable public value.

The purpose is to let the grant system learn without pretending that every public
good can be measured immediately.

---

## Anti-Gaming Rules

Any metric used for funding will eventually be gamed. The reform assumes gaming
from the beginning.

Anti-gaming protections include field normalization, career-stage normalization,
institution-type adjustment, caps on single-metric influence, disclosure of
conflicts, vendor relationship transparency, random audit sampling, independent
replication, negative-result credit, model audits, public methodology reporting,
rotating review panels, and human override with written justification.

Metrics inform portfolio learning. They do not mechanically determine individual
destiny.

The system rewards durable contribution, not citation hacking, patent spam, prestige
laundering, or bureaucratic grant-writing skill.

---

## Institutional Roles

### Congress

Congress defines the statutory portfolio shares, admissibility standards,
transparency requirements, audit authorities, privacy rules, and reporting
obligations. Congress should write the exploration share into law so frontier
research cannot be quietly eliminated by administrative caution.

### Grantmaking Agencies

Agencies administer calls, manage admissibility review, issue awards, oversee
program portfolios, and coordinate with Treasury, financial intermediaries,
auditors, and DoDA. Agencies retain subject-matter responsibility.

### Department of Data and Accountability

DoDA specifies the evaluation standards, certifies the measurement architecture,
and publishes aggregate portfolio-level findings. It does not pick scientific
winners. DoDA certifies the evaluation model, audits the reward metrics, tracks
fraud-detection performance, and reports whether the portfolio is learning over
time. DoDA outputs are evidentiary inputs — they have no independent enforcement
force. DoDA publishes findings while protecting sensitive data, privacy, research
integrity, and national-security constraints.

### Institutional Modernization Corps

The IMC builds the financial instrumentation infrastructure — the grant-linked
account systems, transaction tagging rails, ledger integrations, and anomaly
detection pipelines — to DoDA-certified specifications. Grantmaking agencies and
Treasury operate the systems once transferred. The IMC does not administer grants
or determine merit. It builds the plumbing and hands it off.

### Treasury

Treasury coordinates the financial rail, approved account architecture, ledger
standards, payment tagging rules, and integration with UPI as it matures. Treasury
is the regulatory authority for the financial infrastructure; the IMC is the
builder.

### Financial Institutions

Approved financial institutions administer accounts, cards, merchant controls,
payment processing, and transaction monitoring under federal rules. They do not
decide grant eligibility, scientific merit, portfolio strategy, or enforcement
outcomes.

### Auditors and Inspectors General

Auditors investigate flagged behavior, conduct random audits, evaluate misuse, and
refer serious cases for enforcement. Technical auditors are paired with financial
auditors where domain understanding matters.

### Independent Review Panels

Independent panels validate evaluation designs, replication protocols, field-specific
metrics, and program-level findings. This is the dual-key model in practice:
government administers public programs but cannot grade itself alone.

---

## Relationship to Research Integrity Framework

Grant Approval Reform and the Research Integrity and Methodological Transparency
Framework are designed to operate together. Grant reform governs how research is
funded. RIF governs how research is evaluated.

The protected replication and validation bucket in grant reform is the funding
mechanism that makes the RIF's replication infrastructure doctrine operational.
RIF defines independent replication as a first-class research output and a public
good. Grant reform funds it. Without the protected bucket, replication remains a
principled aspiration with no institutional home. Without the RIF, the funded
replication has no standards framework to operate within.

The digital infrastructure and methods funding bucket also supports the automated
research compliance infrastructure that DoDA specifies and the IMC builds — the
preregistration rails, protocol-to-publication matching pipelines, and disclosure
verification systems that make research process integrity monitorable at scale.

---

## Evidence Communication

Findings from publicly funded research — including null results, failures to
replicate, and infrastructure outputs — are communicated through standardized
evidence summaries consistent with the Evidence Communication doctrine in the
Research Integrity Framework.

Grant outcome reporting is one of the named instantiations of that doctrine. A
member of the public should be able to look up what a federally funded study
produced, whether the findings have been independently replicated, who funded the
work, and what the evidence maturity is — in a format readable without domain
expertise.

Aggregate portfolio performance is published through DoDA's national evidence
observability dashboards. Individual grant outcome summaries follow the minimum
fields established under the Evidence Communication doctrine: what was studied,
how it was studied, what was found, funding and independence, replication status,
evidence maturity, what is not known, and where to find more.

---

## Privacy and Data Protection

The grant ledger protects sensitive information. Public accountability does not
require exposing confidential research details, protected health information, trade
secrets, national-security information, personally identifiable information, or
sensitive institutional data.

The system uses tiered access: public reporting for aggregate spending, outcomes,
and portfolio performance; agency access for grant administration; auditor access
for flagged transactions and investigations; DoDA access for de-identified
evaluation; and restricted access for sensitive research and national-security
contexts.

Researchers do not expose scientific IP or confidential data because the financial
rail is instrumented. The ledger records financial chain of custody, not research
content.

---

## Implementation Sequence

### Phase 0: Design and Baseline

Map existing grant rules, cost categories, audit processes, award types, fraud
cases, and reporting burdens. Select pilot agencies or programs. Define admissibility
standards and initial portfolio buckets. Design ledger metadata. Recruit financial
institution partners. Establish privacy and data governance rules. Run historical
analysis on grant outcomes and known fraud cases.

### Phase 1: Silent Telemetry Pilot

Issue grant-linked accounts for a limited pilot cohort. Run transaction tagging and
anomaly models in silent mode. Do not enforce based on model output alone. Compare
flags against auditor review. Measure false positives and false negatives. Survey
grantees on administrative burden.

### Phase 2: Active Monitoring with Human Review

Begin active anomaly escalation. Maintain human review before punitive action.
Launch random audits and targeted audits. Refine spend categories. Publish early
performance reports. Protect honest failure from fraud classification.

### Phase 3: Portfolio Allocation Reform

Introduce protected frontier, replication, validation, digital infrastructure, and
translation buckets. Use admissibility review for entry. Use guarded exploration
for frontier allocation. Begin delayed composite outcome tracking.

### Phase 4: Adaptive Scaling

Expand across agencies. Integrate with UPI. Standardize grant-account rails.
Publish portfolio-level learning reports. Update statutory shares based on evidence
while preserving exploration floors.

---

## Example: NIH Research Grants

NIH is the natural flagship for this reform.

NIH already recognizes the need for high-risk, high-reward research, but the current
frontier allocation is too small to reshape the research ecosystem. Grant Approval
Reform makes frontier exploration a protected portfolio share rather than a boutique
exception.

NIH peer review retains an admissibility role: real investigator, real institution,
coherent method, testable claim, ethical design, plausible budget, no obvious fraud
or pseudo-science. After admissibility, proposals enter differentiated funding
buckets: core biomedical research, frontier exploration, replication and validation,
shared datasets and methods, digital infrastructure, and translational pathway
support.

Grant funds flow through NIH/Treasury-linked accounts built by IMC deployments.
Researchers receive grant cards or account access. Purchases are tagged against
approved categories. Most spending proceeds normally. Fraud detection runs in the
background.

Auditors evaluate suspicious spending, not failed hypotheses. A lab that pursues a
legitimate frontier idea and fails remains eligible for future funding. A lab that
fabricates progress, misuses funds, hides conflicts, or routes money to fake vendors
is removed from the system.

The result is a research system that tolerates scientific risk while becoming less
tolerant of financial abuse.

---

## Example: Public-Program Pilots

The same model supports non-research public pilots.

A city receiving a federal mobility, housing, health, or workforce grant uses an
instrumented grant account. Approved spend categories map to the pilot plan.
Transactions are logged. Outcome metrics are defined in advance and pre-registered.
DoDA compares results against baselines, matched jurisdictions, or randomized
rollout designs where appropriate. The Independent Review Panel — the second key in
the dual-key certification model — certifies that DoDA's findings are
methodologically sound before expansion is authorized.

This makes public pilots easier to fund and easier to evaluate. The government can
support more experimentation without losing control of the money or grading its
own homework.

---

## Risks and Mitigations

**Metric gaming.** Researchers and institutions may optimize for citations, patents,
or other measurable outputs. Mitigation: composite metrics, field normalization,
delayed evaluation, replication credit, negative-result credit, and caps on
single-metric influence.

**Algorithmic bias.** Adaptive models may favor elite institutions because historical
data reflects existing prestige advantages. Mitigation: adjust for institution type,
career stage, field, baseline capacity, and regional ecosystem. Protect early-career
and non-elite institution buckets.

**Over-surveillance.** Financial telemetry could become intrusive or chill legitimate
research. Mitigation: limit the ledger to financial chain-of-custody data, protect
research content, use tiered access, and require human review before enforcement.

**False fraud flags.** Normal research spending may look unusual to generic fraud
models. Mitigation: calibrate models by field, run silent pilots, publish
false-positive rates, and pair financial auditors with technical reviewers.

**Conservative admissibility review.** Reviewers may still reject unconventional
work by labeling it implausible. Mitigation: define admissibility narrowly, require
written rejection reasons, rotate panels, include frontier reviewers, and allow
appeal or lottery entry for edge cases.

**Administrative capture.** Institutions may learn to game the new categories.
Mitigation: random audits, independent evaluation, portfolio-level reporting, and
periodic DoDA certification.

---

## Statutory Hooks

A Grant Approval Reform statute defines: admissibility review standards; protected
portfolio shares; frontier exploration minimums; replication and validation funding
requirements; digital infrastructure funding requirements; grant-linked financial
account authority; approved financial institution participation; ledger metadata
standards; privacy protections; audit escalation rules; human review requirements
before enforcement; outcome evaluation standards; DoDA certification authority;
IMC build authority for financial instrumentation; public reporting obligations;
anti-gaming safeguards; and appeal rights for applicants and grantees.

---

## Political Argument

Grant reform should not be framed as anti-science or anti-government. It should be
framed as pro-discovery, pro-accountability, and anti-bureaucracy.

The public should be able to fund ambitious research without writing blank checks.
Scientists should be able to pursue hard problems without drowning in paperwork.
Agencies should be able to learn from outcomes instead of pretending every grant can
be perfectly judged in advance. Fraud should be detected through modern financial
systems — not through endless forms imposed on honest applicants.

This is also the institutional infrastructure that makes government programs
measurable in the first place. Without instrumented accounts, ledger records, and
pre-registered outcome metrics, the question "did this program work?" has no clean
answer. Grant reform is not just about research. It is about making every public
investment legible enough to learn from.

The message is: we are making public grants more ambitious, less bureaucratic, and
harder to steal.

---

## Summary

Grant Approval Reform separates the jobs the current grant system bundles together.
Peer review determines admissibility. Portfolio rules allocate risk. Financial
accounts instrument spending. Fraud models detect anomalies. Auditors investigate
misuse. Delayed composite rewards help the system learn.

The reform creates a public grant system that is more ambitious and more accountable
at the same time. It protects frontier work from bureaucratic conservatism, protects
honest grantees from unnecessary paperwork, protects public money from misuse, and
protects the grant system from confusing familiar proposals with valuable ones.

The core doctrine:

**Peer review filters bullshit. It does not pick destiny.**
