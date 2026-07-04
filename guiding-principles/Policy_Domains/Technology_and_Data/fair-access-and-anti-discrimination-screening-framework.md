---
id: fair-access-and-anti-discrimination-screening-framework
title: Fair Access and Anti-Discrimination Screening Framework
sidebar_label: Fair Access Screening
domain: Democratic_Integrity
subdomain: Civil_Rights_and_Access_Markets
policy_type: Civil Rights Infrastructure Framework
status: Draft
phase: 3
version: 0.5
author: Futures Project
changelog:
  - v0.3: Tightened Layer 6 training data language to distinguish statistical
    disparity, compliance failure, and legal finding. Softened Layer 5
    infrastructure reference to architectural inheritance rather than ledger
    identity. Added multi-route protected-characteristic data sourcing
    paragraph to Layer 3 sealed audit channel covering voluntary submission,
    existing compliance channels, and strict-protocol inference.
  - v0.4: Added operational symmetry paragraph to Protected Characteristics
    making explicit that every field is bidirectional — race means every race,
    sex means male and female, sexual orientation includes heterosexual, the
    model flags aberrant behavior in any direction. Added extensibility
    paragraph to The Procedural Standard clarifying that adding a new
    protected characteristic is a schema update, not an architectural
    redesign.
  - v0.5: Added disclosure-to-authorization reframe block in Layer 3 clarifying
    that applicants authorize a sealed civil-rights measurement channel rather
    than declaring protected identity to the covered decision-maker. Added
    corresponding sentence to Privacy Architecture making the same distinction
    explicit.
dependencies:
  - ssi-self-sovereign-identity-framework
  - upi-privacy-preserving-payment-rail
  - immutable-government-ledger
  - department-of-data-and-accountability
  - ai-data-and-governance
  - anti-capture-competition-framework
related_initiatives:
  - credential-portability-framework
  - labor-market-certification-framework
  - housing-access-and-credit-transparency
  - democratic-integrity-stack
  - government-outflow-integrity-framework
non_goals:
  - automated discrimination findings
  - quota enforcement
  - demographic balancing
  - permanent anonymity in hiring, lending, banking, housing, or education
  - public disclosure of individual applicant records
  - replacement of courts or civil-rights agencies
  - government control over private hiring or underwriting decisions
  - collection of unnecessary identity data
tags:
  - civil-rights
  - anti-discrimination
  - fair-access
  - ssi
  - zero-knowledge-proofs
  - immutable-logs
  - statistical-detection
  - labor-markets
  - lending
  - banking
  - housing
  - education
  - public-contracting
---

# Fair Access and Anti-Discrimination Screening Framework

## Executive Summary

Anti-discrimination enforcement and anti-fraud detection share the same
structural problem: both need to catch a pattern inside a decision funnel
without disrupting the legitimate majority of decisions. This framework
applies the same architecture used in the Government Outflow Integrity
Framework to access markets. The front door is de-identified — applicants
prove only what is materially necessary for that stage of review, using
the same SSI credential infrastructure that supports fraud-resistant
benefits disbursement. The back end is instrumented — re-identification
moments are logged, funnel outcomes are monitored, and statistical
aberrance generates audit flags. Flags are investigative leads, not
findings. False positive rates are governed as rigorously as detection
rates.

In covered access markets — employment, lending, banking, housing,
education, insurance, public contracting, and other statutorily defined
domains — first-round screening is conducted through de-identified SSI
credential packets. The applicant proves only the characteristics
legitimately necessary for that stage of decision-making: work
authorization, licensure, credential status, income band, cash-flow
facts, business formation, residency eligibility, collateral category,
safety certification, or other domain-specific qualifications.

Identity is reintroduced only at defined procedural stages. That
re-identification moment is logged. If similarly qualified applicants
experience statistically abnormal drop-off after protected-characteristic
visibility, the system generates an audit flag. The system does not
automate discrimination conclusions. It makes discrimination harder to
hide inside ordinary procedure.

Statistical flags are investigative leads, not legal conclusions. A
single anomaly does not establish unlawful discrimination. Repeated
unexplained anomalies across time, offices, reviewers, models, products,
or applicant cohorts create a rebuttable certification obligation. The
covered entity must explain the pattern, validate the decision variable,
remediate the funnel, or enter enhanced supervision.

---

## Strategic Premise

### The Complaint-Driven Enforcement Failure

Traditional anti-discrimination enforcement places the full evidentiary
burden on the excluded individual — the person least likely to have
access to the institution's own decision data.

A rejected applicant typically cannot see who else applied, what
qualifications they held, when identity became visible, how decision
criteria shifted across stages, whether denial reasons were applied
consistently, or whether the same pattern recurs across the firm.

Three structural failures follow from this.

Discrimination that is statistical and systemic is forced into individual
legal form. The harmed person must prove what the institution's own
decision data could reveal directly.

Intent becomes over-weighted because outcome systems are under-
instrumented. Modern discrimination may arise through biased managers,
proxy variables, referral networks, algorithmic scoring, credential
filters, geography, informal culture-fit screens, model drift, or
inherited data. None of these require an explicit discriminatory
statement.

Enforcement arrives late. By the time a complaint becomes an
investigation, the decision record may be incomplete, inconsistent,
non-standardized, or unavailable.

The result is a regime that can punish some egregious cases while
missing many structural access failures.

### The Certified Decision Funnel

The alternative is a certified decision funnel.

Covered entities retain authority to make legitimate decisions. They may
evaluate qualifications, risk, fit, capacity, portfolio quality,
creditworthiness, safety, licensure, revenue, collateral, experience,
and other lawful criteria.

The system changes what they see, when they see it, and what must be
logged when decisions change.

Where identity is not necessary, it is withheld.

Where identity becomes necessary, the reveal is recorded.

Where outcomes change after identity visibility, the pattern is measured.

Where repeated unexplained disparities persist, enforcement begins.

This is the same design logic as the Government Outflow Integrity
Framework. Make the front door easy for legitimate applicants. Instrument
the back end. Train detection models on confirmed outcomes. Govern false
positives as rigorously as detection rates. The fraud detection
architecture and the fair access architecture share the same stack — SSI
for de-identified credentialing, immutable logs for decision records,
statistical detection for pattern identification, and human review before
any enforcement action.

---

## Core Design Principle

Blind where identity is irrelevant.

Logged where discretion enters.

Statistical where intent is unknowable.

Human-reviewed where liability begins.

Symmetrical across protected classes.

The standard does not ask institutions to prove that no biased individual
exists inside their organization. It asks them to operate decision
systems whose outcomes remain explainable after legitimate qualification
controls.

Where protected-characteristic visibility changes outcomes, the
institution must be able to explain why. Where it cannot explain the
pattern, it must repair the decision system. Where it repeatedly fails to
repair the decision system, enforcement begins.

---

## The Procedural Standard

This framework governs decision-system integrity.

It does not instruct institutions to favor or disfavor any protected
class. It does not require demographic balancing, quota compliance,
institutional values statements, or group-based outcome management.

Its rule is procedural and symmetric: similarly qualified applicants
should not experience materially different access outcomes because
protected identity became visible.

The same audit architecture applies to every protected class. If a
covered decision funnel excludes Black applicants after identity
visibility, the system can flag it. If it excludes white applicants, it
can flag it. If it excludes Asian applicants, Latino applicants, women,
men, older workers, disabled applicants, veterans, immigrants, religious
minorities, rural applicants, or any other protected or statutorily
specified class, the same standard applies.

The protected characteristic does not determine the legal outcome.
The decision funnel does.

The framework does not rely on institutional preference, moral labeling,
discretionary balancing, or soft HR pressure. It relies on de-identified
screening, minimum necessary disclosure, immutable decision logs,
statistical anomaly detection, and human-reviewed certification.

The governing question is whether the decision system can explain itself.

The characteristics list is also extensible by statute without
architectural redesign. Adding a new protected characteristic is a
schema update: define the field value, route it into the sealed audit
channel, and the existing detection logic applies. This is a structural
advantage over complaint-driven enforcement, where adding a new protected
class requires rebuilding investigative capacity, legal precedent, and
institutional knowledge from scratch. The funnel integrity architecture
scales to new fields automatically.

---

## Symmetric Fair Access Standard

A covered entity does not face liability under this framework because a
protected class has a lower success rate in the abstract. A disparity
becomes legally relevant when similarly qualified applicants experience
materially different treatment after legitimate controls — especially
when the disparity appears after identity visibility, discretionary
review, branch assignment, manager review, model scoring, pricing
adjustment, or subjective evaluation.

The standard is symmetric by design. The law does not assign virtue or
suspicion by group. It tests whether protected identity changes outcomes
after legitimate qualification controls.

---

## Scope

### Covered Access Markets

This framework applies to markets where gatekeeping decisions shape
access to employment, capital, housing, essential services, public
opportunity, or regulated economic participation.

Initial covered domains include employment screening, interviews, hiring,
promotion, apprenticeship, and credentialed placement; lending, including
mortgage, consumer, student, small business, and commercial credit;
banking access, including account opening, closures, fraud holds, and
service restrictions; housing rental, mortgage access, tenant screening,
and housing platform decisions; insurance underwriting and pricing where
protected-characteristic proxy risk is material; education admissions,
scholarships, credential programs, and selective training pathways;
public contracting, supplier certification, grant access, and procurement
prequalification; and platform-mediated access markets where ranking,
verification, or eligibility decisions materially affect economic
participation.

### Covered Entities

Covered entities include employers, lenders, banks, housing platforms,
insurers, universities, credentialing bodies, public agencies, contractors
administering public programs, and large digital platforms that operate
access gates.

Small entities may be phased in through simplified compliance pathways,
shared certified screening infrastructure, or safe-harbor tools to avoid
turning compliance into an incumbent advantage.

### Protected Characteristics

The framework applies symmetrically to protected or statutorily specified
classes. Protected characteristics include race, color, sex, pregnancy,
sexual orientation, gender identity where covered by statute, religion,
national origin, age where applicable, disability, veteran status,
familial status in housing, lawful immigration or work-authorization
status where protected, and any additional class defined by federal or
state law.

Each protected characteristic is a symmetric field in the detection
model, not a directional preference. Race means every race. Sex means
male and female. Sexual orientation means every sexual orientation,
including heterosexual. Religion means every religion, including
majority faiths. National origin means every national origin, including
native-born. The model flags aberrant funnel behavior in any direction
across any field. A disparity that disadvantages a majority-group
applicant after identity visibility triggers the same threshold protocol
as one that disadvantages a minority-group applicant. The architecture
enforces this symmetry operationally — it is not a policy commitment
that future administrators could quietly reverse, it is a property of
how the detection model is built and what it is trained to find.

The governing object is funnel integrity, not group preference.

---

## Architecture

### Layer 1 — SSI De-Identified Eligibility Packet

First-stage screening occurs through an SSI-mediated eligibility packet.

The applicant's wallet generates a domain-specific, pairwise identifier
and provides cryptographic proofs responsive to the decision stage. The
covered entity receives only the attributes necessary to conduct that
stage of review.

The packet does not reveal name, race, sex, age, disability status,
precise address, school prestige, photograph, voice, or other identity-
revealing information unless that attribute is legally required or
materially necessary for the decision stage.

This is the same SSI credential infrastructure used for fraud-resistant
benefits disbursement in the Government Outflow Integrity Framework.
The wallet, proof architecture, and pairwise identifier model are shared
across both use cases. The fair access layer adds domain-specific
eligibility packet definitions and civil-rights audit channel routing.

### Layer 2 — Minimum Necessary Disclosure Rules

Covered entities may request only attributes materially relevant to the
decision stage.

The standard is minimum necessary disclosure.

A first-stage employment screen may need to know that an applicant is a
licensed electrician with six years of commercial experience and valid
work authorization. It does not need to know the applicant's name, race,
age, school, exact address, photograph, or referral source.

A first-stage loan screen may need cash-flow, income, collateral,
business revenue, and repayment information. It does not need race or
ethnicity. It may need geography where geography is materially tied to
collateral valuation or jurisdictional risk, but geographic use must be
documented because geography is also a redlining vector.

The minimum necessary rule is the first line of defense against proxy
discrimination and data extraction.

### Layer 3 — Sealed Civil-Rights Audit Channel

Protected-characteristic data is separated from the decision channel.

Decision-makers do not see it during ordinary review. Where protected-
class measurement is necessary for civil-rights auditing, the applicant
may submit protected-characteristic credentials into a sealed audit
channel that runs parallel to — and entirely separate from — the
decision process.

The certified analytics authority accesses protected-class data under
governed protocols to measure aggregate funnel outcomes, post-
reidentification drop-off, pricing disparities, denial patterns, and
appeal outcomes.

This preserves measurement without operationalizing protected identity
in the process it is meant to protect. The system must be able to detect
discrimination without giving decision-makers unnecessary access to the
attributes discrimination law is meant to protect.

The protected-characteristic audit channel changes the applicant's act
from disclosure to authorization.

Under the legacy model, applicants are often asked to declare race, sex,
disability status, veteran status, or other protected traits on forms
connected to the application process. Even where employers claim those
fields are separated from hiring review, the applicant must trust that
separation.

Under this framework, the applicant does not disclose protected identity
to the employer. The applicant authorizes a sealed civil-rights audit
channel to use protected-characteristic credentials or lawful compliance
data to test whether covered decision systems produce abnormal disparities
after legitimate controls.

The employer receives the eligibility packet. The audit authority receives
the protected-characteristic measurement channel. The two are separated
by design.

This preserves civil-rights measurement while reducing identity exposure
inside the access decision itself.

Protected-characteristic credentials entering the sealed audit channel
may be supplied through several routes depending on domain. Applicants
may voluntarily submit protected-characteristic credentials as part of
the audit channel separately from the decision packet. Where voluntary
submission is unavailable or incomplete, aggregate protected-class
measurement may be conducted through existing compliance collection
channels — such as the demographic data collected under HMDA in lending
or EEO-1 reporting in employment — under the same governed access
protocols. Where neither route is available and statistical inference
from confirmed-outcome data is legally permitted in the relevant domain,
inference may be used under strict methodological protocols with
documented uncertainty bounds. The framework does not depend on
universal applicant submission of protected-class credentials, and no
inference or compliance-channel data is exposed to ordinary decision-
makers.

### Layer 4 — Controlled Re-Identification

Re-identification is permitted where operationally necessary.

Employers eventually need to interview and hire real people. Lenders
eventually need to close loans with named borrowers. Banks need legally
accountable customers. Housing providers need lease parties. Schools
need enrolled students.

The framework does not require permanent anonymity. It requires staged
identity disclosure.

Each covered process defines permissible re-identification points. At
each point, the system logs when identity became visible, which identity
attributes became visible, who or what system gained access, what
decision followed, what reason code was recorded, and whether the
applicant advanced, was denied, withdrew, appealed, or received
different terms.

The re-identification moment is legally meaningful because it creates a
statistical test point. The cleanest signal is not simply that one group
has a lower final success rate. The cleanest signal is that similarly
qualified applicants performed comparably under blind review, but one
protected class experienced abnormal drop-off after identity-revealing
information became visible.

### Layer 5 — Immutable Decision Log

Covered entities maintain an append-only decision log for covered access
decisions, using the same append-only, cryptographically sealed audit
architecture established across the broader integrity stack.

The log records procedural events, not unnecessary personal content.
It includes pseudonymous applicant identifier, covered domain and
decision process, credential packet fields disclosed at each stage,
decision-stage timestamps, reviewer and office identifiers, re-
identification moment, protected-characteristic visibility stage,
decision outcome, reason code, pricing or terms where applicable, and
appeal or correction records.

The log does not include interview transcripts, application essays,
communications, medical narratives, raw identity documents, or
unnecessary personal details unless required by law.

The decision log is civil-rights accountability infrastructure. It is
not a commercial data asset.

### Layer 6 — Statistical Detection and Threshold Monitoring

DoDA or a certified civil-rights analytics authority monitors covered
decision funnels for aberrant patterns.

Detection operates on structured funnel data: blind-screen advancement
rates, post-reidentification drop-off, interview conversion, offer,
approval, denial, and account-opening rates, pricing and terms, reason-
code concentration, fraud-review referrals, account closures, appeals
and reversal rates, manager and branch variance, peer comparison within
domain and geography, and historical comparison within the same entity.

The detection architecture mirrors the fraud detection layer of the
Government Outflow Integrity Framework. Models are trained on confirmed
outcomes — confirmed unlawful or noncompliant patterns, confirmed
remediated process failures, and confirmed legitimate processes — not on
investigator suspicions. Every confirmed pattern enters the training
pipeline after review closure. Every confirmed false positive enters the
pipeline with equal weight. Detection rates and false positive rates are
published and audited on the same cadence.

Automated detection produces audit flags only. It does not establish
discrimination. It does not issue penalties. It does not reverse
decisions. It does not create civil liability by itself.

### Layer 7 — Human Review and Certification

Statistical flags trigger review.

Human investigators, domain experts, civil-rights officials, and where
applicable courts determine whether the pattern reflects lawful criteria,
model error, operational drift, proxy discrimination, negligent
governance, or intentional discrimination.

The review asks whether the disparity was real after legitimate controls;
whether it emerged at or after re-identification; whether the decision
variable was materially related to the decision purpose; whether it was
applied consistently; whether there was a less-discriminatory feasible
alternative; whether the entity previously received notice; whether the
entity remediated; and whether reason codes were pretextual, clustered,
or inconsistently applied.

The entity receives an opportunity to rebut, explain, correct, or
demonstrate legitimate business necessity.

---

## Threshold and Action Protocol

### Below Threshold — Longitudinal Monitoring

Patterns below threshold are retained for longitudinal monitoring. No
entity-specific intervention occurs. The purpose is to preserve the
ability to detect compounding or recurring patterns without creating
enforcement noise.

### Notice Threshold — Confidential Notice

At notice threshold, the covered entity receives confidential
statistical notice. The entity must conduct internal review and preserve
relevant decision logs. No public finding is made. No penalty attaches.

### Review Threshold — Documentation Obligation

At review threshold, the entity must submit decision-variable
documentation, funnel metrics, reason-code definitions, model cards
where applicable, and validation evidence. The question is whether the
disparity is explainable by legitimate, consistently applied, materially
relevant decision criteria.

### Corrective Threshold — Corrective Certification

At corrective threshold, the entity enters corrective certification.
This may require a remediation plan, enhanced reporting cadence,
validation of high-impact variables, restriction of weak proxy
variables, standardized reason-code use, manager or branch-level review,
model recalibration, vendor audit, applicant appeal repair, or an
external civil-rights monitor.

The objective is repair before punishment.

### Enforcement Threshold — Civil-Rights Referral

At enforcement threshold, repeated unexplained disparities after notice
and corrective certification may be referred to civil-rights enforcement.
Referral may occur where disparities persist after remediation, the
entity cannot validate high-impact variables, reason codes appear
pretextual, records are incomplete or falsified, the entity refuses
cooperation, or protected-class drop-off consistently appears after
re-identification without lawful explanation.

A single statistical anomaly does not establish unlawful discrimination.
Repeated unexplained anomalies create a rebuttable certification
obligation. Persistent failure to satisfy that obligation may support
enforcement.

---

## Variable Validity Standard

The central gaming risk is proxy laundering.

Once direct identity variables are hidden, institutions may shift
discriminatory discretion into variables that correlate with protected
class but have weak legitimate value. Examples include school prestige,
employment gaps, referral source, ZIP code, neighborhood, name-adjacent
metadata, extracurricular organizations, accent or communication-style
proxies, social-media presence, personality scoring, automated video
interview features, legacy banking relationships, collateral proxies that
embed historical segregation, and unexplained fraud-risk features.

A covered entity using a high-impact decision variable must be able to
demonstrate that the variable is materially related to the lawful
decision purpose, consistently applied, periodically validated, and not
replaceable by a feasible less-discriminatory alternative.

Historical use is not sufficient. Administrative convenience is not
sufficient. Vendor certification alone is not sufficient.

If a variable has high disparate impact and low predictive validity,
it must be removed, capped, delayed to a later stage, or replaced.

---

## Model and Vendor Governance

Where covered entities use algorithms, AI systems, scoring tools,
automated underwriting, resume screeners, fraud models, tenant-screening
tools, or third-party vendors, the entity remains responsible for the
decision system. A vendor cannot be used as a liability shield.

Covered algorithmic systems must maintain model version history,
training-data provenance, documented target variables, feature
inventory, protected-class impact testing, reason-code mapping, false-
positive and false-negative evaluation, subgroup calibration reports,
human override records, and appeal and correction pathways.

Models used in covered access decisions may assist, rank, score,
summarize, or flag. They may not create unreviewable denials in
high-impact access markets.

---

## False Positive Discipline

Anti-discrimination detection carries its own false-positive risk,
governed by the same logic that applies to fraud detection.

If thresholds are too sensitive, legitimate institutional variation
becomes enforcement noise. If thresholds are too weak, structural
discrimination remains hidden. The civil-rights analytics authority is
subject to the same reciprocal accountability it applies to covered
entities.

The authority must publish and audit flag rates by domain, referral
rates, sustained finding rates, false-positive rates where review finds
no actionable issue, unsupported referral rates, threshold drift,
subgroup calibration quality, small-sample suppression rules, appeal
success rates, and time-to-resolution.

Repeated unsupported enforcement referrals trigger internal review of
the enforcement body. Bad-faith or politically motivated initiation is
itself an institutional integrity failure.

The system's legitimacy runs in both directions: covered entities must
explain repeated unexplained disparities, and enforcement bodies must
explain repeated unsupported actions.

---

## Privacy Architecture

This framework reduces identity exposure rather than expanding it.

Applicants disclose fewer raw personal attributes at the first stage
than they do under current systems. Covered entities receive proofs
rather than documents wherever possible. Decision logs use pseudonymous
identifiers. Protected-characteristic analysis is performed under
governed access by authorized civil-rights analytics bodies, not exposed
to ordinary reviewers. Applicants are not asked to declare protected
identity to the covered decision-maker; they authorize protected-
characteristic measurement through a sealed audit channel governed by
civil-rights law. Individual applicant records are not public.
Aggregate statistics may be published with disclosure controls.

The system does not create a general-purpose government identity
database, cross-service profile, or public applicant registry.

---

## Domain Applications

### Employment

First-round screening uses de-identified qualification packets.
Employers receive verified job-relevant characteristics such as
licensure, experience band, work authorization, portfolio certification,
skills assessment, availability, and location constraints. Names,
photographs, age, race, sex, exact address, school prestige, and other
irrelevant identity signals are withheld unless necessary.

Re-identification occurs at interview or conditional offer stages
depending on role type. The audit system monitors whether similarly
qualified applicants experience abnormal drop-off after re-
identification, after voice or video interviews, after manager
assignment, after referral review, or after subjective evaluation.

### Lending

Underwriting begins from verified cash-flow, income, collateral,
repayment, business revenue, and debt-service proofs. Race is not
visible to underwriters. Geography is governed because it can be both
legitimately relevant and historically discriminatory.

The audit system monitors approval rates, interest rates, fees,
collateral adjustments, denial reasons, fraud referrals, manual review
outcomes, and appeal reversals. The key signal is whether similarly
situated borrowers receive worse terms or higher denial rates after
identity, geography, branch, or manual discretion enters the process.

### Banking

Account access begins with proof of identity verification, compliance
status, age eligibility, and sanctions-screening clearance. The system
monitors abnormal account-opening denial, fraud holds, account
closures, enhanced due diligence referrals, and service restrictions
by protected class or protected-class proxy.

This is especially important for immigrants, low-income households,
religious minorities, cash-heavy businesses, and communities
historically treated as risk categories rather than customers.

### Housing

Tenant screening begins with verified income-to-rent band, rental
history, subsidy eligibility, household-size compatibility, identity
verification, and lawful occupancy eligibility. Landlords and platforms
do not see unnecessary identity data at the first gate.

The audit system monitors showing access, application advancement,
denial reasons, security deposit terms, rent offers, lease approvals,
voucher treatment, and post-reidentification drop-off.

### Education and Training

Selective programs may screen first on competency, prerequisite
completion, credential eligibility, portfolio samples, income
eligibility where relevant, and geographic or service-commitment
constraints. Re-identification may occur at interview, finalist, or
enrollment stages.

The audit system monitors whether protected-class disparities emerge
after identity visibility, legacy review, recommendation review,
interview, discretionary committee scoring, or subjective evaluation.

### Public Contracting

Supplier prequalification begins with verified business status,
licensure, bonding capacity, revenue band, performance history, safety
record, ownership eligibility where legally relevant, and conflict-
screening proofs. The audit system monitors whether minority-owned,
women-owned, veteran-owned, rural, small, or non-incumbent firms drop
abnormally after discretionary review, relationship-based scoring,
bonding interpretation, or incumbent preference.

---

## Legal Standard

The statutory standard:

A statistically significant disparity does not, by itself, establish
unlawful discrimination.

A repeated unexplained disparity in a covered decision funnel creates
a rebuttable certification obligation. The covered entity must
demonstrate that the challenged variable, model, procedure, or
discretionary practice is materially related to legitimate decision
criteria, applied consistently, and not replaceable by a feasible less-
discriminatory alternative.

Failure to satisfy that obligation after notice and corrective
opportunity may support enforcement.

Intent evidence, where present, remains independently actionable.

The framework does not create quota liability.

---

## Governance

### DoDA or Certified Civil-Rights Analytics Authority

The analytics authority owns statistical certification, threshold
publication, audit protocols, aggregate reporting, and methodological
validation. It does not make hiring, lending, housing, education,
banking, insurance, or contracting decisions. It does not publish
individual applicant records. It does not issue automatic liability
findings. Its role is measurement, certification, and referral.

### Sector Regulators

Sector regulators define domain-specific legitimate variables, minimum
necessary disclosure standards, and model documentation requirements.
Examples include EEOC for employment, CFPB and banking regulators for
lending and banking, HUD for housing, the Department of Education for
education access, FTC for platform-mediated access markets, and
procurement authorities for public contracting.

### Courts and Civil-Rights Agencies

Courts and civil-rights enforcement agencies retain legal authority.
The statistical system creates evidence, triage, and certification
obligations. It does not replace legal process.

---

## Phase Strategy

### Phase 0 — Standards and Pilot Design

Define covered domains, minimum necessary disclosure standards,
decision-log schemas, reason-code taxonomies, protected-class analysis
protocols, threshold governance, and privacy rules.

Pilot only in domains where SSI credentials and structured decision data
are mature enough to support meaningful testing. Recommended first pilots
include large-employer first-round hiring, public-sector hiring,
apprenticeship and credentialed workforce placement, mortgage
prequalification, small-business lending through participating public
programs, and public contracting prequalification.

### Phase 1 — Voluntary and Public-Sector Pilots

Begin with public agencies, federal contractors, PCA-backed programs,
and voluntary private-sector participants. This avoids immediate
universal compliance burden while generating empirical baselines.
Publish aggregate pilot results. Refine threshold calibration. Validate
false-positive discipline.

### Phase 2 — Federal-Funds Condition

Entities receiving federal funds, federal guarantees, federal contracts,
public workforce funding, housing subsidies, or public lending support
must use certified fair-access screening in covered processes. This
creates adoption leverage without immediately federalizing all private
decision-making.

### Phase 3 — Covered Market Expansion

Large covered entities in employment, lending, banking, housing,
education, insurance, and platform access markets become subject to
phased compliance. Small entities receive simplified safe-harbor
pathways and certified third-party tools.

### Phase 4 — Full Decision-Funnel Certification

Covered access markets operate under standardized decision-log schemas,
periodic funnel audits, model and vendor certification, and statistical
threshold monitoring. DoDA publishes aggregate market integrity
dashboards showing access, disparity, flag, remediation, and enforcement
trends without exposing individual applicant records.

---

## Failure Modes

The framework fails if de-identification is superficial and proxy
variables remain unconstrained.

It fails if statistical flags become automatic guilt.

It fails if protected-class data is exposed to ordinary reviewers.

It fails if small-sample noise produces enforcement churn.

It fails if vendors become unaccountable decision-makers.

It fails if compliance costs entrench large incumbents.

It fails if agencies optimize for finding violations rather than
improving funnel integrity.

It fails if firms can delete, alter, or selectively reconstruct decision
records after a complaint.

It fails if the sealed civil-rights audit channel becomes a general-
purpose identity database.

It fails if the system treats symmetry as rhetorical rather than
operational.

---

## Conclusion

Civil-rights enforcement should not depend on excluded individuals
reverse-engineering opaque decision systems from the outside.

If institutions make consequential access decisions, they should be able
to show how those decisions were made, when identity became visible,
what variables mattered, and whether similarly qualified people were
treated differently after protected-characteristic visibility.

The old regime asks whether the applicant can prove bias. The new regime
asks whether the decision system can explain itself. That is a better-
aimed question — and the same infrastructure that makes government
disbursement honest makes access markets legible.
