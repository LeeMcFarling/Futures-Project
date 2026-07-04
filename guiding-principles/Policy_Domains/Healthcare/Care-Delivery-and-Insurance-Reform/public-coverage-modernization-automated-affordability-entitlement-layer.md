---
id: public-coverage-modernization-automated-affordability-entitlement-layer
title: Medicaid and Medicare Modernization — Automated Public Coverage Layer
sidebar_label: Public Coverage Modernization
sidebar_position: TBD
slug: /healthcare/care-delivery/public-coverage-modernization
domain: Healthcare
subdomain: Care_Delivery_and_Insurance
policy_type: Affordability Infrastructure Framework
status: Draft
phase: 2
version: 0.1
author: Futures Project
last_updated: 2026-05-03
dependencies:
  - care-delivery-market-design
  - insurance-architecture-sec
  - healthcare-infrastructure-layer
  - benefits-gradient-modernization
  - permanent-health-security-accounts
  - dental-care-hta-actuarial-integration
  - maternal-family-care-hta-integration
  - ssi-self-sovereign-identity-framework
  - upi-privacy-preserving-payment-rail
  - department-of-data-and-accountability
  - immutable-government-ledger
  - government-outflow-integrity-framework
related_initiatives:
  - regional-health-center-network
  - cost-performance-backstop
  - labor-stack-enforcement-framework
  - sec-administration-heta-steady-state
  - portable-healthcare-contribution-floor
tags:
  - healthcare
  - medicaid
  - medicare
  - affordability
  - income-gradient
  - chronic-illness
  - market-layer
  - sec
  - ssi
  - upi
  - fraud-detection
  - automated-eligibility
---

## Purpose and Scope

This brief defines how Medicaid and Medicare functions are modernized under the
restructured healthcare framework. The statutory guarantees are preserved. Medicaid
remains the affordability guarantee for low-income and medically vulnerable
populations. Medicare remains the age- and disability-linked public healthcare
entitlement. The delivery mechanism changes.

Under the restructured system, both programs operate through a shared public coverage
layer executed by the healthcare rail. Eligibility is verified through
privacy-preserving attestations. Market-layer affordability and entitlement support
is applied automatically at settlement. SEC covers severe, acute, medically necessary,
and high-cost events according to clinical trigger rules. Providers receive confirmed
payment and standardized service codes without seeing whether support originated from
Medicaid, Medicare, employer contributions, public credits, or household funds.

The purpose is not to abolish Medicaid or Medicare. It is to preserve their statutory
commitments while removing the administrative fragmentation, provider stigma,
duplicative claims machinery, and program-specific care silos that make public
coverage difficult to use and expensive to administer.

Medicaid becomes automatic. Medicare remains Medicare — the card still means
guaranteed public coverage. The backend gets simpler. Those are the bridge phrases.

This brief defines the three-tier Medicaid affordability gradient, the Medicare
automated entitlement layer, how both operate through the SSI and UPI infrastructure,
how the chronic illness problem is addressed, the federal-state fiscal interface, the
continuity protections during transition, and the fraud and gaming controls that
protect the system from provider attestation schemes and organized abuse. Full
program-specific policy details — Medicare Advantage unwind, prescription drug
coordination, age and disability entitlement treatment, and SEC coordination rules —
are addressed in companion documents. The shared architecture belongs here.

---

## The Statutory Continuity Argument

Medicaid and Medicare exist as distinct statutory guarantees with different legal
foundations, different constituencies, and different political histories. Medicaid is
a means-tested affordability guarantee — Congress established it to ensure that income
does not determine access to healthcare for low-income and medically vulnerable
populations. Medicare is an earned social-insurance entitlement — Congress established
it to guarantee healthcare access for older Americans and people with qualifying
disabilities regardless of current income.

Neither guarantee disappears under this framework.

What disappears is the bureaucratic delivery apparatus that has accumulated around
both guarantees — separate enrollment universes, distinct provider participation
regimes, managed care intermediary layers that extract administrative rent, cliff-based
eligibility structures, provider stigma, and program-specific care silos that make
public coverage difficult to use and expensive to administer.

For Medicaid, the redistributive function survives. The eligibility maze does not.
For Medicare, the entitlement guarantee survives. The claims bureaucracy gets simpler.
For both, the shared public coverage rail replaces program-specific administrative
machinery without replacing the programs themselves.

The deeper principle is this: legacy public healthcare programs stop functioning as
separate care universes and become rail-executed affordability, risk, and settlement
functions. Different statutory guarantees. Common execution layer. That is what
modernization means here.

---

## Core Design Principle

In this framework, Medicaid-derived support does not operate as a separate
bureaucratic coverage silo. It operates as an automated affordability layer applied
through the healthcare rail.

Income eligibility is verified through privacy-preserving attestation. Clinical-need
adjustments, where authorized, are verified through purpose-bound health attestations.
The rail applies the relevant discount, credit, or account enhancement at settlement.

The patient sees the net price before booking and at checkout. The provider receives
the confirmed settlement amount and standardized service code. The provider does not
see Medicaid status, income tier, subsidy amount, clinical-condition attestation, or
payer mix.

This design preserves the redistributive function of Medicaid while removing the
legacy administrative form. Provider stigma cannot operate when the provider cannot
see which patients receive Medicaid support. Cliff effects cannot operate when
eligibility is a continuous gradient rather than a binary threshold. Enrollment
friction cannot operate when eligibility is verified automatically through SSI
attestation rather than through a separate application process.

Medicaid support becomes automatic price reduction, not a separate care system.

---

## The Three-Tier Gradient

The affordability layer operates through three tiers that can apply individually or
in combination depending on the patient's income and clinical situation.

### Tier 1 — Income Gradient

The income gradient is the foundational tier. It applies to every market-layer
service for every patient whose income attestation places them within the gradient
range. No clinical information is required. No separate enrollment is required. The
patient's SSI credential holds the income attestation, the rail reads it at
settlement, and the discount applies automatically.

The gradient is continuous, not binary. A patient at 150% of the federal poverty
level receives a larger discount than a patient at 250% FPL, who receives a larger
discount than a patient at 350% FPL. There is no income threshold at which support
suddenly disappears. The slope is calibrated so that additional earnings never
produce a net loss in household resources — the discount phases down in proportion to
income growth, coordinated with the benefits gradient framework governing all other
support programs.

Income attestation is updated on a defined cadence through the SSI layer. DoDA
monitors whether the gradient calibration is producing cliff effects at any income
band and adjusts thresholds through a defined rulemaking process. The gradient is a
living instrument, not a fixed schedule.

### Tier 2 — Income Plus Acute Clinical Need

The second tier adds a condition-sensitive component for situations where a specific
clinical circumstance creates a one-time or episodic affordability problem at the
market-layer boundary. The endodontic example from the dental brief is the clearest
case: a root canal is market-layer care by design — predictable, schedulable, not
SEC-appropriate — but the out-of-pocket cost at market rates may be sufficient to
produce harmful deferral for a patient whose income gradient discount does not fully
cover it.

In these cases, a purpose-bound clinical-need attestation through the patient's SSI
health wallet activates an enhanced, time-bounded discount on top of the standard
income gradient. The attestation confirms that the patient has a clinical condition
or pathway that generates elevated market-layer exposure for a defined service
category. It does not disclose the underlying diagnosis to the provider, the employer,
or any entity beyond what is required for settlement, audit, and fraud prevention.

Tier 2 activations are event-specific and time-bounded. They are not a permanent
reclassification of the patient's cost basis. A patient receiving a Tier 2 enhanced
discount for an endodontic procedure does not carry that enhancement forward to
unrelated services. The activation is proportional, temporary, and recalibrated as
the clinical situation resolves.

Tier 2 is also the mechanism for the boundary cases identified in the maternal brief
and elsewhere: high-risk pregnancy monitoring that is technically schedulable but not
genuinely optional, postpartum services with elevated clinical need, and similar
situations where the market-layer classification is correct but the affordability
assumption is not.

### Tier 3 — Income Plus Chronic Condition

The third tier addresses the chronic illness problem directly. A patient managing
diabetes, hypertension, a serious mental health condition, a chronic autoimmune
disease, or any other ongoing condition has predictable, recurring, non-emergency
care needs across multiple service categories. Those needs are market-layer by
design — they are schedulable, manageable, not acute. But the cumulative cost of
managing a chronic condition over time is not affordable at market rates for most
low- and middle-income patients, and the current system's response to this — narrow
Medicaid networks, prior authorization burdens, coverage gaps — predictably produces
the expensive acute events the system was supposedly preventing.

Tier 3 recalibrates the patient's effective market-layer cost basis across the
relevant service categories for as long as the condition persists and their income
warrants it. This is not a one-time enhanced discount. It is a persistent adjustment
to what routine care costs for that patient, reflecting the clinical reality that
managing their condition is not optional and not episodic.

DoDA certifies which conditions qualify for Tier 3 based on evidence of cumulative
market-layer exposure, documented relationship between routine management and
prevention of severe-event escalation, and actuarial analysis of expected downstream
cost reduction. The list is evidence-based and updated on a defined cadence. HETA
configures the rail logic for each certified condition category. The patient receives
the recalibration automatically once their condition attestation and income
attestation are verified through SSI.

Tier 3 is the chronic illness fix. A diabetic patient is not just getting a discount
on today's endocrinology appointment. Their entire routine care cost structure across
relevant categories — primary care, diagnostics, medication management, dietary
support, ophthalmology, podiatry — is adjusted to reflect the reality of their
clinical situation. That adjustment persists. It renews as long as the condition is
attested and income warrants it.

This is what Medicaid was always trying to do for people with chronic conditions. The
difference is that it does it automatically, without a separate enrollment universe,
without narrow networks, without provider stigma, and without the managed care
intermediary extracting margin in the middle.

---

## How It Operates Through the Rail

From the patient's perspective, the affordability layer is invisible in the best
possible sense. The patient opens the app, searches for a provider, sees their net
price, books an appointment, and pays that price. The income gradient, clinical-need
enhancement, and chronic condition recalibration have all been applied before the
price appears. The patient does not apply for Medicaid. They do not present a
Medicaid card. They do not navigate a separate eligibility portal. Their SSI
credential carries the relevant attestations and the rail does the arithmetic.

From the provider's perspective, the patient is a patient. The provider receives a
confirmed payment amount and a standardized service code. They do not see which tier
applied, what the patient's income is, whether a clinical-need attestation was
involved, or what the public contribution to the settlement was. Provider stigma
cannot operate on information the provider does not have.

From the system's perspective, the rail applies a defined sequence: check income
attestation and apply Tier 1 gradient, check clinical-need attestation and apply
Tier 2 enhancement if active, check chronic condition attestation and apply Tier 3
recalibration if active, combine with HTA balance and employer contributions, display
net price to patient, settle through UPI to provider. The sequence is automated,
auditable, and logged through the immutable ledger without recording personal
attribute data beyond what is necessary for settlement and audit.

---

## The Chronic Illness Fix

It is worth stating this directly because it is the most important thing this
framework does that the current system consistently fails to do.

Chronic illness is expensive to manage and catastrophically expensive to neglect. The
current system creates financial incentives to neglect it. Medicaid patients with
chronic conditions navigate narrow networks that frequently exclude the specialists
and services they need. Prior authorization burdens delay treatment. Coverage gaps
create periods of unmanaged disease. The result is preventable hospitalizations,
avoidable complications, accelerated disease progression, and ultimately the
expensive severe events that SEC was designed to cover.

Tier 3 breaks that cycle by making ongoing disease management genuinely affordable
rather than nominally covered. A patient who can actually afford their primary care
visits, their diagnostic monitoring, their medication management, and their specialist
consultations will manage their condition. A patient who faces financial barriers to
routine management — even modest ones — will defer, and the deferral will compound
into crisis.

The actuarial logic is straightforward. DoDA measures the expected downstream
severe-event cost reduction associated with adequate routine management of each
certified chronic condition. That expected savings is the calibration basis for the
Tier 3 recalibration. The system is paying a known, bounded cost now to avoid a
larger, probabilistic cost later. That is what preventive investment means. It is
also, coincidentally, what Medicaid was always supposed to deliver and rarely has.

---

## Federal-State Fiscal Interface

Medicaid modernization preserves the federal-state fiscal structure during transition
while standardizing the affordability function through the healthcare rail. This
section does not fully resolve the intergovernmental fiscal relationship — that work
belongs in the Healthcare Transition and State Pilot Framework and the forthcoming
Medicare modernization brief. But the attack surface is large enough to name
explicitly here.

States do not operate separate market-layer provider networks under this framework.
Their role shifts toward fiscal participation, eligibility-data coordination where
required, state regulatory alignment, and monitoring of access conditions inside their
jurisdiction. State Medicaid agencies are not abolished — they are reoriented from
enrollment and network administration toward oversight, data coordination, and access
accountability within their jurisdictions.

Federal matching funds may be converted into rail-applied affordability support for
eligible residents, subject to maintenance-of-effort rules, anti-supplantation
safeguards, and DoDA reporting. States may provide additional affordability support
above the federal floor through their own matching contributions, but may not
recreate cliff-based eligibility, provider-visible Medicaid status, narrow networks,
or separate enrollment systems for market-layer care. The federal floor is a floor.
States can build above it. They cannot rebuild the maze below it.

Governors and state legislatures retain substantial political stake in the transition.
That stake is legitimate — states have co-invested in Medicaid for decades and carry
real fiscal exposure. The transition framework should treat state fiscal stability
as a constraint, not an afterthought. During pilot phases, state fiscal exposure,
federal match treatment, and transition stabilization payments are governed by the
Healthcare Transition and State Pilot Framework. States that enter pilots early carry
transition risk; the federal backstop is designed to make that risk manageable.

The predictable attack vector is a governor or state Medicaid director claiming that
the automated affordability layer does not deliver equivalent coverage for their
residents and using that claim to resist or delay transition. The defense against
that attack is the continuity protection framework defined below and the DoDA
certification requirement — states cannot be certified as transitioned until the
affordability layer is demonstrated to provide equal or better functional access.
That certification is not discretionary and is not controlled by the state.

---

## Continuity Protection During Transition

No current Medicaid beneficiary loses access to covered care because their state or
region enters a pilot. During transition, legacy Medicaid coverage remains available
until the automated affordability layer is certified to provide equal or better
functional access for the relevant service category.

Certification requires demonstrated provider availability, net-price visibility for
the relevant service category, rail settlement reliability, accessible appeal
pathways for coverage disputes, and continuity for ongoing treatment relationships.
A beneficiary managing an active chronic condition does not transition off legacy
Medicaid coverage for that condition until Tier 3 recalibration is active and
certified for their service categories.

The transition is service-category specific. Dental, maternal care, primary care,
behavioral health, chronic disease management, and prescription support may move at
different speeds depending on provider readiness, rail infrastructure maturity, and
access conditions in the relevant region. A service category that is ready in an
urban pilot district may not be ready in a rural region within the same state.
Certification is granular enough to reflect that variation.

Patients with ongoing treatment relationships — an established psychiatrist, a
primary care physician managing a complex chronic condition, an oncologist mid-course
— retain access to those relationships through the transition window. Continuity of
care is not sacrificed for administrative convenience.

DoDA monitors continuity outcomes from the beginning of pilot deployment. Any
demonstrated gap between legacy Medicaid access and automated affordability layer
access for a certified service category triggers automatic escalation to HETA and
the relevant state Medicaid agency. The burden of proof is on the transition, not
on the beneficiary.

---

## Medicare Function — Automated Entitlement Layer

Medicare-derived support operates as an age-, disability-, and statutory-status-based
entitlement layer applied through the same healthcare rail. Medicare beneficiaries do
not enter a separate provider universe for market-layer care. They use the same
provider marketplace, app, price display, and settlement rail as other patients. Their
Medicare entitlement is verified through SSI attestation and applied at settlement
according to statutory rules.

Where a service is SEC-covered, SEC remains the severe-event floor and Medicare
coordination rules determine fiscal responsibility between the entitlement layer and
the SEC risk pool. Where a service is market-layer care — including dental, vision,
hearing, and other services not currently covered by traditional Medicare — the rail
applies Medicare-derived support, income-gradient support where applicable, HTA or
Health Security Account balances, and any authorized supplemental coverage before
displaying the patient's net price.

The provider receives a confirmed settlement amount and standardized service code.
The provider does not see whether payment support originated from Medicare, Medicaid,
employer contributions, public credits, or patient account balances unless disclosure
is legally required for a narrow operational purpose.

Medicare's administrative apparatus — claims processing, provider credentialing, the
Medicare Advantage plan review and marketing infrastructure — is rationalized over
time through the same SSI, UPI, and immutable ledger infrastructure that underlies
the broader healthcare reform. Provider reimbursement flows through UPI. Claims
adjudication simplifies as episode boundaries are standardized. The audit trail is
permanent and attributable. Medicare Advantage unwinding, prescription drug
coordination, and the full treatment of age and disability entitlement rules are
addressed in companion documents.

The political logic of Medicare is distinct from Medicaid and must be handled
carefully. Medicare beneficiaries are extremely sensitive to anything that sounds like
replacement, voucherization, or means-testing — and rightly so given the program's
history and the attacks it has faced. The language must be conservative even as the
architecture converges. Medicare remains Medicare. The card still means guaranteed
public coverage. The backend gets simpler. That is the message, and it should not be
complicated by premature policy detail.

Two things are true simultaneously and must both be said clearly. First, Medicare
and Medicaid are different statutory guarantees with different legal and political
foundations — they are not the same program and should never be described as such.
Second, in the modernized architecture, both use the same execution layer: SSI for
eligibility attestation, UPI for settlement, SEC for severe-event protection, and
the healthcare rail for market-layer care. Different guarantees. Common plumbing.
That distinction is the entire argument.

---

## Fraud and Gaming Controls

The affordability layer creates predictable fraud incentives that must be explicitly
addressed. The most serious risk is not individual patient gaming — income
attestation is based on verified records, and false attestation carries legal
consequences. The more serious risk is provider-side attestation schemes: a provider
or provider network generating systematic clinical-need attestations or chronic
condition attestations to activate enhanced discounts for patients who do not qualify,
effectively milking the Tier 2 and Tier 3 systems for revenue.

The pattern signature for this abuse is distinctive and detectable. A provider
generating chronic-condition attestations at rates significantly above their regional
peer group, relative to their patient population demographics and prior utilization
history, stands out in the data. A provider whose attestation volume spikes shortly
after Tier 3 activations begin generating enhanced settlements stands out in the
data. A network of providers with coordinated attestation patterns and correlated
settlement timing stands out in the data.

Detection operates through the same architecture defined in the Government Outflow
Integrity Framework. Domain-specific models are trained on confirmed provider
attestation fraud cases. The immutable ledger records every attestation-linked
settlement permanently — fraud committed today is subject to the detection
capabilities of every future year applied to a record that does not change. DoDA
monitors provider attestation volume, condition mix, attestation renewal rates, and
the correlation between attestations issued and downstream utilization patterns.
Anomalies are flagged automatically and routed to human investigators who make
findings. No automated system issues a determination.

Three additional controls are specific to the clinical attestation context.

First, attestation integrity at the credential level. A clinical-need or chronic
condition attestation can only be generated through a credentialed clinical encounter
with a licensed provider. The patient cannot self-attest a chronic condition. The
clinician who generates the attestation is identified by their SSI credential in the
rail record. That attribution is permanent and auditable. A clinician who generates
false attestations is personally identifiable in the ledger.

Second, cross-domain signal triangulation. Because SSI and UPI connect healthcare,
labor, and benefits data at the infrastructure level, the system can detect
coordination schemes that span domains — a provider network generating attestations
that correlate with employer contribution avoidance patterns, or attestation mills
that appear simultaneously across multiple benefit categories. The immutable ledger
makes cross-domain patterns permanent and auditable in ways that siloed systems
cannot achieve.

Third, renewal scrutiny. Chronic condition attestations require periodic renewal.
A patient whose condition resolves but whose attestation is renewed without supporting
clinical evidence is a detection signal. A provider who renews attestations at
unusually high rates without corresponding clinical visit records is a detection
signal. Renewal patterns are monitored through the same aberrance detection
infrastructure as initial attestation volume.

Consequences for confirmed provider attestation fraud are severe. Civil penalties,
recovery of enhanced settlements, suspension from rail participation, and criminal
referral where the pattern supports it. The framework is explicit that the
affordability layer exists to serve patients with genuine need, and that fraudulent
attestation schemes divert resources from those patients and undermine the public
legitimacy of the gradient. The deterrent must be proportional to that harm.

---

## What This Is Not

This is not the abolition of Medicaid. The statutory guarantee survives. The
redistributive commitment survives. What does not survive is the administrative
apparatus that has made Medicaid difficult to use, stigmatizing to receive, and
expensive to administer.

This is not a high-deductible affordability scheme. The gradient does not require
patients to absorb a large out-of-pocket threshold before support activates. It
applies from the first dollar of market-layer exposure, proportional to income.

This is not a managed care intermediary model. There is no Medicaid managed care
organization extracting administrative margin between the patient and the provider.
The rail applies the discount directly. The savings from eliminating the intermediary
layer go to lower net prices for patients, not to plan administration overhead.

This is not a narrow network. Patients with income-gradient support use the same
market-layer provider pool as every other patient. They see the same prices, compare
the same options, and book through the same app. Provider-side blindness to Medicaid
status means there is no separate Medicaid network to be excluded from.

This is not a wellness program or a behavioral incentive scheme. The Tier 2 and Tier
3 clinical-need components are triggered by medical condition, not by compliance with
lifestyle or behavior requirements. A patient with diabetes receives Tier 3 support
because they have diabetes, not because they have demonstrated satisfactory
glycemic control.

This is not a surveillance system. The clinical attestations are purpose-bound and
privacy-preserving. Employers cannot see them. Providers cannot see them beyond what
is necessary for clinical care. The rail processes them and discards what is not
needed for settlement and audit.

---

## Bottom Line

The current Medicaid and Medicare systems fail the people they are designed to serve
in overlapping and well-documented ways: enrollment cliffs that punish income growth,
narrow networks that exclude necessary providers, managed care intermediaries that
extract rent, provider stigma that suppresses participation, chronic disease
management that is nominally covered and practically inaccessible, and an
administrative apparatus so fragmented that patients navigate multiple bureaucracies
to receive care that should be simple.

This framework fixes those failures by changing the delivery mechanism rather than
the underlying commitment. Medicaid's affordability guarantee becomes a continuous
income gradient applied automatically through the healthcare rail. Clinical need
activates targeted enhancements at the market-layer boundary. Chronic illness triggers
a persistent recalibration of routine care costs that makes ongoing disease management
genuinely affordable. Medicare's entitlement guarantee becomes an automatic
attestation verified at settlement through the same rail every patient uses.
Providers cannot see program status. Patients do not navigate separate systems.
The arithmetic is done automatically.

Medicaid becomes a rule in the rail, not a maze around the patient. Medicare remains
Medicare — the guarantee is preserved, the backend gets simpler. The statutory
commitments survive. The bureaucratic maze does not.

Different programs. Common plumbing. That is what public coverage modernization means.
