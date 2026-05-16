---
id: healthcare-market-integrity-and-anti-gaming-framework
title: Healthcare Market Integrity, Anti-Gaming, and Cost Validation Framework
sidebar_label: Market Integrity and Anti-Gaming
sidebar_position: TBD
slug: /healthcare/execution/market-integrity-and-anti-gaming
domain: Healthcare
subdomain: Execution_and_Transition
policy_type: Market Integrity and Enforcement Framework
status: Draft
version: 0.4
author: Futures Project
last_updated: 2026-05-09
dependencies:
  - healthcare-execution-authority
  - heta-revised-charter
  - healthcare-infrastructure-layer
  - healthcare-transition-phase-strategy
  - healthcare-state-pilot-framework
  - insurance-architecture-sec
  - cost-performance-backstop
  - public-capital-authority
  - employer-sponsored-coverage-transition
  - coordinated-deceptive-practices-enforcement-framework
related_initiatives:
  - department-of-data-and-accountability
  - regional-health-center-network
  - permanent-health-security-accounts
tags:
  - healthcare
  - anti-gaming
  - cost-validation
  - transparency
  - nearest-neighbor-analysis
  - sec
  - heta
  - doda
  - provider-pricing
  - insurer-behavior
  - anti-capture
  - coordinated-deceptive-enterprise
description: >
  Establishes the market integrity, anti-gaming, and cost validation framework
  governing the restructured healthcare system, including standardized cost reporting,
  nearest-neighbor benchmarking, DTC standard-candle comparison methodology,
  insurer anti-denial logic, SEC boundary enforcement, vendor integrity rules,
  institutional anti-capture design, and the CDE escalation pathway for
  organizational-level coordinated fraud.
---

## Purpose and Scope

This brief defines the integrity architecture governing the restructured healthcare
market. The objective is not merely to detect and punish fraud after it occurs. The
objective is to structurally reduce the profitability of the behaviors that have
distorted healthcare economics for decades — opacity, artificial scarcity, denial
complexity, administrative gaming, monopoly extraction, and billing manipulation —
by making the system observable, comparable, and auditable at every layer.

This framework does not regulate benefit design, pharmaceutical policy, or malpractice
standards. Those are governed separately. What it governs is the integrity of the
market structure that makes the rest of the reform work: the transparency requirements
that allow prices to be compared, the benchmarking systems that make unexplained
variance visible, the boundary enforcement that keeps market-layer care from migrating
into SEC, the ownership rules that prevent consolidation from neutralizing competition,
the vendor integrity rules that keep the technical infrastructure from becoming a
gaming surface, and the institutional design that prevents enforcement from being
captured by the entities it regulates.

The framework operates in conjunction with HETA's enforcement authority, DoDA's
independent measurement mandate, the SEC actuarial architecture, and the Immutable
Government Ledger. The Immutable Government Ledger is the Futures Project's
append-only, privacy-preserving audit infrastructure. It is not a public blockchain,
a cryptocurrency system, or a transaction-level public surveillance tool. It is an
internal audit record designed to make historical data permanent, attributable, and
resistant to retroactive manipulation by the institutions that generate it.

---

## Why This Framework Exists

The current healthcare system allows a large portion of its cost growth to hide inside
structures that are individually defensible and collectively indefensible. Fragmented
billing systems prevent comparison. Insurer-provider negotiation opacity prevents
anyone outside the transaction from knowing what anything actually costs. Facility-fee
layering, post-hoc coding escalation, and emergency upcoding add cost in ways that
are invisible at the point of care. Monopoly conditions in regional markets allow
providers to price against the absence of alternatives rather than against their own
costs. Debt-service obligations accumulated through decades of acquisition and
consolidation get recovered through patient billing rather than disclosed as what they
are.

The consequence is that policymakers cannot distinguish between a hospital that costs
what it costs because of genuine emergency readiness obligations, rural access burdens,
and regional labor markets — and a hospital that costs what it costs because of
monopoly pricing, administrative inflation, and leverage over a captive patient
population. When that distinction cannot be made, policy cannot respond to actual cost
drivers. It can only add more money to an opaque system and hope some of it reaches
care.

This framework makes that distinction possible. Once costs and prices are visible,
comparable, and auditable, the difference between legitimate operational burden and
extractive behavior becomes identifiable and actionable.

---

## Core Design Principle

The framework does not rely primarily on trust. It changes the incentive environment.

Providers who deliver legitimate care at legitimate cost should find honest
participation in the reformed system easier and more profitable than gaming it.
Insurers should find that competing on service quality, reduced friction, and superior
supplemental products is more commercially durable than denial complexity. Hospitals
with genuine emergency readiness and rural access obligations should receive
transparent, direct support rather than being forced to recover those costs through
inflated billing structures that nobody can audit.

The design target is a system where opacity becomes expensive because visible anomalies
trigger escalating scrutiny; where denial becomes commercially unsustainable because
SEC removes the leverage that made denial profitable; where administrative gaming
becomes self-defeating because the Immutable Government Ledger makes patterns permanent
and detectable; and where transparent participation becomes the path of least
resistance for any provider or insurer whose cost structure can withstand examination.

---

## The Anti-Gaming Architecture: An Explicit Enumeration

The framework operates through nine distinct anti-gaming mechanisms. Each targets a
specific failure mode in the current system. Together they constitute a layered
integrity architecture in which gaming any single mechanism is made more difficult by
the presence of the others.

### Mechanism 1 — Standardized Cost Reporting

The foundational layer is mandatory, standardized, machine-readable cost disclosure.
All regulated providers, facilities, insurers, and SEC-participating entities report
cost and pricing data through the healthcare infrastructure layer on a defined cadence.

Required reporting categories include labor costs by category, capital costs with
depreciation methodology, equipment costs, pharmaceutical acquisition costs at invoice
price, administrative overhead with allocation methodology, malpractice coverage costs,
emergency readiness obligations, uncompensated-care exposure, debt-service obligations,
and bundled episode pricing.

Submissions are version-controlled, auditable, and linked to standardized service
taxonomy definitions so that cost categories are comparable across institutions. The
objective is comparability, not uniform pricing. A trauma center and a suburban primary
care clinic have genuinely different cost structures. The reporting system is designed
to make both structures visible and comparable to appropriate peers.

Cost submissions are signed using the submitting entity's SSI credential and carry a
statutory attestation obligation. Named officers of the submitting entity — not the
entity as an abstraction — certify that submitted figures accurately reflect actual
costs. Hospitals do not commit perjury; named officers do, and the attestation
structure is designed to make that accountability visible and personal. A chief
financial officer who certifies an inflated cost submission creates individual criminal
exposure that the entity cannot absorb on their behalf. That personal accountability
is the mechanism. An entity that inflates its cost submission to justify high pricing
simultaneously creates attributable evidence against its attesting officers when those
figures are compared against peer submissions.

What this defeats: The current system sustains pricing opacity by making it impossible
for any external observer to determine whether pricing reflects actual cost. When costs
must be disclosed in a standardized, auditable format with named-officer attestation,
the gap between stated cost and observed pricing becomes visible, and defending that
gap becomes a personal liability rather than a corporate communications exercise.

### Mechanism 2 — Nearest-Neighbor Benchmarking

Cost and pricing data are analytically meaningless in isolation. A hospital billing
$12,000 for a procedure may be exploiting a local monopoly or may be operating a
Level I trauma center in an underserved region with legitimate cost burdens that
justify the price. The nearest-neighbor benchmarking framework exists to make that
distinction tractable.

DoDA certifies benchmarking models that compare provider pricing and cost structures
against peer groups constructed from genuinely similar institutions. Comparison
dimensions may include metro region size, demographic structure, population density,
payer mix, labor-market conditions, chronic disease burden, trauma obligations, and
specialist availability. The methodology may use Euclidean nearest neighbors,
Mahalanobis distance, propensity-score matching, or successor methodologies that DoDA
certifies as producing valid peer comparisons.

The framework does not assume every hospital should cost the same. Trauma centers,
teaching hospitals, frontier access facilities, and rural emergency providers carry
genuine operational burdens that legitimately increase their costs. The nearest-neighbor
framework exists to identify unexplained variance — cost and pricing divergence that
exceeds what peer institutions with comparable obligations actually incur.

Peer group assignment is based on verified institutional characteristics reported
through standardized cost submissions and cross-referenced against external data
sources. Providers may not self-select into comparison groups. The methodology includes
anti-gerrymandering controls: a hospital cannot reclassify its reported service mix,
trauma designation, or population characteristics in ways designed to migrate it into a
softer comparison set. DoDA monitors for characteristic drift that correlates with
enforcement pressure and treats systematic drift as an anomaly warranting audit
escalation independent of the underlying cost comparison.

Where a provider or system materially exceeds regional and national comparison bands
without an explanation consistent with its disclosed cost structure, HETA may require
additional disclosure, trigger integrity review, analyze debt-service exposure, or
evaluate whether monopoly conditions rather than legitimate operational burden are
driving the divergence.

What this defeats: The use of institutional complexity, specialty status, and regional
market power to price above cost without any external reference point. Nearest-neighbor
benchmarking creates that reference without requiring central price-setting. The market
does not have uniform prices. It has observable prices and observable comparisons.

### Mechanism 3 — Direct-to-Consumer Standard Candles

Independent direct-to-consumer providers — surgery centers, imaging centers, diagnostic
clinics, transparent primary care practices — function in this framework as market
reference anchors. Their pricing, staffing models, throughput, and outcome-adjusted
cost structures serve as visible benchmarks for what comparable services cost when
delivered without the overhead of institutional billing complexity, opaque
insurer-provider negotiation, or facility-fee layering.

These are real providers operating in real markets. Their prices reflect actual
operating costs at competitive margins. When the gap between DTC reference pricing and
incumbent institutional pricing for comparable services is large, that gap requires
explanation. Sometimes the explanation is legitimate: the DTC provider does not carry
emergency readiness costs, uncompensated-care obligations, or teaching hospital
overhead. Those explanations are disclosable and appear in standardized cost reporting.
Where the gap exceeds what disclosed institutional burdens can account for, the residual
is a measure of administrative inflation, billing complexity rent, or monopoly
extraction.

HETA and DoDA may use standard-candle comparisons to flag provider systems for
enhanced disclosure, trigger integrity review, or recommend PCA restructuring pathways
where debt-service obligations are identified as a primary driver of the gap.

What this defeats: The use of institutional opacity to sustain pricing well above the
competitive market level for comparable services. Standard candles do not set prices.
They create public reference points that make the gap between institutional pricing and
competitive market cost visible to patients, employers, payers, and policymakers.

### Mechanism 4 — Legitimate Fragility vs. Monopoly Extraction

The nearest-neighbor and standard-candle mechanisms identify unexplained pricing
divergence. The framework then asks whether that divergence reflects legitimate
institutional fragility or exploitative pricing behavior, and responds differently to
each.

A hospital carrying unsustainable debt while providing essential regional access is a
problem that warrants direct, transparent support: PCA restructuring instruments,
refinancing pathways, temporary stabilization mechanisms, or explicit public subsidy
of the access obligations that justify its existence. Essential facilities should not
be required to survive by charging patients and employers inflated prices that neither
party can evaluate or contest. If emergency readiness capacity, rural access
obligations, or historical debt burdens require public support, those obligations
should be funded directly and visibly, with costs disclosed and outcomes measured.

An institution extracting monopoly rents through inflated pricing and administrative
complexity, without the legitimate operational burden that would justify the divergence,
warrants enforcement, antitrust referral, ownership transparency requirements, or
market access consequences. The framework does not confuse these two categories. Both
require intervention. The interventions are different, and forcing the distinction with
evidence is the mechanism's primary function.

Financial structures that conflict with public-purpose delivery — where returns are
extracted from care obligations rather than generated by service quality — may be
excluded or conditioned where they materially undermine access stability or cost
integrity. Those conditions and exclusions are applied through the service obligation
and participation frameworks, proportional to documented harm, not through categorical
prohibition.

What this defeats: The use of legitimate institutional fragility as cover for monopoly
extraction. Cost disclosure and peer comparison force the distinguishing question to be
asked with evidence. Facilities that need support get it through visible mechanisms.
Facilities that are extracting value through opacity face scrutiny calibrated to the
evidence.

### Mechanism 5 — Anti-Upcoding and Reclassification Enforcement

HETA maintains standing authority to detect and investigate systematic manipulation of
episode classification — the billing behaviors through which providers inflate
reimbursement by misrepresenting the clinical category of care delivered.

Targeted behaviors include emergency upcoding (billing market-layer urgent care
encounters as emergency events to access SEC reimbursement rates), retroactive severity
escalation (upgrading the documented clinical severity of an encounter after the fact
to justify higher billing), bundled-service fragmentation (unbundling services that
belong together into separately billed components), phantom facility-fee layering
(adding facility charges not disclosed at the point of care), shadow billing (billing
for services not delivered or not as described), and post-hoc reclassification of
routine market-layer services as SEC-covered severe events.

All SEC episode classifications are timestamped, logged, auditable, and linked to
standardized episode definitions in the Immutable Government Ledger. The classification
is recorded at the time of the clinical encounter and cannot be retroactively altered
without generating a documented reclassification event that is itself logged and
subject to review. Isolated anomalies are investigated before enforcement action is
taken. Systematic patterns, detected through DoDA's longitudinal monitoring functions,
do not wait for individual complaint. Consequences escalate from documentation requests
through audit escalation to reimbursement clawback, SEC participation suspension, and
referral for civil or criminal enforcement where the pattern supports it.

What this defeats: The use of clinical coding as a revenue optimization tool rather
than an accurate record of care delivered. The timestamped, immutable ledger makes
retroactive manipulation detectable. Pattern detection makes systematic abuse visible
even when individual instances are designed to look like isolated errors. The
escalating consequence structure makes the expected cost of systematic gaming exceed
the expected revenue from it.

### Mechanism 6 — SEC Boundary Integrity

The distinction between market-layer care and Severe Event Coverage is the structural
spine of the reformed healthcare system. If routine care migrates into SEC through
reclassification gaming, price discovery collapses and administrative claims warfare
re-emerges inside the SEC layer. If catastrophic care migrates into market-layer
exposure through under-coverage, the financial protection that SEC is designed to
provide fails precisely when patients need it most.

HETA's SEC Boundary Authority maintains permanent responsibility for episode
classification integrity, anti-gaming enforcement at the market-SEC interface,
emergency utility pricing oversight, and actuarial boundary stewardship. Boundary
decisions are publicly documented, version-controlled, and periodically reviewed.
Changes to episode boundary definitions follow the transparent, versioned process
described in the SEC administration framework: published in advance, subject to public
comment, logged in the Immutable Government Ledger.

The boundary is enforced structurally through the payment rail architecture. A
market-layer service code does not trigger SEC reimbursement routing. A SEC-covered
episode code triggers SEC routing, validation, and the full suite of cost transparency
and rate-band requirements that apply to regulated emergency utility services. Providers
cannot simply choose which routing to request — the clinical escalation codes that
trigger SEC coverage are defined by episode classification, and misclassification is
detectable against the timestamped ledger record of what care was actually delivered.

What this defeats: The selective use of clinical reclassification to access
higher-reimbursement SEC coverage for services that belong in the competitive market
layer, undermining price discovery in that layer and actuarial integrity in the SEC
pool. Structural rail enforcement makes this gaming technically difficult. Timestamped
classification logging makes it permanently detectable.

### Mechanism 7 — Insurer Anti-Denial Architecture

Under the legacy system, denial complexity functions as a profit mechanism. Insurers
can improve their financial position by denying, delaying, or administratively
complicating claims in ways that wear down patients and providers into accepting less
than coverage entitles them to. The leverage underlying this mechanism is catastrophic
financial exposure: the threat that disputing a denial risks losing access to coverage
for a severe medical event produces capitulation that has nothing to do with whether
the denial was justified.

This framework removes that leverage structurally. SEC is a universal catastrophic
floor that operates independently of supplemental insurance status. Supplemental
insurers cannot threaten access to catastrophic protection during a coverage dispute,
because catastrophic protection is not theirs to withhold. SEC remains the payer of
record for covered severe events regardless of supplemental plan status. Direct-care
markets remain accessible for market-layer services regardless of supplemental
enrollment.

The commercial consequence operates at the level of employer plan selection and
household enrollment decisions, not in the moment of care. Patients are not actively
choosing supplemental insurers during a medical crisis. The leverage point is
enrollment and renewal: an employer whose workforce has experienced repeated
administrative friction from a supplemental insurer can move its coverage at renewal
without exposing employees to catastrophic financial risk during the transition.
A household that has experienced denial-pattern behavior faces a genuinely lower cost
of exit than under the legacy system, because catastrophic protection does not leave
with the plan. In a market where SEC performance benchmarking publishes four-test
results across all supplemental plans — risk transfer, value add, actuarial honesty,
complexity — denial-pattern behavior is publicly visible at the moment enrollment
decisions are made.

Denial-based business models become commercially unsustainable when the captive
leverage that sustained them is removed and when performance data is public at the
point of choice.

What this defeats: The commercial exploitation of catastrophic financial exposure as
leverage for denial, delay, and administrative attrition. The structural removal of
that leverage changes the competitive economics of the supplemental insurance market
from one where complexity is profitable to one where service quality and reduced
friction are the durable competitive advantages.

### Mechanism 8 — Vendor and Software Integrity

If the reformed healthcare system runs on standardized rails and produces its integrity
through machine-readable data, then the software and vendors that generate, format, and
transmit that data become a strategic attack surface. EHR vendors, billing middleware
providers, revenue-cycle management firms, and coding software developers occupy
chokepoints in the data flow. A vendor whose software systematically optimizes for
upcoded outputs, obscures price transparency requirements, blocks API compliance through
proprietary lock-in, or presents billing interfaces designed to generate favorable
coding can undermine the integrity architecture without any individual provider making
an explicit decision to game the system.

Revenue-cycle management software and coding tools used by regulated providers and
facilities must comply with interface standards published by HETA and DoDA. Prohibited
design features include dark-pattern billing interfaces that default toward upcoded
outputs, proprietary data formats that block required API compliance, coding suggestion
engines that systematically recommend higher-severity classifications without clinical
basis, and interfaces that obscure or suppress required price transparency fields.
Compliance is a condition of use by regulated entities, and HETA maintains authority
to audit vendor software and the output patterns it generates.

Vendors whose software produces systematic output anomalies — coding distributions that
diverge from clinical peer norms in ways that correlate with revenue rather than
clinical complexity — face the same escalating scrutiny as providers whose billing
patterns diverge from peer benchmarks. A vendor cannot disclaim responsibility for
output distributions that are the predictable result of its system's design choices.

What this defeats: The use of software architecture and vendor design as a passive
gaming mechanism — one in which no individual provider or officer makes a specific
decision to commit fraud, but in which the collective output of vendor-optimized coding
and billing behavior systematically inflates costs, obscures prices, and degrades the
data quality that the integrity architecture depends on.

### Mechanism 9 — Ownership Transparency and Anti-Consolidation

All participating providers and insurers must disclose ownership structures, referral
relationships, private-equity control, cross-ownership arrangements, and material
financial conflicts. This is a condition of participation, not a voluntary disclosure.

HETA and DoDA monitor regional consolidation patterns, referral concentration,
anti-competitive acquisition behavior, and local market foreclosure using the same
nearest-neighbor and longitudinal monitoring infrastructure that underlies cost
benchmarking. Where consolidation materially undermines market competition or access
stability, HETA may block participation privileges, trigger enhanced review, recommend
antitrust referral, or condition PCA support on structural restructuring requirements.

Vertical integration that generates genuine clinical value — care coordination, shared
clinical infrastructure, population health management — is distinguishable from
vertical integration that generates financial value primarily through referral capture,
network foreclosure, and competitive exclusion. The disclosure and monitoring
requirements create the visibility needed to make that distinction. The enforcement
authority creates the consequence structure that makes the distinction matter.

What this defeats: The use of acquisition strategy and referral network control to
neutralize market competition before transparent pricing and anti-gaming enforcement
have a chance to function. Markets require competitors. Ownership transparency and
anti-consolidation enforcement protect the competitive structure that makes the other
eight mechanisms possible.

---

## Escalation to Coordinated Deceptive Enterprise Designation

The nine mechanisms described above address the full range of individual and
organizational gaming behaviors that the reformed healthcare system is designed to
resist. Most of that gaming — upcoding, reclassification, consolidation, vendor
optimization, denial complexity — operates at the level of institutional incentive
misalignment. The framework corrects those incentives through transparency requirements,
peer benchmarking, structural enforcement, and commercial consequence.

A distinct category of conduct sits above this threshold. Where gaming behavior is not
the product of misaligned incentives operating independently across an organization,
but is instead the product of deliberate coordination — planned across actors, sustained
over time, concealed through structural mechanisms, and directed at producing material
harm to the public or to the integrity of the healthcare system — it becomes a candidate
for designation as a Coordinated Deceptive Enterprise under the CDE Enforcement
Framework.

The CDE Framework is a separate instrument. It is not a healthcare-specific framework
and is not administered by HETA. What this section establishes is the referral pathway
and the conditions under which healthcare-sector conduct crosses from gaming into
coordinated deception.

CDE designation in the healthcare context requires all five elements defined in the CDE
Framework: enterprise coordination across multiple actors, internal knowledge that
contradicts public-facing conduct, a pattern of sustained action rather than isolated
incidents, material impact on public health or market integrity exceeding domain-specific
published thresholds, and concealment through structures designed to obscure origin or
intent. No single element, and no combination of fewer than five, triggers CDE
liability.

In the healthcare context, the conduct patterns most likely to meet this threshold
include the following. A hospital system or insurer that systematically coordinates
upcoding across facilities while maintaining internal documentation demonstrating
awareness of the practice — knowledge contradicting the public-facing billing narrative
— satisfies elements 1, 2, and 3. If the coordination produces material harm to the
SEC risk pool or to patients, and the structure is designed to obscure the coordination,
all five elements are present. A pharmaceutical manufacturer or PBM that coordinates
cost attestation submissions across affiliated entities to produce a false cost baseline
for recoupment calculation, while internal records document the actual cost structure,
similarly presents a five-element pattern. A vendor network that coordinates the
distribution of billing optimization software designed to generate systematic upcoding,
while marketing the software as a compliance tool, may satisfy all five elements where
the coordination, internal knowledge, and concealment mechanism are documentable.

The organizational knowledge aggregation clause of the CDE Framework is particularly
relevant in healthcare contexts. Healthcare organizations are complex, and it is
structurally possible for senior leadership to compartmentalize awareness of systematic
fraud so that no individual holds complete knowledge of the coordinated conduct while
the organization as a whole operates on it. The CDE Framework explicitly forecloses
this defense: deliberate compartmentalization does not constitute a defense where the
aggregated evidence, across documented communications and decision-making processes,
establishes that the organization possessed the required internal knowledge
contradiction. Healthcare entities that construct information flows designed to ensure
plausible deniability for senior officers while sustaining systematic gaming at the
operational level are not insulated by that structure.

The referral pathway runs from HETA to the CDE enforcement body through DoDA. HETA's
longitudinal monitoring and anomaly detection functions generate the evidentiary record.
Where that record, assessed against the five-element test, produces findings that meet
or approach the clear and convincing standard required for CDE designation, HETA refers
to DoDA for verification and trigger class assessment. DoDA's output is an evidentiary
input to the CDE enforcement process, not a determination. Final CDE designation
proceeds through the CDE Framework's adjudication process with full due process
protections. HETA does not make CDE designations and cannot impose CDE consequences
through its own authority.

The existence of this escalation pathway matters for the anti-gaming architecture even
in cases that never reach CDE designation. The knowledge that organizational-level
coordination of fraud schemes is a candidate for enterprise-level joint and several
liability — not just regulatory penalty — changes the risk calculus for organizations
considering whether to allow, coordinate, or institutionalize gaming behavior. The
nine mechanisms create consequences for individual violations. The CDE escalation
pathway creates consequences for the decision to make violation a deliberate
organizational strategy.

---

## Institutional Anti-Capture Design

The anti-gaming architecture is only durable if the institutions operating it are
themselves resistant to capture by the entities they regulate. Healthcare incumbents
have strong financial incentives and substantial organizational capacity to capture
regulatory processes — through revolving-door employment, strategic litigation,
regulatory comment flooding, and long-term relationship cultivation with enforcement
personnel.

Three institutional design features address this.

The first is the DoDA independence architecture. DoDA certifies the methodologies
underlying benchmarking, cost comparison, anomaly detection, and audit systems. HETA
operates those systems against the certified methodology. DoDA audits HETA's adherence
to the certified methodology on a defined schedule and publishes findings. If HETA's
practices diverge from DoDA's methodology, DoDA flags it publicly and Congress receives
notification through the cost performance backstop reporting cycle. This separation
prevents the operating institution from certifying its own methodology, and prevents a
captured operating institution from quietly degrading the standards it applies.

The second is rotating integrity review. HETA operates rotating audit and integrity
review teams with mandatory geographic, organizational, and functional rotation
schedules. Review personnel may not maintain undisclosed financial relationships with
reviewed entities, accept post-service employment within defined cooling-off windows,
or participate in review of institutions where direct conflicts exist. Rotation
schedules are auditable and public. Long-term dependency relationships between
enforcement personnel and regulated entities are the primary mechanism through which
regulatory capture operates. Rotation disrupts those relationships before they become
deference.

The third is public reporting. Aggregate audit findings, pricing distributions, outlier
frequency, SEC boundary disputes, insurer denial metrics, vendor compliance findings,
and enforcement outcomes are published publicly on a recurring basis. The public should
be able to observe whether the healthcare system is functioning honestly. When that
observation is possible, the political cost of allowing enforcement to degrade becomes
real. Captured enforcement agencies sustain capture most easily when their operations
are invisible. Public reporting makes the quality of enforcement an observable fact
rather than an institutional claim.

---

## Blind Subsidy and Payment Logic

Where public subsidies, employer contributions, and affordability supports apply,
settlement occurs through the unified payment rail without exposing the full payer
composition to providers. Providers receive payment confirmation, not household
financial profiles. The subsidy arithmetic is invisible to the provider by architectural
design rather than by discretionary policy. Providers who can see patient subsidy status
will price to subsidy rather than to market, tier availability by payment level, and
recreate the two-tier access dynamics the market-layer reform is designed to eliminate.
Architectural enforcement is not gameable in the way that policy-level rules are.

---

## Post-Hoc and Surprise Billing Prohibition

All regulated payments settle through the unified payment rail with known pricing,
verified eligibility, and final settlement terms established prior to service except
in defined emergency conditions where the patient cannot consent at the point of care.
Post-hoc balance billing, retroactive surprise billing, and delayed insurer liability
reassignment are prohibited as structural properties of the payment architecture, not
as aspirational compliance standards.

The emergency exception is bounded. Emergency care is governed by the utility
regulation framework, which imposes cost transparency and rate-band requirements
precisely because emergency providers know patients cannot negotiate at the moment of
crisis. Surprise billing prohibition in the emergency layer operates through rate-band
enforcement rather than through pre-service price consent that is clinically impossible
to obtain.

---

## Enforcement Philosophy

This framework is not anti-provider. It is not anti-insurer. It is anti-opacity.

Providers delivering legitimate care at legitimate cost should face less administrative
burden under this system than under the legacy system, because the legacy system
generated administrative complexity not as a byproduct of care delivery but as a
revenue optimization mechanism that all parties were forced to participate in. A
provider whose cost structure can withstand examination has nothing to fear from
transparent cost reporting, nearest-neighbor benchmarking, or standard-candle
comparisons. Scrutiny is calibrated to unexplained variance, not to variance per se.

Insurers offering superior supplemental products — genuine reduction in patient
financial exposure, faster care navigation, lower administrative friction, demonstrably
better outcomes — can compete and profit transparently above the SEC floor. The
framework does not prevent supplemental insurance from being commercially viable. It
prevents supplemental insurance from being commercially viable primarily through denial
complexity and catastrophic leverage rather than service quality.

The framework intervenes where opacity replaces price discovery, where monopoly
replaces competition, where denial replaces service, or where administrative gaming
replaces care delivery. That is the scope of its enforcement mandate. Enforcing that
scope is what makes the reformed system capable of functioning as designed.

---

## Relationship to Other Frameworks

This framework operates in conjunction with the HETA Revised Charter, the Healthcare
Infrastructure Layer, the SEC Insurance Architecture, the Cost Performance Backstop,
the Employer Coverage Transition Framework, the SEC Administration and HETA
Steady-State Operating Model, and the Coordinated Deceptive Practices Enforcement
Framework. The anti-gaming architecture is the enforcement layer that makes the market
design, the SEC floor, and the insurance architecture resistant to erosion over time.
The CDE Framework is the escalation pathway for conduct that moves beyond misaligned
incentives into deliberate organizational coordination of deception. Markets without
integrity enforcement do not stay honest. Insurance floors without boundary enforcement
get gamed into irrelevance. Cost transparency without consequence for misrepresentation
becomes optional disclosure. Organizational fraud without enterprise-level liability
becomes a manageable cost of doing business. This framework is the part of the system
that ensures none of those degradations happen quietly.
