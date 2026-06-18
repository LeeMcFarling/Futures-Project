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

## What This Is

This document defines the operational mechanics of Severe Event Coverage
administration and establishes HETA as the executing institution in its steady-state
form.

Read this alongside the HETA Revised Charter, which defines HETA's transition-phase
structure, deployment model, enforcement firewall, and congressional oversight
architecture. Those elements are not repeated here. This document describes what
HETA becomes once the transition is complete — its standing, long-term operational
form.

As the healthcare market matures and the transition functions defined in the HETA
charter wind down, two functions persist as HETA's steady-state mandate: SEC
administration and healthcare market enforcement. The Provider Transition Corps
sunsets per the charter's phase-gated provisions. The Integrated Transition Teams
disband as pilot districts stabilize. What remains is a leaner, standing institution
operating the SEC rail, maintaining the actuarial reference class, enforcing market
boundaries, and managing the payment routing infrastructure the reformed system
depends on.

The relationships between HETA and DoDA, PCA, SSI, UPI, the state pilot framework,
and the cost performance backstop carry forward unchanged into steady state from the
transition architecture. This document adds only what is specific to SEC operational
mechanics.

---

## Core Principle

SEC administration is infrastructure operation, not insurance adjudication.

The SEC rail does not decide whether care was appropriate. It does not manage
utilization. It does not negotiate prices. It validates that submitted costs meet the
standardized schema, routes payment to the correct payer, detects anomalies against
the regional reference database, and settles through UPI. Clinical decisions remain
with providers and patients. Price discipline comes from transparency and competition,
enforced by market structure. HETA's SEC function ensures the plumbing works
correctly and that the data flowing through it is honest.

---

## What SEC Covers — Operational Definition

Severe Event Coverage activates on defined clinical events. For operational purposes,
activation is triggered by emergency and trauma admissions covered under the SEC
utility framework, major surgical procedures delivered through the bundled episode
pricing system, serious illness episodes meeting defined inpatient or complex care
thresholds, and high-cost episodes exceeding the statutory clinical threshold
established in the insurance architecture.

Coverage applies at the episode level and includes all services within the defined
episode boundary — facility fees, professional services, anesthesia, standard
post-operative care, and defined complication windows. Services outside the episode
boundary are market-layer care and are not SEC-covered.

HETA maintains the episode boundary definitions and updates them on a defined cadence
through a transparent, versioned process. Episode boundary changes are published in
advance, subject to public comment, and logged in the immutable government ledger.

---

## Provider Cost Submission and Validation

Every provider participating in the SEC-regulated market submits costs through a
standardized schema on a defined reporting cadence. The schema captures labor costs
by category, facility and capital costs with depreciation methodology, device, drug,
and supply acquisition costs at invoice price, overhead allocation methodology and
basis, and readiness and standby costs for emergency-designated facilities.
Submissions are machine-readable, version-controlled, and submitted through the SEC
rail using UPI-integrated reporting APIs. The format is standardized across all
provider types and sizes. Large health systems connect directly through published
APIs. Smaller providers access the schema through pre-built integrations in major
practice management platforms, which are required to support the standardized format.

Cost submissions are signed with the provider's SSI credential and carry a legal
attestation that the submitted figures accurately reflect actual costs. This is not a
checkbox — it is a legally binding declaration that creates criminal exposure for
material misrepresentation. The attestation serves two functions simultaneously.
First, it establishes the minimum defensible floor: a provider attesting to their
costs cannot then bill below those costs without raising questions, and cannot
credibly claim their rates are cost-justified if their submissions show otherwise.
Second, it creates a self-reinforcing honesty incentive — inflating submitted costs
to justify high billing rates is self-incriminating when those costs are compared
against regional peers. Providers are informed of the attestation obligation and its
legal implications at onboarding. HETA maintains clear guidance on what constitutes
material misrepresentation versus legitimate cost accounting variation.

HETA operates the cost submission infrastructure and maintains the regional price
comparison database. DoDA certifies the methodology — the cost accounting standards,
the comparability framework, the statistical models used for anomaly detection — but
does not operate the database itself. This separation preserves DoDA's role as an
independent measurement institution rather than an operational one. DoDA publishes
the certified methodology, audits HETA's adherence to it on a defined schedule, and
publishes the audit findings. If HETA's operational practices diverge from certified
methodology, DoDA flags it publicly and Congress receives notification through the
annual cost performance backstop reporting cycle.

---

## Payment Routing — How the Rail Works

When a provider submits a bill through the SEC rail, the routing logic runs
automatically and is invisible to the provider. The provider sees: bill submitted,
validation result, payment received. They do not see where the bill was routed, what
mix of payers contributed, or how much of the payment came from SEC government
coverage versus private insurance. This provider-side blindness is a deliberate
design feature. Providers cannot adjust their pricing based on the payer mix because
they cannot see the payer mix. Price discovery operates against the regional market,
not against known subsidy levels.

The routing logic runs in five steps. First, the submitted bill is checked against
the standardized schema for completeness and format compliance — missing required
fields or format errors trigger an immediate return with specific error codes, and
valid submissions proceed. Second, the bill is classified against the episode boundary
definitions maintained by HETA — services within a defined SEC episode proceed to
coverage routing, while services outside episode boundaries are flagged as
market-layer care and routed to direct-pay or supplemental insurance settlement.
Third, the SEC rail queries the patient's SSI wallet for insurance status attestation
and income bracket attestation — the wallet returns cryptographic proofs confirming
credential validity without transmitting underlying credential data, so the rail
learns whether the patient has active private insurance for this episode type without
learning the specific insurer, plan details, or exact income.

Fourth, the routing decision is made. If the patient has active private insurance
covering this episode type, the bill routes to the insurer at regulated rate bands —
the insurer receives the bill through standardized APIs, settles through UPI, and the
patient's out-of-pocket if any is calculated against the regulated rate band and
collected through UPI at settlement. If the patient has no private insurance, the
bill routes to SEC government coverage — payment is calculated based on the regulated
rate band and settled through UPI, with the cost flowing into the SEC risk pool and
recovered through the income-based withholding and reconciliation system. If the
patient has partial coverage through supplemental insurance above the SEC floor, SEC
covers the baseline episode cost at regulated rates, supplemental coverage settles
the difference through its own rail, and the patient's residual out-of-pocket is
calculated and collected through UPI.

Fifth, payment flows through UPI to the provider's registered account. Settlement is
final at the point of transfer. No post-hoc balance billing, no retroactive fee
adjustments, no surprise charges. The provider's UPI transaction record shows payment
received with a standardized reference code but no payer identity.

While the provider sees only that payment was made, the patient sees everything
relevant to their situation. Their SSI wallet app shows the episode that was covered,
the regulated rate band that applied, whether the cost flowed through private
insurance or SEC government coverage or a combination, their out-of-pocket
responsibility if any, and the settlement confirmation. Before receiving care, the
app shows the patient cost estimates based on their current insurance status and
income bracket attestations — giving them visibility into what they would pay before
they walk in the door. This pre-care transparency is the patient-facing equivalent of
the provider-side price posting requirement.

---

## Fraud Detection and Anomaly Response

HETA maintains a continuously updated regional price comparison database built from
all cost submissions and billing events flowing through the SEC rail. For each service
category, the database maintains the regional distribution — median, standard
deviation, percentile bands — updated on a rolling basis as new submissions arrive.
This database is the operational heart of anomaly detection and first-line integrity screening. It makes
visible, in near-real-time, what every provider in a region is charging for every
covered service category, compared against every other provider including the regional
surgery centers that serve as the competitive reference point. It is also the
mechanism by which the system structurally detects when someone is charging far above
what their peers charge and their own costs justify.

The fraud detection model runs against every submitted bill in near-real-time.
Anomalies are classified by type and severity. Pricing anomalies occur when a bill
exceeds the regional median by more than a defined threshold for a given service
category — the response is an automatic flag and a query to the provider requesting
cost justification against their submitted cost attestation, which is a request for
explanation rather than a punitive action. Providers who can justify the variation
through legitimate cost differences clear the flag; providers who cannot are escalated
to the Market and Utility Enforcement function.

Pattern anomalies occur when provider billing patterns diverge from regional norms in
ways that suggest upcoding, unbundling, or episode boundary gaming — these require
more analysis than point-in-time pricing anomalies and are handled by HETA's
enforcement function rather than the automated system. Schema anomalies occur when
submitted bills contain internal inconsistencies — line items that don't sum
correctly, episode classifications that don't match the services listed, or cost
attestations that contradict billing amounts — and are treated as administrative
errors unless the pattern suggests intentional manipulation. Identity anomalies are
the most serious: when SSI credential queries return revoked credentials, credentials
presented for patient identities that don't match the episode context, or credential
sequences that suggest impersonation, payment routing is immediately held and
escalated to identity integrity review under the enforcement firewall.

All anomaly events are logged in the tamper-evident immutable ledger. DoDA receives
aggregate anomaly statistics — frequency, type, resolution rates — without individual
case data. Individual case data remains within HETA's enforcement function under the
privacy protections established in the HETA charter.

For pricing anomalies that exceed defined thresholds, the automated system triggers
a structured provider inquiry — what is colloquially the phone call. The provider
receives a notification through their SEC rail account that a submitted bill has been
flagged for pricing review, with the specific service category and the regional
comparison data that triggered the flag. They are asked to provide cost justification
referencing their submitted cost attestation. The inquiry is handled by a standing
provider relations function in steady state and is explicitly not handled by the
Market and Utility Enforcement function — the enforcement firewall established in the
HETA charter applies here. The inquiry is a compliance support interaction, not an
enforcement action, unless the provider's response reveals intentional
misrepresentation. Most pricing anomaly inquiries resolve at this stage. The system
is designed to be diagnostic before it is punitive.

HETA's role in fraud detection is first-line anomaly detection and payment integrity.
HETA is not the long-horizon investigative body. Where anomaly patterns suggest
systemic fraud — coordinated billing across providers, attestation abuse, identity
compromise, provider-network collusion, or cross-domain subsidy capture — HETA
packages the evidence and refers it to the Public Integrity Office. The Public
Integrity Office conducts adversarial investigation. HETA controls the payment gate.

---

## Payment Integrity Holds and Systemic Fraud Referral

HETA has authority to stop, hold, or return payments where the SEC rail detects a
defined payment-integrity failure.

Payment-integrity failures include revoked or invalid SSI credentials, invalid
provider credentials, schema failure, duplicate billing, facially inconsistent episode
classification, billing outside the authorized episode boundary, prohibited
balance-billing attempts, or other transaction-level defects defined by HETA rule and
DoDA-certified methodology.

A payment hold is not a fraud finding. It is a temporary integrity action to prevent
public, pooled, or insured funds from leaving the rail when the transaction fails
validation.

Where HETA detects repeated anomalies, coordinated billing patterns, attestation
abuse, identity compromise, provider-network collusion, subsidy capture, or other
indicators of systemic fraud, HETA shall package the anomaly record and refer the
matter to the Public Integrity Office.

The Public Integrity Office conducts adversarial investigation and coordinates with
DOJ, inspectors general, state attorneys general, licensing boards, and other
competent enforcement bodies. HETA does not prosecute and does not conduct systemic
fraud investigations outside its rail-integrity mandate.

Upon confirmed findings or emergency integrity certification from the Public Integrity
Office, HETA may suspend rail participation, revoke SEC settlement eligibility, impose
enhanced audit status, restrict access to PCA instruments, recover improper payments
where authorized, and notify affected patients or payers as required by law.

HETA controls payment integrity. The Public Integrity Office investigates systemic
abuse. DOJ and competent enforcement bodies pursue civil or criminal remedies.

---

## Risk Pool Architecture

During the pilot phase and early rollout, the SEC risk pool is federally backstopped.
The federal government provides the capital reserve necessary to ensure payment
continuity while the pool builds scale and actuarial stability. This backstop is
explicit, bounded, and governed — a defined capital facility with statutory limits,
not an open-ended guarantee. As pilot states enter the system and the enrolled
population grows, the risk pool builds toward actuarial self-sufficiency. The federal
backstop declines proportionally as the pool's own reserves reach defined adequacy
thresholds. The transition from backstop-dependent to self-sufficient is governed by
the same performance-gated expansion logic established in the HETA charter — defined
metrics, independent certification by DoDA, transparent public reporting.

SEC risk is pooled nationally, not state-by-state. This is the critical structural
decision that makes SEC actuarially tractable. State-bounded pools produce adverse
selection, instability, and the same fragmentation problems that plague current
insurance markets. As states enter the system through the opt-in pilot framework,
their enrolled populations are immediately included in the national pool. Insurers
participating in SEC cannot maintain state-bounded books of business for SEC coverage
— they participate in the national pool or they do not participate. This rule is
enforced by HETA and is a condition of SEC market participation.

Because SEC enrollment is universal and coverage is standardized, the risk pool
produces the cleanest available dataset on severe-event incidence in the United
States. HETA maintains this dataset as the actuarial reference class — the baseline
against which all insurance products operating above the SEC floor are evaluated. The
reference class includes severe-event incidence rates by type, region, age band, and
demographic category; episode-level cost distributions by service category and
geography; geographic and demographic adjustment factors for premium calculation; and
trend and variance data over time as the dataset matures. This data is published in
aggregate, de-identified form through DoDA dashboards. It is the public good that the
universal SEC pool produces — a national ground truth for healthcare cost that has
never existed before because no previous system had universal enrollment with
standardized coverage. Private insurers use this reference class to price their
products above the SEC floor. HETA uses it to evaluate whether those products are
adding value or merely adding cost.

---

## HETA as Steady-State Institution

The Provider Transition Corps sunsets as markets stabilize. Regional transition
offices close on the published schedule as their districts complete the transition.
The Integrated Transition Teams disband as the federal-state co-deployment model is
no longer needed. Market Transition Waiver authority expires unless affirmatively
reauthorized. These are the transition functions that wind down.

Two functions persist as HETA's standing mandate. The first is SEC administration —
the SEC rail, the cost submission and validation infrastructure, the payment routing
system, the fraud detection model, the regional price comparison database, the risk
pool management function, and the actuarial reference class maintenance. This is the
operational core of the reformed healthcare system and it requires a permanent
institution to run it. The second is healthcare market enforcement — price
transparency enforcement, market boundary rules that keep insurance excluded from
primary care and urgent care, anti-gaming audits, SEC utility-rate discipline across
all non-shoppable care, and the insurance product classification system. Markets do not self-enforce. HETA's
standing enforcement function is what keeps the market structure honest after the
transition is complete.

In steady state, HETA is substantially smaller than during the transition. It needs
a standing SEC rail operations function, a standing fraud detection and anomaly
response function, a standing market enforcement function, and a standing actuarial
and data function that maintains the reference class and interfaces with DoDA. These
are bounded, well-defined operational mandates that can be staffed and resourced
appropriately for a standing institution rather than a transition deployment.

The Execution Corps framework's scope immutability and renewal-by-default prohibition
apply. HETA in steady state cannot expand its mandate without explicit congressional
reauthorization. Its standing functions are reviewed on a defined statutory cadence.
If the healthcare market reaches a state of genuine stability where enforcement and
SEC administration require less institutional capacity, HETA scales down accordingly.
This is what HETA was always designed to become — not a permanent bureaucracy, but a
permanent infrastructure operator. Running the rails the reformed system depends on,
enforcing the market rules that keep it honest, and scaling its own footprint to
match what the system actually needs.

---

## PBM Interface

Drug distribution through the pharmacy and PBM layer is a downstream integration
target for the SEC rail. As the rail reaches operational maturity, pharmacies connect
through standardized APIs and drug costs flow through the SEC payment infrastructure
with the same transparency and routing logic as other covered services. Recoupment
tracking for branded drugs is maintained in the HETA database and updated as sales
data flows through the rail.

This integration is phased — it cannot happen until the SEC rail itself is
operational and stable. The PBM transition timeline is downstream of the SEC
operational timeline, with full integration as a late-phase milestone rather than a
day-one requirement.

The detailed mechanics of PBM contract disclosure, legacy contract grandfathering,
rebate pass-through requirements, spread pricing prohibition, and formulary
transparency obligations are defined in the PBM Reform Framework. That brief carries
the policy detail. This section defines only the SEC rail interface point.

---

## Guardrails

Provider blindness is structurally enforced. Payment routing is invisible to
providers by design, not by policy. The rail architecture does not produce a data
field that providers could read even if they wanted to. This is not a rule that can
be gamed — it is an architectural property.

Patient transparency is structurally enforced. The patient-facing app reads from the
SSI wallet and the SEC reference database. It cannot show information that isn't
there and it cannot hide information that is. Transparency is a property of the
architecture, not a compliance obligation.

Fraud detection is diagnostic before punitive. The automated system flags anomalies
and triggers inquiries. It does not trigger enforcement actions. Enforcement requires
human review under the firewall provisions of the HETA charter. The system is
designed to catch errors and legitimate variation before it catches fraud — most
anomalies resolve without enforcement.

The risk pool cannot be state-bounded. This rule has no exceptions during the SEC
operational period. State-bounded pools would recreate the fragmentation the system
is designed to eliminate. HETA has no authority to grant exceptions and Congress
cannot authorize them without amending the SEC statute.

HETA cannot expand its mandate in steady state. Scope immutability from the Execution
Corps framework applies. New functions require explicit congressional authorization.
HETA in steady state is an infrastructure operator, not a policy originator.

---

## Known Gaps — Pending Development

Long-term care integration is not addressed in the current SEC framework and
represents a significant fiscal and humanitarian gap. SEC as defined covers acute
and severe events. Long-term care — nursing facilities, home health, extended
disability support — requires a dedicated document and likely a separate program
design.

Mental health episode boundaries need more specificity at the SEC operational
interface. The dental, vision, and mental health integration document addresses some
of this but the SEC operational interface needs clearer rules on what constitutes a
severe event, what belongs in the market layer, and how episodic and ongoing
treatment interact with the SEC coverage model.

Rural and frontier access creates specific challenges for the regional price
comparison database and anomaly detection. In low-density markets with very few
providers, the reference database may not be robust enough to support meaningful
comparisons or anomaly detection. HETA needs specific protocols for low-density
markets that preserve access without creating regulatory arbitrage opportunities.

International coverage for American citizens receiving emergency care abroad is not
addressed. This affects a meaningful population and needs defined rules, but is a
smaller-scale problem than the domestic architecture.

Patient and provider appeals require further development. The SEC rail needs a fast,
bounded dispute process for episode-boundary classification errors, payment-routing
errors, and medically necessary complication-window disputes. The appeal process must
be fast enough to protect patients from financial exposure and providers from
settlement uncertainty without recreating legacy claims adjudication.

---

## Bottom Line

SEC administration is the operational core of the reformed healthcare system. The
rail settles payments, validates costs, routes claims, detects fraud, maintains the
actuarial reference class, and enforces the market boundary that makes everything
else work. HETA runs that rail in steady state — leaner than during the transition,
permanently authorized for its core functions, and explicitly constrained from
expanding beyond them.

The plumbing has to work. That is the job. Everything else the reform promises
depends on it.
