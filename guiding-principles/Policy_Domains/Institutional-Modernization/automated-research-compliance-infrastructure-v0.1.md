---
id: automated-research-compliance-infrastructure
title: Automated Research Compliance Infrastructure
sidebar_label: Automated Research Compliance
slug: /institutional-modernization/automated-research-compliance-infrastructure
domain: Institutional_Modernization
subdomain: Evidence_and_Accountability
policy_type: Technical Infrastructure
status: draft
version: 0.1
author: Futures Project
last_updated: 2026-05-30
dependencies:
  - research-integrity-and-methodological-transparency-framework
  - department-of-data-and-accountability
  - institutional-modernization-corps
  - immutable-government-ledger
  - grant-approval-reform
  - unified-law-regulation-repository
  - ssi-self-sovereign-identity-framework
tags:
  - research-integrity
  - automation
  - compliance
  - ml-pipelines
  - preregistration
  - doda
  - monitoring
  - publication-bias
  - endpoint-drift
---

# Automated Research Compliance Infrastructure

## Purpose

This brief defines the technical infrastructure that makes the Research Integrity
and Methodological Transparency Framework operational at scale.

The core problem is one of volume. Hundreds of thousands of federally funded studies
are active at any given time. Preregistration requirements, disclosure obligations,
protocol-to-publication matching, endpoint consistency checks, and funding disclosure
verification cannot be performed through per-study human review without creating
precisely the bureaucratic bottleneck the framework is designed to avoid.

Automated pipelines solve this. A pre-registration record is a structured data
object. Checking whether a published paper's endpoints match the registered plan is
a string-comparison and statistical-structure problem. Detecting anomalous p-value
distributions across a body of literature is a pattern-recognition problem. Flagging
publication gaps against registered protocols is a database reconciliation problem.
None of these require human reviewers to read papers. They require well-designed
pipelines, clean data standards, and a permanent public record that creates the
reference point for comparison.

Human reviewers become the exception handler — the escalation endpoint for anomalies
the pipeline surfaces, not the first-pass filter for a literature that no realistic
staffing level can cover.

This is DoDA's observability function. DoDA specifies and certifies the national
evidence observability layer — the APIs, schemas, identifiers, audit logs, routing
rules, and dashboard requirements that make research compliance legible across
institutions. The IMC builds the implementing systems. Domain authorities receive
the flags. The public sees the dashboard.

---

## Design Principle

**Standardize the rails. Automate the obvious. Escalate the unusual.**

Routine compliance — verifying that a protocol was registered before enrollment,
that disclosed funding matches grant records, that reported endpoints appear in the
registered plan — is automatable and should be automated. The pipeline runs
continuously. Compliance is the default state. Anomalies surface as exceptions
requiring human judgment.

This is identical to the logic already applied in the healthcare fraud detection
architecture: automated anomaly detection, human review before enforcement,
permanent immutable ledger. The research compliance pipeline is the same pattern
applied to the evidence layer rather than the payment layer.

Critically, this framework does not automate peer review, replication, or
scientific validation. Those remain human functions performed by domain experts.
What this framework automates is process compliance monitoring — the structured
check that what was published matches what was registered, that disclosures are
complete, and that statistical patterns across a body of literature are consistent
with genuine inquiry rather than coordinated manufacturing of results. Human
reviewers conduct science. The pipeline monitors the integrity of the process
those reviewers depend on.

---

## Digital Laboratory Notebooks and LIMS Integration

The most robust fraud-resistance architecture is one where compliance is ambient
rather than retrospective. If researchers are entering data into a system that has
federal API hooks built in as the project progresses, the fraud surface collapses
significantly. Retroactive fabrication of a data trail that was being written in
real time is structurally harder than fabricating a final publication. Statistical
checks run on live data entry are harder to game than checks run on submitted
manuscripts, because the data history is already in the record by the time results
are generated.

The approach is adaptation, not mandated replacement. Laboratory Information
Management Systems (LIMS) are already standard in serious research environments.
Serious labs already have QA departments, audit trails, and data integrity
procedures. The ask is standardized federal API conformance — not a wholesale
system replacement or a government-run platform that researchers must use.

**Federated LIMS model.** Research institutions may use any LIMS system — commercial,
open-source, or internally developed — provided it conforms to the federal API
standards specified by DoDA and enumerated by the IMC for each deployment context.
Conforming systems expose standardized APIs that allow DoDA to pull structured data
for periodic compliance checks without requiring bulk data access or continuous
surveillance.

**What the federal API pulls.** The integration is narrow and purpose-bound:
protocol registration status, endpoint definitions as structured data fields,
enrollment milestones, amendment history with timestamps, and statistical analysis
plan metadata. Clinical data, raw experimental data, and identifiable participant
information are not pulled through the federal API. The pull is about process
compliance, not scientific content.

**Researcher SSI credential integration.** Each researcher's LIMS profile is
linked to their SSI credential, which carries verifiable attestations of
institutional affiliation, employment relationships, and registered funding
disclosures. The LIMS system authenticates against that credential. Conflicts of
interest that appear in the SSI credential — employment by a sponsor, equity
relationships, consulting arrangements — are structurally detectable against what
the researcher disclosed in the protocol registration, without requiring manual
cross-referencing or self-report alone.

**Contracted LIMS systems.** Where institutions use contracted or commercial LIMS
platforms, those platforms must satisfy the same federal API conformance requirements
as any other contracted government-interfacing system. The IMC enumerates the
specific technical requirements. DoDA certifies conformance. Systems that cannot
interface with the federal compliance layer through published APIs are not eligible
for use in federally funded research programs. This is the structural defense against
compliance silos reasserting themselves through vendor platforms.

---

## Infrastructure Components

### 1. Preregistration Rail

The preregistration rail is the foundation of the entire compliance architecture.
A pre-registered protocol is a timestamped, immutable public record. Everything
else in the pipeline compares outputs against that record.

**What it stores:**

- Study identifier linked to the registering institution's SSI credential
- Protocol version and amendment history
- Primary and secondary endpoints as structured data fields
- Statistical analysis plan, including pre-specified methods and thresholds
- Enrollment targets and population definition
- Funding sources and conflict-of-interest disclosures
- Expected completion and publication timeline
- Any subsequent amendments with timestamps and justification fields

**How it works:**

Registration occurs through a standardized API before enrollment begins.
The record is written to the Immutable Government Ledger and assigned a
permanent, publicly accessible identifier. Amendments are permitted but logged
as versioned updates — the original registration is never overwritten. The gap
between an original registration and a subsequent amendment is itself a data
point that the pipeline tracks.

The preregistration rail does not require DoDA to read protocols. It requires
institutions to submit structured data through a standardized interface. The
submission format is machine-readable by design.

### 2. Protocol-to-Publication Matching Pipeline

Once a study's expected completion window has passed, the matching pipeline
activates. It compares the registered protocol against the published record.

**What it checks:**

- Whether a publication exists for the registered study
- Whether the reported primary endpoints match the registered endpoints
- Whether the reported statistical methods match the pre-specified plan
- Whether the reported sample size falls within the registered enrollment targets
- Whether the funding and conflict-of-interest disclosures in the publication
  match the registered disclosures
- Whether amendment history is reflected in the published methods section

**What it flags:**

- Non-publication after the expected completion window: the registered study
  has no linked publication. This is a detectable gap, not a private decision.
- Endpoint drift: the primary endpoint in the publication differs from the
  registered primary endpoint. The pipeline flags the specific divergence.
- Method substitution: statistical methods in the publication differ from the
  pre-specified plan without a registered amendment justifying the change.
- Disclosure mismatch: funding sources or conflicts in the publication do not
  match the registered disclosures.

**What it does not do:**

The pipeline does not determine whether endpoint drift was scientifically
justified. It flags that it occurred. Human review — by the domain authority
or the institution's research integrity board — determines whether the
deviation was appropriate, disclosed, and defensible. The pipeline surfaces
the question. It does not answer it.

### 3. Statistical Pattern Detection

Certain forms of research misconduct produce detectable statistical signatures
across a body of literature even when individual studies are not obviously
problematic in isolation.

**P-value distribution monitoring.** In a large body of genuinely independent
studies, p-values should be distributed relatively uniformly below the significance
threshold. A spike of p-values just below 0.05 — the classic signature of
p-hacking, selective reporting, or HARKing — is statistically anomalous and
detectable at the literature level. The pipeline monitors p-value distributions
within ingredient categories, sponsor cohorts, research groups, and funding streams.

**Effect size consistency.** Sponsor-funded studies on the same intervention often
produce systematically larger effect sizes than independent replications. That
divergence is measurable. The pipeline tracks effect size distributions by funding
source within a research domain.

**Outcome reporting completeness.** Registered secondary endpoints that do not
appear in publications, baseline characteristics that shift between registration
and publication, and subgroup analyses that appear in publications without
pre-registration — these patterns are detectable through structured comparison.

Statistical pattern detection operates at the aggregate level. It generates
signals about research areas, sponsor cohorts, or institutional patterns — not
determinations about individual studies. Those signals inform audit priority and
independent replication targeting, not enforcement actions.

### 4. Disclosure Verification Pipeline

Funding and conflict-of-interest disclosures are verifiable against external
records where those records exist. The SSI-based researcher credential architecture
makes this structurally more robust than self-report systems.

**SSI credential cross-reference.** Each researcher's SSI credential carries
verifiable attestations of institutional affiliation, employment relationships,
equity positions, and registered funding arrangements. The pipeline cross-references
disclosed conflicts against the researcher's live SSI credential. Relationships that
appear in the credential but are absent from the protocol registration or publication
disclosure are flagged as undisclosed conflicts. This makes conflict detection a
structured data comparison rather than a manual audit of self-reported forms.

**Grant record matching.** Federally funded studies disclose federal grant
identifiers. The pipeline matches disclosed grant identifiers against the relevant
agency's grant database. Discrepancies — grants disclosed that do not match records,
or grant relationships detectable from acknowledgments that are not disclosed —
are flagged.

**Industry relationship verification.** Industry funding relationships registered
through the Open Payments database and equivalent registries can be cross-referenced
against researcher SSI credentials and publication disclosures. Systematic
non-disclosure of known industry relationships is a detectable pattern at the
institutional level.

**Institutional affiliation consistency.** Author affiliations, corresponding
author institutions, and acknowledgment sections provide multiple reference points
for verifying disclosed relationships. The pipeline identifies inconsistencies
across these fields and against the SSI credential record.

### 5. Replication Coverage Dashboard

The pipeline tracks replication status across research domains, providing a
public-facing signal about where the literature rests on replicated versus
unreplicated foundations.

**What it displays:**

- Proportion of high-influence findings in a domain with at least one
  independent replication attempt
- Proportion of independent replications that confirm versus fail to confirm
  original findings
- Time elapsed since original publication without replication attempt
- Funding source distribution for replication attempts versus original studies

This dashboard serves two functions. It is public accountability infrastructure —
researchers, journalists, policymakers, and the public can see where evidence is
strong and where it rests on unreplicated foundations. It is also a targeting
signal for the grant system's replication and validation funding bucket, which
directs public research dollars toward the highest-value independent replication
targets.

### 6. Institutional Compliance Dashboards

DoDA publishes institution-level and domain-level compliance dashboards showing
aggregate performance across the monitored metrics.

**Institution-level view:**

- Preregistration rate for funded studies
- Publication completion rate against registered timelines
- Endpoint consistency rate (proportion of studies with no flagged endpoint drift)
- Disclosure match rate
- Replication engagement rate

**Domain-level view:**

- Aggregate compliance metrics across the domain
- Sponsor-funded versus independently funded study distribution
- Replication coverage
- Statistical pattern anomalies flagged at the domain level
- Active monitoring flags and their resolution status

Dashboards are public. Institutions can see their own metrics and compare against
domain-level aggregates. Sponsors can see how their funded research cohort performs
against the same benchmarks applied to independently funded work. The information
asymmetry that allows systematic non-compliance to persist invisibly is the primary
target.

---

## Data Standards and Interoperability

The pipeline's value depends on data standards that make outputs comparable across
institutions, funders, and domains. DoDA defines and maintains those standards.
The IMC enumerates the specific technical implementation requirements for each
deployment context.

**Protocol data schema.** Standardized fields for endpoint specification, population
definition, statistical plan, and funding disclosure. Machine-readable formats
required. Narrative-only disclosures are not sufficient for pipeline processing.

**Contractor and vendor API conformance.** Any LIMS system, research platform, or
data system used in federally funded research must conform to DoDA-specified API
standards as a condition of use. This covers schemas, audit log formats,
authentication interfaces, and data access controls. Conformance is certified by
DoDA before a system is approved for use. Systems that cannot interface with the
federal compliance layer through published standards are not eligible for use in
federally funded research programs. The IMC enumerates specific technical
requirements by deployment context. This is the structural defense against research
data siloing through proprietary vendor platforms.

**Publication metadata schema.** Structured fields for reported endpoints, sample
characteristics, statistical methods, and funding disclosures, extracted from
published papers through automated parsing and where necessary through structured
submission requirements for journals participating in the framework.

**Cross-domain identifiers.** Persistent study identifiers that link the
preregistration record, any amendments, the published output, and any replication
attempts. The identifier system connects to the SSI credential of the registering
institution for attribution and audit purposes.

**ULRR integration.** Research compliance records, certification statuses, and
aggregate monitoring findings are indexed in the Unified Law and Regulation
Repository alongside regulatory and policy records. This makes research evidence
status queryable alongside the policy frameworks that depend on it.

---

## Institutional Architecture

### DoDA Operates the National Evidence Observability Layer

DoDA maintains the national interoperability standards for these pipelines and
operates the core observability layer: the preregistration rail specifications,
the protocol-to-publication matching requirements, the statistical monitoring
dashboard standards, the disclosure verification API specifications, and the
public reporting standards. DoDA certifies that implementing systems meet those
specifications. DoDA does not build the implementing systems itself.

The Institutional Modernization Corps builds the infrastructure to DoDA-certified
specifications. Pipelines may subsequently be operated by domain authorities,
universities, accredited infrastructure providers, or approved public-interest
data utilities — provided they conform to DoDA-certified schemas, audit logs,
routing rules, and transparency requirements. The standard is DoDA's. The build
is the IMC's. The operation is distributed.

DoDA does not review individual studies. It does not make findings about whether
endpoint drift was scientifically justified. It does not determine whether a
statistical pattern represents misconduct or legitimate variation. It certifies
specifications, surfaces aggregate anomalies through the observability layer, and
publishes the data.

### Flags Route to Domain Authorities

When the pipeline flags an anomaly, the flag routes to the relevant domain
authority — NIH's Office of Research Integrity, FDA's compliance functions,
the relevant agency's inspector general, or the institution's research integrity
board — depending on the funding source and domain.

DoDA does not receive the flag and then decide what to do with it. The routing
is defined by the domain relationship architecture in the RIF. DoDA is the
plumbing. Domain authorities are the endpoints.

### Human Review Before Any Consequence

No automated flag produces an enforcement consequence. The pipeline is a
prioritization and anomaly-detection system. Human reviewers within the relevant
domain authority determine what the flag means and whether escalation is warranted.

This is not a limitation of the system. It is a design requirement. Automated
pattern detection has false positive rates. Research is complex. Context matters.
The pipeline makes human review more targeted and more efficient — it does not
replace it.

### Immutable Ledger as the Reference Record

Every preregistration, amendment, flag, routing event, and resolution is logged
in the Immutable Government Ledger. The ledger creates permanent, tamper-resistant
chain of custody for the compliance record. A flag that was routed, reviewed, and
cleared is a different record than a flag that was routed and never resolved.
The difference is visible and auditable.

This is what makes the race condition between institutional disclosure and external
flag detection meaningful. An institution that discovers a compliance problem and
discloses through the standing track creates a ledger record that precedes any
pipeline flag. An institution that receives a pipeline flag without having
disclosed creates a different ledger record. The sequence is permanent and
unambiguous.

---

## What This Infrastructure Is Not

This is not a surveillance system for researchers. The pipeline operates on
structured data about protocols, publications, and disclosures — not on research
content, private communications, or unpublished work. A researcher's scientific
ideas, unpublished findings, and internal deliberations are not monitored.

This is not a replacement for peer review. Peer review evaluates scientific
quality, logical coherence, and methodological soundness. The pipeline evaluates
process compliance — whether what was published matches what was registered.
These are different questions requiring different expertise.

This is not a tool for suppressing unconventional research. The compliance
requirements are procedural: register before you enroll, disclose your funding,
report your pre-specified endpoints. A researcher pursuing an unconventional
hypothesis through a transparent, pre-registered, properly disclosed study has
nothing to fear from this infrastructure.

This is not a DoDA enforcement mechanism. DoDA operates the rails and publishes
the data. Domain authorities determine consequences through their existing
processes with full due process protections.

---

## Relationship to the Research Integrity Framework

This brief is a dependency of the RIF, not a standalone instrument. The RIF's
monitoring functions — described in Layers One, Six, and Eight of that document
— are operationalized through this infrastructure. Without it, those layers
describe aspirations. With it, they describe an operational system.

The RIF defines what should be monitored and why. This brief defines how
monitoring is performed at scale. Both are required.

---

## Relationship to Grant Approval Reform

The grant reform framework's preregistration requirements and immutable ledger
logic are the same infrastructure described here applied to the grant funding
context. The automated compliance pipeline operates on both: a study funded through
the NIH grant system and a study funded through a supplement manufacturer's
research program are both preregistered on the same rail and monitored by the
same protocol-to-publication matching pipeline.

This is the mechanism that makes non-publication a detectable event rather than
a private decision. A sponsor who funds a study, registers it on the public rail,
and then does not publish the results creates a visible gap in the ledger. The
pipeline detects that gap. The dashboard displays it. The domain authority's queue
receives the flag. The decision to suppress results is no longer invisible.

---

## Relationship to CDE Framework

The automated compliance pipeline is an evidentiary input to the CDE framework's
DoDA detection layer. Systematic patterns flagged by the pipeline — coordinated
endpoint drift across a sponsor's funded research cohort, correlated non-publication
across related studies, anomalous p-value distributions concentrated in a funding
stream — are exactly the kind of cross-entity pattern that the CDE framework's
detection layer is designed to surface.

The pipeline does not make CDE findings. DoDA does not make CDE designations.
But the permanent, auditable record the pipeline creates is what makes
organizational-level coordination detectable even when no individual act is
dispositive. The pattern is in the ledger. The ledger does not change.

---

## Phase Strategy

**Phase 0 — Standards and baseline.** DoDA defines the protocol data schema and
publication metadata schema. Preregistration rails are built. Pilot institutions
connect. Baseline compliance rates are established before monitoring begins, so
that later comparison is against a known starting point rather than an assumed one.

**Phase 1 — Silent monitoring.** The protocol-to-publication matching pipeline
runs in silent mode. Flags are generated and reviewed internally against auditor
judgment. False positive rates are measured and models are calibrated. No flags
are routed externally.

**Phase 2 — Active monitoring with domain routing.** Flags begin routing to
domain authorities. Human review processes are established. Resolution tracking
goes into the ledger. Public dashboards launch showing aggregate metrics.

**Phase 3 — Statistical pattern detection.** The more sophisticated pipeline
layers — p-value distribution monitoring, effect size consistency tracking,
disclosure verification — go live. These require larger data volumes to be
statistically meaningful. They are not appropriate for Phase 1.

**Phase 4 — Full integration.** ULRR integration. Cross-domain identifier
system. Replication coverage dashboard. Full public API access to aggregate
compliance data.

---

## Summary

The research compliance problem is not a staffing problem. It is a data
infrastructure problem. The volume of federally funded research exceeds what
any realistic human review capacity can monitor continuously. The solution is
not to monitor less or accept the opacity — it is to build the pipelines that
make compliance the default and anomalies the exception.

DoDA certifies the observability specifications. The IMC builds the infrastructure
to those specifications. The pipelines run continuously once deployed. Flags route
to the relevant domain authority. Human reviewers handle escalations. The public
sees the dashboard.

The plumbing makes the framework real.
