---
id: sec-administration-heta-steady-state
title: Severe Event Coverage Administration — HETA Steady-State Operating Model
sidebar_label: SEC Administration
sidebar_position: 4
slug: /healthcare/care-delivery/sec-administration
domain: Healthcare
subdomain: Execution_and_Transition
policy_type: Operational Framework
status: Draft
version: 0.1
author: Futures Project
last_updated: 2026-04-10
dependencies:
  - insurance-architecture-sec
  - healthcare-execution-authority
  - heta-revised-charter
  - healthcare-infrastructure-layer
  - ssi-self-sovereign-identity-framework
  - upi-privacy-preserving-payment-rail
  - irs-modernization-automated-income-attestation
  - department-of-data-and-accountability
  - healthcare-state-pilot-framework
  - cost-performance-backstop
related_initiatives:
  - care-delivery-market-design
  - emergency-trauma-services
  - recoupment-bound-pricing
  - pbm-pharmacy-reform
  - gradient-modernized-welfare
tags:
  - healthcare
  - sec
  - heta
  - insurance
  - payment-routing
  - fraud-detection
  - risk-pool
  - steady-state
---

# Severe Event Coverage Administration — HETA Steady-State Operating Model

## What This Is

This document defines the operational mechanics of Severe Event Coverage (SEC) administration and establishes the Healthcare Execution and Transition Authority (HETA) as the executing institution.

It should be read alongside the HETA Revised Charter, which defines HETA's transition-phase structure, deployment model, enforcement firewall, and congressional oversight architecture. Those elements are not repeated here. This document describes what HETA becomes once the transition is complete — its standing, long-term operational form.

As the healthcare market matures and the transition functions defined in the HETA charter wind down, two functions persist as HETA's steady-state mandate: SEC administration and healthcare market enforcement. The Provider Transition Corps sunsets per the charter's phase-gated provisions. The Integrated Transition Teams disband as pilot districts stabilize. What remains is a leaner, standing institution operating the SEC rail, maintaining the actuarial reference class, enforcing market boundaries, and managing the payment routing infrastructure that the reformed system depends on.

The relationships between HETA and DoDA, PCA, SSI, UPI, the state pilot framework, and the cost performance backstop are fully defined in the transition architecture and carry forward unchanged into steady state. This document adds only what is specific to SEC operational mechanics.

---

## Core Principle

SEC administration is infrastructure operation, not insurance adjudication.

The SEC rail does not decide whether care was appropriate. It does not manage utilization. It does not negotiate prices. It validates that submitted costs meet the standardized schema, routes payment to the correct payer, detects anomalies against the regional reference database, and settles through UPI.

Clinical decisions remain with providers and patients. Price discipline comes from transparency and competition, enforced by market structure. HETA's SEC function ensures the plumbing works correctly and that the data flowing through it is honest.

---

## What SEC Covers — Operational Definition

Severe Event Coverage activates on defined clinical events. For operational purposes, activation is triggered by:

- Emergency and trauma admissions as designated under the utility regulation framework
- Major surgical procedures delivered through the bundled episode pricing system
- Serious illness episodes meeting defined inpatient or complex care thresholds
- High-cost episodes exceeding the statutory clinical threshold established in the insurance architecture

Coverage applies at the episode level and includes all services within the defined episode boundary — facility fees, professional services, anesthesia, standard post-operative care, and defined complication windows. Services outside the episode boundary are market-layer care and are not SEC-covered.

HETA maintains the episode boundary definitions and updates them on a defined cadence through a transparent, versioned process. Episode boundary changes are published in advance, subject to public comment, and logged in the ULRR.

---

## Provider Cost Submission and Validation

### The Standardized Cost Schema

Every provider participating in the SEC-regulated market submits costs through a standardized schema on a defined reporting cadence. The schema captures:

- Labor costs by category
- Facility and capital costs with depreciation methodology
- Device, drug, and supply acquisition costs at invoice price
- Overhead allocation methodology and basis
- Readiness and standby costs for emergency-designated facilities

Submissions are machine-readable, version-controlled, and submitted through the SEC rail using UPI-integrated reporting APIs. The format is standardized across all provider types and sizes. Large health systems connect directly through published APIs. Smaller providers access the schema through pre-built integrations in major practice management platforms, which are required to support the standardized format.

### The Perjury Attestation Mechanism

Cost submissions are signed with the provider's SSI credential and carry a legal attestation that the submitted figures accurately reflect actual costs. This is not a checkbox — it is a legally binding declaration that creates criminal exposure for material misrepresentation.

The attestation serves two functions simultaneously. First, it establishes the minimum defensible floor: a provider attesting to their costs cannot then bill below those costs without raising questions, and cannot credibly claim their rates are cost-justified if their submissions show otherwise. Second, it creates a self-reinforcing honesty incentive — inflating submitted costs to justify high billing rates is self-incriminating when those costs are compared against regional peers.

Providers are informed of the attestation obligation and its legal implications at onboarding. HETA maintains clear guidance on what constitutes material misrepresentation versus legitimate cost accounting variation.

### DoDA's Role in Cost Validation

HETA operates the cost submission infrastructure and maintains the regional price comparison database. DoDA certifies the methodology — the cost accounting standards, the comparability framework, the statistical models used for anomaly detection — but does not operate the database itself. This separation preserves DoDA's role as an independent measurement institution rather than an operational one.

DoDA publishes the certified methodology, audits HETA's adherence to it on a defined schedule, and publishes the audit findings. If HETA's operational practices diverge from certified methodology, DoDA flags it publicly and Congress receives notification through the annual cost performance backstop reporting cycle.

---

## Payment Routing — How the Rail Works

When a provider submits a bill through the SEC rail, the routing logic runs automatically and is invisible to the provider. The provider sees: bill submitted, validation result, payment received. They do not see where the bill was routed, what mix of payers contributed, or how much of the payment came from SEC government coverage versus private insurance.

This provider-side blindness is a deliberate design feature. Providers cannot adjust their pricing based on the payer mix because they cannot see the payer mix. Price discovery operates against the regional market, not against known subsidy levels.

### The Routing Logic

**Step 1 — Validation.** The submitted bill is checked against the standardized schema for completeness and format compliance. Missing required fields or format errors trigger an immediate return with specific error codes. Valid submissions proceed to routing.

**Step 2 — Episode classification.** The bill is classified against the episode boundary definitions maintained by HETA. Services within a defined SEC episode proceed to coverage routing. Services outside episode boundaries are flagged as market-layer care and routed to direct-pay or supplemental insurance settlement.

**Step 3 — SSI credential check.** The SEC rail queries the patient's SSI wallet for two credentials: insurance status attestation and income bracket attestation. The wallet returns cryptographic proofs — binary confirmations of credential validity — without transmitting the underlying credential data. The rail learns whether the patient has active private insurance coverage for this episode type. It does not learn the specific insurer, the plan details, or the patient's exact income.

**Step 4 — Routing decision.**

- Patient has active private insurance covering this episode type: bill routes to the insurer at regulated rate bands. The insurer receives the bill through standardized APIs and settles through UPI. The patient's out-of-pocket, if any, is calculated against the regulated rate band and collected through UPI at point of settlement.

- Patient has no private insurance: bill routes to SEC government coverage. Payment is calculated based on the regulated rate band for the episode type and settled through UPI. The cost flows into the SEC risk pool and is recovered through the income-based withholding and reconciliation system described in the IRS modernization framework.

- Patient has partial coverage (supplemental insurance above SEC floor): SEC covers the baseline episode cost at regulated rates; supplemental coverage settles the difference through its own rail; the patient's residual out-of-pocket is calculated and collected through UPI.

**Step 5 — Settlement.** Payment flows through UPI to the provider's registered account. Settlement is final at the point of transfer. No post-hoc balance billing, no retroactive fee adjustments, no surprise charges. The provider's UPI transaction record shows payment received with a standardized reference code but no payer identity.

### Patient-Side Transparency

While the provider sees only that payment was made, the patient sees everything relevant to their situation. Their SSI wallet app shows:

- The episode that was covered
- The regulated rate band that applied
- Whether the cost flowed through their private insurance, SEC government coverage, or a combination
- Their out-of-pocket responsibility, if any, calculated against the rate band
- The settlement confirmation

Before receiving care, the app shows the patient cost estimates based on their current insurance status and income bracket attestations — giving them visibility into what they would pay in each scenario before they walk in the door. This pre-care transparency is the patient-facing equivalent of the provider-side price posting requirement.

---

## Fraud Detection and Anomaly Response

### The Regional Price Comparison Database

HETA maintains a continuously updated regional price comparison database built from all cost submissions and billing events flowing through the SEC rail. For each service category, the database maintains the regional distribution — median, standard deviation, percentile bands — updated on a rolling basis as new submissions arrive.

This database is the operational heart of the fraud detection system. It makes visible, in near-real-time, what every provider in a region is charging for every covered service category, compared against every other provider including the regional surgery centers that serve as the competitive reference point.

The database is also the mechanism by which the system structurally calls bullshit. A provider billing two standard deviations above the regional median for an anesthesiology episode is not automatically a fraudster — there may be legitimate reasons for cost variation. But they are automatically flagged for review, and they must be able to explain the variation against their own cost attestation.

### Anomaly Detection and Response

The fraud detection model runs against every submitted bill in near-real-time. Anomalies are classified by type and severity:

**Pricing anomalies:** Bill exceeds regional median by more than a defined threshold for a given service category. Response: automatic flag, provider receives a query requesting cost justification against their submitted cost attestation. This is not punitive — it is a request for explanation. Providers who can justify the variation through legitimate cost differences clear the flag. Providers who cannot are escalated to the Market and Utility Enforcement function.

**Pattern anomalies:** Provider billing patterns diverge from regional norms in ways that suggest upcoding, unbundling, or episode boundary gaming. Response: escalation to audit queue. Pattern anomalies require more analysis than point-in-time pricing anomalies and are handled by HETA's enforcement function rather than the automated system.

**Schema anomalies:** Submitted bills contain internal inconsistencies — line items that don't sum correctly, episode classifications that don't match the services listed, cost attestations that contradict billing amounts. Response: immediate return for correction. Schema anomalies are treated as administrative errors unless the pattern suggests intentional manipulation.

**Identity anomalies:** SSI credential queries return unexpected results — credentials that have been revoked, credentials presented for patient identities that don't match the episode context, or credential sequences that suggest impersonation. Response: immediate hold on payment routing, escalation to identity integrity review. These are the most serious anomalies and are handled under the enforcement firewall with full audit trail.

All anomaly events are logged in the tamper-evident ledger maintained under the government outflow integrity framework. DoDA receives aggregate anomaly statistics — frequency, type, resolution rates — without individual case data. Individual case data remains within HETA's enforcement function under the privacy protections established in the HETA charter.

### The Phone Call

For pricing anomalies that exceed defined thresholds, the automated system triggers a provider outreach event — what is colloquially the phone call. This is a structured inquiry, not an accusation. The provider receives a notification through their SEC rail account that a submitted bill has been flagged for pricing review, with the specific service category and the regional comparison data that triggered the flag. They are asked to provide cost justification referencing their submitted cost attestation.

The inquiry is handled by HETA's Provider Transition Corps during the transition phase and by a standing provider relations function in steady state. It is explicitly not handled by the Market and Utility Enforcement function — the enforcement firewall established in the HETA charter applies here. The inquiry is a compliance support interaction, not an enforcement action, unless the provider's response reveals intentional misrepresentation.

Most pricing anomaly inquiries resolve at this stage. Providers either explain legitimate cost variation or correct billing errors. The system is designed to be diagnostic before it is punitive.

---

## Risk Pool Architecture

### Capitalization During Transition

During the pilot phase and early rollout, the SEC risk pool is federally backstopped. The federal government provides the capital reserve necessary to ensure payment continuity while the pool builds scale and actuarial stability. This backstop is explicit, bounded, and governed — it is not an open-ended guarantee but a defined capital facility with statutory limits, as established in the state pilot framework.

As pilot states enter the system and the enrolled population grows, the risk pool builds toward actuarial self-sufficiency. The federal backstop declines proportionally as the pool's own reserves reach defined adequacy thresholds. The transition from backstop-dependent to self-sufficient is governed by the same performance-gated expansion logic established in the HETA charter — defined metrics, independent certification by DoDA, transparent public reporting.

### Cross-State Pooling

SEC risk is pooled nationally, not state-by-state. This is the critical structural decision that makes SEC actuarially tractable. State-bounded pools produce adverse selection, instability, and the same fragmentation problems that plague current insurance markets.

As states enter the system through the opt-in pilot framework, their enrolled populations are immediately included in the national pool. Insurers participating in SEC cannot maintain state-bounded books of business for SEC coverage — they participate in the national pool or they do not participate. This rule is enforced by HETA and is a condition of SEC market participation.

### The Actuarial Reference Class

Because SEC enrollment is universal and coverage is standardized, the risk pool produces the cleanest available dataset on severe-event incidence in the United States. HETA maintains this dataset as the actuarial reference class — the baseline against which all insurance products operating above the SEC floor are evaluated.

The reference class includes:
- Severe-event incidence rates by type, region, age band, and demographic category
- Episode-level cost distributions by service category and geography
- Geographic and demographic adjustment factors for premium calculation
- Trend and variance data over time as the dataset matures

This data is published in aggregate, de-identified form through DoDA dashboards. It is the public good that the universal SEC pool produces — a national ground truth for healthcare cost that has never existed before because no previous system had universal enrollment with standardized coverage.

Private insurers use this reference class to price their products above the SEC floor. HETA uses it to evaluate whether those products are adding value or merely adding cost. The four-test framework established in the insurance architecture doc — risk transfer, value-add, actuarial honesty, complexity — is applied against this reference class.

---

## HETA as Steady-State Institution

### What Winds Down

The Provider Transition Corps sunsets as markets stabilize, per the phase-gated provisions in the HETA charter. Regional transition offices close on the published schedule as their districts complete the transition and provider onboarding is complete. The Integrated Transition Teams disband as the federal-state co-deployment model is no longer needed for transition management. Market Transition Waiver authority expires unless affirmatively reauthorized.

### What Persists

Two functions persist as HETA's standing mandate:

**SEC Administration.** The SEC rail, the cost submission and validation infrastructure, the payment routing system, the fraud detection model, the regional price comparison database, the risk pool management function, and the actuarial reference class maintenance. This is the operational core of the reformed healthcare system and it requires a permanent institution to run it.

**Healthcare Market Enforcement.** Price transparency enforcement, market boundary rules (insurance excluded from primary care and urgent care), anti-gaming audits, emergency utility rate discipline, and the insurance product classification system. Markets do not self-enforce. HETA's standing enforcement function is what keeps the market structure honest after the transition is complete.

### The Lean Steady-State Form

In steady state, HETA is substantially smaller than it is during the transition. It does not need a Provider Transition Corps. It does not need regional offices in every pilot district. It does not need the full federal-state co-deployment infrastructure.

What it needs is a standing SEC rail operations function, a standing fraud detection and anomaly response function, a standing market enforcement function, and a standing actuarial and data function that maintains the reference class and interfaces with DoDA. These are bounded, well-defined operational mandates that can be staffed and resourced appropriately for a standing institution rather than a transition deployment.

The Execution Corps framework's scope immutability and renewal-by-default prohibition apply. HETA in steady state cannot expand its mandate without explicit congressional reauthorization. Its standing functions are reviewed on a defined statutory cadence. If the healthcare market reaches a state of genuine stability where enforcement and SEC administration require less institutional capacity, HETA scales down accordingly.

This is what HETA was always designed to become: not a permanent bureaucracy, but a permanent infrastructure operator — running the rails the reformed system depends on, enforcing the market rules that keep it honest, and scaling its own footprint to match what the system actually needs.

---

## PBM Transition Pathway

The PBM reform framework defines the end state — pharmacies as distribution infrastructure, full formulary transparency, recoupment-bound pricing ceilings, prohibited rebate practices. HETA manages the transition from the current contractual landscape to that end state.

### Transition Mechanics

Existing PBM contracts with payers, manufacturers, and pharmacies are subject to a mandatory disclosure requirement from the date of HETA's establishment. All contracts must be filed with HETA within a defined window. HETA publishes aggregate statistics on contract structures without revealing proprietary terms — the public sees the landscape of practices, not individual agreements.

New contracts entered after HETA's establishment must comply with the end-state rules immediately. Legacy contracts are grandfathered for a defined transition period — long enough to prevent disruption, short enough to create genuine urgency for reform. The transition period is published in advance and cannot be extended without congressional authorization.

During the transition period, HETA enforces:
- Mandatory rebate pass-through — retained rebates must be disclosed and passed through to the system or patient
- Spread pricing prohibition — effective from HETA establishment with no grandfathering
- Formulary transparency — full public disclosure of covered drugs, tier placement criteria, and price concessions on a defined schedule

Practices that are prohibited from day one cannot be grandfathered. Practices that require structural market change — moving to standardized service fees, unwinding complex rebate arrangements — are subject to the transition period with published milestones.

### Integration with SEC Rail

As the SEC rail reaches operational maturity, drug distribution through the pharmacy and PBM layer is integrated into the SEC payment infrastructure. Pharmacies connect through standardized APIs. Drug costs flow through the SEC rail with the same transparency and routing logic as other covered services. Recoupment tracking for branded drugs is maintained in the HETA database and updated as sales data flows through the rail.

This integration is phased — it cannot happen until the SEC rail itself is operational and stable. The PBM transition timeline is therefore downstream of the SEC operational timeline, with full integration as a late-phase milestone rather than a day-one requirement.

---

## Guardrails

1. **Provider blindness is structurally enforced.** Payment routing is invisible to providers by design, not by policy. The rail architecture does not produce a data field that providers could read even if they wanted to. This is not a rule that can be gamed — it is an architectural property.

2. **Patient transparency is structurally enforced.** The patient-facing app reads from the SSI wallet and the SEC reference database. It cannot show information that isn't there and it cannot hide information that is. Transparency is a property of the architecture, not a compliance obligation.

3. **Fraud detection is diagnostic before punitive.** The automated system flags anomalies and triggers inquiries. It does not trigger enforcement actions. Enforcement requires human review under the firewall provisions of the HETA charter. The system is designed to catch errors and legitimate variation before it catches fraud — most anomalies resolve without enforcement.

4. **The risk pool cannot be state-bounded.** This rule has no exceptions during the SEC operational period. State-bounded pools would recreate the fragmentation the system is designed to eliminate. HETA has no authority to grant exceptions and Congress cannot authorize them without amending the SEC statute.

5. **HETA cannot expand its mandate in steady state.** Scope immutability from the Execution Corps framework applies. New functions require explicit congressional authorization. HETA in steady state is an infrastructure operator, not a policy originator.

---

## Known Gaps — Pending Development

**Long-term care integration.** SEC as defined covers acute and severe events. Long-term care — nursing facilities, home health, extended disability support — is not addressed in the current SEC framework and represents a significant fiscal and humanitarian gap. This requires a dedicated doc and likely a separate program design.

**Mental health episode boundaries.** Mental health and substance use disorder treatment creates difficult episode boundary definition questions — what constitutes a severe event, what belongs in the market layer, and how episodic and ongoing treatment interact with the SEC coverage model. The dental, vision, and mental health integration doc addresses some of this but the SEC operational interface needs more specificity.

**Rural and frontier access.** The regulated rate bands and regional price comparison database assume sufficient market density to produce meaningful comparisons. In rural and frontier areas with very few providers, the reference database may not be robust enough to support anomaly detection or meaningful competition. HETA needs specific protocols for low-density markets that preserve access without creating regulatory arbitrage opportunities.

**International coverage.** SEC coverage for American citizens receiving emergency care abroad is not addressed. This is a smaller-scale problem than the domestic architecture but affects a meaningful population and needs defined rules.
