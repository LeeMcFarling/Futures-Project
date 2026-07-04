---
id: preventive-dental-hta-actuarial-integration
title: Preventive Dental, HTA Settlement, and Actuarial Risk Attenuation Framework
sidebar_label: Preventive Dental & HTA
sidebar_position: TBD
slug: /healthcare/care-delivery/preventive-dental-hta-actuarial-integration
domain: Healthcare
subdomain: Care_Delivery_and_Insurance
policy_type: Cross-Domain Integration Framework
status: Draft
phase: 2
version: 0.1
author: Futures Project
last_updated: 2026-04-28
dependencies:
  - dental-vision-mental-health-integration
  - care-delivery-market-design
  - insurance-architecture-sec
  - sec-administration-heta-steady-state
  - healthcare-infrastructure-layer
  - portable-healthcare-contribution-floor
  - benefits-gradient-modernization
  - worker-classification-parity
  - irs-modernization-automated-income-attestation
  - ssi-self-sovereign-identity-framework
  - upi-privacy-preserving-payment-rail
related_initiatives:
  - regional-health-center-network
  - cost-performance-backstop
  - employer-sponsored-coverage-transition
  - real-time-eitc-ctc-delivery
  - labor-stack-enforcement-framework
tags:
  - healthcare
  - dental
  - preventive-care
  - hta
  - sec
  - actuarial-risk
  - labor
  - benefits-gradient
  - payment-rails
  - ssi
  - upi
---

## Purpose and Scope

This brief defines how routine preventive dental care integrates with the Health
Transition Account structure, the Severe Event Coverage architecture, and the
labor-domain employer healthcare contribution floor.

The purpose is to prevent dental care from remaining a carved-out pseudo-insurance
market while preserving the core distinction of the healthcare framework: routine,
predictable, shoppable services operate in the market layer, and severe, acute,
non-elective events are covered through SEC.

Three rules govern the entire framework. First, routine dental care is paid through
the same HTA routine-care account used for other market-layer healthcare services.
Second, severe dental events are covered through SEC when they cross defined clinical
triggers. Third, verified preventive dental utilization may be used as an actuarial
risk attenuation signal, allowing the system to recognize lower expected downstream
risk without converting routine dental care into insurance coverage.

This brief does not create a separate dental insurance program. It does not create a
provider network. It does not make routine dental care part of SEC. It defines how
routine dental care is financed, displayed, settled, and recognized in actuarial
modeling through existing healthcare and labor rails.

---

## Problem Statement

Dental care is structurally misclassified in the current U.S. healthcare system.

Routine dental services are predictable, schedulable, and highly price-comparable.
Cleanings, examinations, X-rays, fluoride treatments, sealants, fillings, crowns,
dentures, root canals, and orthodontic services can almost always be scheduled in
advance and compared across providers. They are poorly suited to traditional insurance
claims processing — and the existing dental insurance market reflects that failure.
Most dental plans function as capped discount products with narrow networks, annual
benefit maximums that have not meaningfully changed since the 1970s, waiting periods,
exclusions, and administrative friction that drives underutilization of preventive
care, delayed treatment, avoidable emergency dental episodes, and higher downstream
health costs.

The current system also embeds a labor-market distortion. Workers with full-time
employer-sponsored coverage may receive some dental support. Part-time, seasonal,
gig, and dependent-contractor workers often receive none. This reproduces the
hour-threshold problem found in employer-sponsored healthcare more broadly — firms
avoid benefit obligations by structuring work below coverage thresholds, and workers
absorb the cost through deferred care or out-of-pocket exposure.

The reformed healthcare and labor stacks create the tools needed to correct this. HTA
accounts provide a portable routine-care financing vehicle. The benefits gradient
provides income-based affordability support without cliffs. The employer healthcare
contribution floor requires firms to contribute to routine-care costs regardless of
full-time status. SSI and UPI provide privacy-preserving eligibility, utilization, and
settlement rails. SEC remains available for acute, severe, high-cost dental events.

The missing piece is an integration rule that connects routine dental care to this
architecture without rebuilding the failed dental insurance model.

---

## Core Design Principle

Routine dental care is market-layer care. Severe dental events are SEC-covered care.
Preventive utilization is an actuarial signal. This distinction governs the entire
framework.

Routine dental care should not be insured through SEC because it is predictable and
shoppable. It should be priced transparently, compared regionally, paid through
portable routine-care accounts, and supported by income-based credits where
appropriate. Severe dental events should be covered by SEC when the clinical situation
becomes acute, systemic, traumatic, surgical, or medically integrated with a covered
episode. Preventive dental utilization should be recognized by the actuarial system
when evidence supports a measurable relationship between routine prevention and lower
downstream risk. The system does not moralize preventive care. It treats verified
prevention as a risk attenuation input.

---

## Domain Placement

Routine dental services that remain in the market layer and are eligible for HTA
settlement include routine examinations, preventive cleanings, dental X-rays within
defined frequency limits, fluoride treatments, sealants, oral cancer screening,
periodontal maintenance where clinically indicated, fillings, crowns, bridges, inlays
and onlays, non-emergency root canals, dentures, scheduled implants, orthodontics, and
cosmetic dental services subject to any statutory limits on subsidized use. These
services are not SEC-covered merely because they are expensive. The governing test is
clinical urgency and non-shoppability, not price alone.

SEC covers dental events when they cross defined clinical triggers, including oral and
maxillofacial surgery arising from trauma, fracture, abscess, pathology, or other
covered medical event; dental care required as part of a covered medical episode such
as pre-surgical extraction before cardiac surgery, organ transplant, chemotherapy, or
other high-risk medical treatment; acute dental infection with systemic involvement
including fever, facial swelling, airway risk, or inpatient management; trauma-related
dental injury including avulsed, fractured, or displaced teeth arising from an
emergency or trauma admission; and dental procedures requiring general anesthesia or
IV sedation where the clinical trigger independently meets SEC criteria. Routine root
canals, crowns, periodontal treatment, implants, and orthodontic services remain
market-layer services unless the clinical context independently triggers SEC.

---

## HTA Eligibility Rule

Routine dental care is eligible for payment through the same HTA account used for
other market-layer care. Eligible account sources may include worker-owned HTA
balances, monthly employer healthcare contribution floor deposits, income-graduated
routine-care subsidies, patient direct contributions, approved supplemental discount
wrap instruments, and public or philanthropic dental-access credits where authorized.

The rail combines these sources at settlement. The provider receives a confirmed
payment and standardized reference code. The provider does not see the patient's
employer contribution balance, income subsidy, public credit, private account mix, or
actuarial classification. The patient sees the full breakdown through the health
wallet or public portal. That asymmetry is structural and enforced — not discretionary.

---

## Employer Contribution Integration

Under the Portable Healthcare Contribution Floor, employers make monthly contributions
into worker-owned healthcare accounts. These contributions apply across full-time,
part-time, seasonal, gig, and dependent-contractor work where the statutory employment
or dependent-work test is satisfied. Routine dental care is an eligible use of those
employer-funded account balances.

The contribution obligation is not dental insurance. It is not employer-sponsored
coverage. It is a portable routine-care contribution that follows the worker,
accumulates across employers where applicable, and may be combined with income-based
public credits. This solves the old hour-threshold distortion. A worker does not lose
routine dental support because they work twenty hours instead of forty. The employer
contribution may be proportional to hours, but the right to receive portable
contributions does not disappear at an arbitrary full-time boundary.

---

## Benefits Gradient Integration

Income-graduated routine-care subsidies may apply to dental services in the market
layer. Subsidies must taper under the Benefits Gradient rules so that additional
earnings do not create a net loss in household resources. Dental affordability support
therefore phases down in coordination with other covered benefits rather than
operating through a separate cliff-based eligibility threshold.

The subsidy is invisible to providers. The patient-facing portal displays the net
price after applicable credits, but the provider receives only the settled amount.
Providers may not price discriminate based on subsidy eligibility, employer
contribution status, or account balance. Dental affordability support is calibrated
by region, household income, household size, and local price distribution. DoDA
monitors whether subsidy increases are being captured by provider price increases in
supply-constrained markets.

---

## Preventive Utilization Attestation

A qualifying preventive dental visit may generate a privacy-preserving preventive
utilization attestation. To satisfy the baseline preventive dental utilization
standard, an individual must complete two qualifying preventive dental visits within
a defined period — typically a calendar year or rolling twelve-month period — subject
to clinical exceptions and access safeguards.

A qualifying visit may include dental examination, preventive cleaning, oral cancer
screening, indicated X-rays within frequency limits, fluoride or sealant treatment
where age- or risk-appropriate, and periodontal maintenance where clinically indicated.

The attestation records only that the utilization standard was satisfied. It does not
expose detailed dental records to employers, insurers, providers, or public benefit
administrators beyond what is required for settlement, audit, and fraud prevention.
The attestation is held through the patient's SSI health wallet and verified through
UPI-compatible settlement logic. The rail confirms status through a binary proof:
preventive dental utilization standard satisfied — yes or no. This attestation may be
renewed annually or on another evidence-based cadence.

---

## Actuarial Risk Attenuation

Verified preventive dental utilization may be used to place an individual into a lower
actuarial reference category where DoDA-certified evidence supports a measurable
reduction in expected downstream risk. Relevant downstream risk categories may include
emergency dental utilization, acute infection risk, high-cost oral surgery episodes,
avoidable restorative escalation, missed work associated with untreated dental disease,
complications in covered medical episodes where oral infection is a known risk factor,
and chronic disease management interactions where evidence supports a
dental-health relationship.

Actuarial recognition may take the form of HTA top-up, preventive utilization credit,
SEC premium offset where applicable, routine-care subsidy enhancement, lower actuarial
reference classification, reduced required reserve level within the HTA account, or
payroll or refundable tax credit where legislatively authorized. The credit is
calibrated to expected savings, not political preference. DoDA certifies the evidence
base and model specification. HETA configures the rail logic. The patient receives the
credit automatically.

---

## Upside-Only Rule

Preventive utilization recognition is upside-only during initial phases. A person who
satisfies the preventive utilization standard may receive a credit, lower
classification, or account benefit. A person who does not satisfy the standard remains
in the ordinary reference category.

Non-utilization may not be used to deny SEC coverage, increase point-of-care charges,
increase employer obligations tied to that specific worker, or impose punitive premiums
during the initial implementation period. This rule is necessary because non-
utilization may reflect access barriers rather than risk preference. Rural provider
shortages, transportation limits, disability, unstable work schedules, lack of
childcare, distrust caused by prior medical mistreatment, language barriers, and local
capacity constraints can all prevent routine dental use. No punitive use of
non-utilization may be authorized unless DoDA certifies regional access adequacy and
Congress affirmatively authorizes a later-stage rule.

---

## Price Transparency and Portal Display

Routine dental services appear in the same public portal used for other market-layer
care. For each covered dental service, the portal displays the provider name and
credential status, posted price, standard service bundle definition, local median
price, local percentile range, SEC or DoDA reference band where applicable, patient
net price after available credits, available appointment windows, provider quality and
safety indicators where validated, whether the provider accepts UPI settlement, and
whether the provider participates in approved discount wrap products.

The portal allows filtering by service type, price, distance, availability, language,
accessibility, sedation capability, pediatric availability, and regional health center
participation. Dental price comparison uses standardized procedure bundles where
possible. HETA defines and versions the service taxonomy to prevent providers from
fragmenting comparable services into non-comparable billing units.

---

## Settlement Flow

The standard routine dental settlement flow is straightforward. The patient selects a
dental service through the portal or receives care from a participating provider. The
provider submits the standardized service code and posted price through the unified
payment rail. The rail checks the patient's available HTA balance, employer
contribution deposits, income-graduated subsidy eligibility, and approved supplemental
instruments, then calculates the patient's net responsibility and displays the
settlement breakdown to the patient. Payment settles to the provider through UPI —
the provider receives the confirmed amount and reference code, but not the payer mix.
If the service qualifies as a preventive utilization event, the rail updates the
patient's attestation. If the patient satisfies the utilization standard, the rail
applies the authorized actuarial risk attenuation credit or classification update.

The entire flow is automated. The patient does not file a claim. The provider does not
submit to an insurer. The arithmetic is done by the rail.

---

## Privacy and Anti-Surveillance Guardrails

This framework must not become a health surveillance or social scoring system.

The preventive utilization attestation may only confirm that the standard was
satisfied. It may not expose diagnosis, procedure detail beyond qualifying category,
employer identity, exact income, subsidy amount, or full dental record. Employers may
not access individual utilization attestations — employers satisfy their obligation by
making monthly HTA contributions through payroll. Providers may not access a patient's
actuarial classification, income subsidy status, employer contribution balance, or
full account history. Insurers and SEC administrators may use aggregate, de-identified,
DoDA-certified utilization data for actuarial modeling, but individual-level
classification changes must be executed through privacy-preserving proofs wherever
technically feasible. Public reporting occurs at aggregate levels sufficient for
accountability without exposing individual behavior.

---

## Fraud, Gaming, and Abuse Controls

The rail detects and deters abuse without creating a high-friction claims process.
Potential abuse patterns include providers submitting preventive visits that did not
occur, upcoding routine services as preventive events, splitting one visit into
multiple qualifying events, excessive frequency of X-rays or adjunctive services,
steering patients into unnecessary add-ons, coordinated price increases following
subsidy activation, and creating low-value preventive appointments solely to trigger
credits.

Controls include standardized qualifying-event definitions, frequency limits, provider
attestation under penalty of law, randomized audit sampling, regional outlier
detection, patient confirmation of completed service, peer comparison of service mix,
automatic flags for anomalous preventive-event volume, and suspension of credit-
trigger eligibility for providers with unresolved fraud flags. The enforcement model
is pattern-based. Patients are not forced into paperwork-heavy reimbursement processes
because of provider-side gaming risk.

---

## Access Safeguards

Preventive utilization credits are not scaled in regions where dental appointment
supply is inadequate. Before full activation, DoDA certifies regional access adequacy
using metrics including dental providers per covered population, appointment
availability within defined time windows, preventive dental utilization by income
quintile, geographic travel time to participating providers, regional health center
dental capacity, mobile clinic availability, pediatric dental access, Medicaid-
transition population access where applicable, and price dispersion and provider
participation rates.

Where access is inadequate, HETA and PCA may prioritize dental capacity expansion
through Regional Health Centers, FQHCs, dental school partnerships, mobile clinics,
hygienist scope expansion where state law permits, and transition support for
independent dental practices connecting to the rail. Credits may still be offered in
inadequate regions if they increase access without creating penalties, but
non-utilization may not be interpreted as an individual risk choice.

---

## Relationship to Regional Health Centers

Regional Health Centers provide baseline dental capacity in underserved regions. At
minimum, covered centers support preventive dental exams, cleanings, basic X-rays,
fillings, periodontal maintenance, pediatric preventive services, oral surgery referral
coordination, and emergency dental stabilization and transfer coordination where
needed. Regional Health Centers do not replace private dental practices. They
establish a floor of access where market capacity is insufficient and provide a
reliable pathway for low-income, rural, and high-barrier populations to satisfy
preventive utilization standards.

---

## Relationship to SEC

This framework preserves SEC actuarial integrity. Routine dental care does not become
an SEC claim. Preventive dental utilization does not require SEC adjudication.
HTA settlement does not alter the SEC trigger boundary. SEC remains responsible for
dental events that become acute, systemic, traumatic, surgical, or medically
integrated with a covered episode. The only connection between preventive dental
utilization and SEC is actuarial — verified prevention may reduce expected future
severe-event risk and may therefore be recognized in risk modeling, credits, or
reserve calibration.

---

## Relationship to Labor Enforcement

Employer HTA contributions must be enforceable through the labor stack. Contribution
failures, underreporting of hours, dependent-contractor evasion, payroll manipulation,
or misclassification designed to avoid healthcare account obligations trigger the
Labor Stack Enforcement Framework. Consequences may include automatic reporting flags,
formula-based civil penalties, PCA access suspension, enhanced enforcement, and
debarment where warranted.

The dental framework depends on this enforcement. If employers can evade monthly HTA
contributions by fragmenting labor relationships, routine-care stabilization fails and
the system recreates the old full-time benefit cliff under a new name.

---

## Metrics and Evaluation

DoDA evaluates the framework using pre-specified metrics. Key indicators include
preventive dental utilization rates by income quintile, age, region, and employment
type; HTA dental spending by service category; employer contribution adequacy relative
to routine-care costs; income-graduated dental subsidy utilization; dental appointment
availability and wait times; price dispersion for standardized dental services;
provider participation in the unified rail; emergency dental utilization rates; acute
dental infection episodes; trauma and maxillofacial SEC claims; avoidable restorative
escalation rates; patient out-of-pocket dental burden; credit uptake and distribution;
fraud and anomalous billing patterns; and impact on SEC claim frequency and severity
where measurable.

Evaluation must distinguish between utilization growth caused by improved access and
cost growth caused by provider price inflation. Increased preventive utilization is an
intended effect. Unexplained price acceleration is not.

---

## Phase Strategy

Phase 0 focuses on definition and baseline. HETA defines standardized dental service
bundles. DoDA establishes baseline utilization, access, price, and emergency dental
metrics. The portal displays routine dental prices voluntarily where providers opt in.

Phase 1 activates HTA eligibility and price display. Routine dental services become
eligible for HTA settlement. Participating providers post machine-readable prices.
Patients can compare providers through the portal. Employer HTA contributions may be
used for qualifying routine dental services.

Phase 2 introduces income-graduated dental credits. Income-graduated routine-care
subsidies apply to preventive dental services. Provider-side blindness is enforced.
DoDA monitors subsidy capture, access, and price movement.

Phase 3 activates preventive utilization attestation. SSI and UPI attestations go
live. Patients completing the defined preventive utilization standard receive account
credits or related benefits where authorized.

Phase 4 enables actuarial risk attenuation. DoDA-certified models permit preventive
utilization attestations to update actuarial reference classifications or reserve
requirements. Credits remain upside-only unless Congress later authorizes a stronger
rule after access adequacy certification.

Phase 5 scales nationally and adjusts based on pilot evidence. HETA updates bundle
definitions, anti-gaming rules, and settlement logic based on what the pilots
actually showed.

---

## What This Is Not

This is not dental insurance. It is not a return to employer-sponsored health plans.
It is not a new Medicaid dental carveout. It is not a punitive wellness program. It
is not a provider network. It is not a social credit system. It is not SEC coverage
for routine dental services.

It is a market-layer financing and settlement framework that makes routine dental care
payable through the same account architecture as other routine care, while allowing
verified prevention to improve actuarial modeling and return part of the expected
savings to households.

---

## Draft Statutory Language Sketch

Section 1 establishes HTA eligibility. Routine dental services, as defined by the
Secretary through HETA-maintained service bundle standards, shall be eligible for
payment through Health Transition Accounts on the same basis as other market-layer
healthcare services.

Section 2 preserves the SEC boundary. Nothing in this Act shall be construed to make
routine dental services covered under Severe Event Coverage. SEC coverage for dental
services shall apply only where the dental event satisfies the clinical trigger
criteria established under the Severe Event Coverage framework.

Section 3 establishes the preventive dental utilization attestation. HETA shall
establish, in coordination with DoDA and the healthcare infrastructure layer, a
privacy-preserving attestation for qualifying preventive dental utilization. Such
attestation shall confirm only whether the individual satisfied the preventive
utilization standard and shall not disclose underlying clinical records except as
required for audit, fraud prevention, or lawful patient-authorized exchange.

Section 4 authorizes the actuarial risk attenuation credit. Where DoDA certifies that
qualifying preventive dental utilization is associated with a measurable reduction in
expected downstream cost or severe-event risk, HETA may configure the unified payment
rail to apply an actuarially calibrated credit, account contribution, premium offset,
reserve adjustment, or related benefit to the individual.

Section 5 establishes upside-only protection. Failure to satisfy the preventive dental
utilization standard shall not be used to deny coverage, increase point-of-care
charges, increase baseline SEC obligations, or impose punitive premiums during the
initial implementation period.

Section 6 governs employer contribution use. Monthly employer healthcare contributions
made under the Portable Healthcare Contribution Floor may be used for qualifying
routine dental services. Employers shall have no access to individual preventive
utilization records, dental service history, subsidy status, or actuarial
classification.

Section 7 establishes provider-side blindness. Providers shall receive only the
confirmed settlement amount and standardized reference code. Providers may not receive
information regarding the patient's income-based subsidy, employer contribution
balance, public credit, preventive utilization classification, or payer mix.

Section 8 establishes anti-gaming and enforcement authority. HETA shall maintain
anti-gaming rules for qualifying preventive dental events, including frequency limits,
service definitions, attestation requirements, anomaly detection, audit procedures,
and provider suspension authority where fraudulent or abusive patterns are identified.

---

---

## Medicaid Transition Boundary and Endodontic Cost Monitoring

### The Risk

Endodontic treatment — root canals — sits at the expensive end of the market layer.
A non-emergency root canal runs $1,500 to $2,000 or more out of pocket. That is
within the market layer by design: the overwhelming majority of endodontic
presentations are predictable, schedulable, and comparable across providers. The
brief correctly places non-emergency endodontics in the market layer and acute
endodontic infection in SEC.

The risk is a perverse delay incentive. A patient without sufficient HTA balance or
subsidy coverage may defer a $1,500 root canal until the infection becomes systemic —
at which point it crosses the SEC trigger threshold and is treated at far higher cost
as an emergency event. We would be trading a manageable market-layer expenditure for
an avoidable SEC claim and a preventable health crisis. That is the wrong outcome
for the patient and the wrong outcome for the actuarial model.

This risk is concentrated in two overlapping populations: low-income workers whose
HTA balances are not yet sufficient to cover high-end market-layer dental events, and
patients transitioning off Medicaid dental coverage who are uncertain about their
cost exposure during the transition window and may delay care rather than engage with
an unfamiliar system.

### What We Suspect — and What We Need to Confirm

We expect that the Medicaid gradient layer will discount endodontic treatment
sufficiently for populations who could not reasonably absorb that cost, especially
in combination with HTA employer contributions that reduce out-of-pocket exposure.
The subsidy architecture is designed for exactly this situation — a high-cost but
schedulable and preventable event in a low-income population.

But we need the data to confirm that calibration is correct before we can rely on
it. The monitoring has to be in place before enforcement tightens — not after the
fact when avoidable SEC claims are already accumulating. The transition window is
where the risk is highest and where the data will be most informative.

### Required Monitoring

DoDA shall track the following signals from the beginning of pilot deployment,
reported on a quarterly basis during the transition period and annually thereafter:

The ratio of acute dental infection SEC claims to market-layer preventive and
restorative dental utilization, broken down by income quintile, Medicaid transition
status, and region. A rising ratio in low-income or Medicaid-transition cohorts is
a direct signal that the delay incentive is active and the subsidy calibration is
insufficient.

The share of SEC dental claims that involve endodontic origin — presentations where
a root canal that could have been treated in the market layer progressed to systemic
infection requiring SEC coverage. This measures the cost of delay directly.

Endodontic utilization rates by income quintile before and after Medicaid transition.
If utilization drops at transition and SEC dental claims rise in the same cohort,
the transition cliff is real and the calibration needs adjustment.

HTA balance adequacy for endodontic events — the share of patients who face a
market-layer endodontic cost that exceeds their combined HTA balance and applicable
subsidy. This measures whether the contribution floor and gradient are set correctly
for this specific cost category.

### Medicaid Transition Continuity Protection

Patients transitioning off Medicaid dental coverage retain access to endodontic
treatment at Medicaid-equivalent cost through Regional Health Centers or via enhanced
income-graduated subsidy for a defined transition window — initially 24 months from
the date of Medicaid transition, subject to extension if DoDA monitoring indicates
the delay incentive remains active.

This is not a permanent carve-out. It is a transition buffer designed to close the
delay incentive window while the gradient stabilizes and earns trust. It ends
automatically when DoDA certifies that endodontic utilization rates in the
transitioning cohort have stabilized at market-layer levels without a corresponding
increase in SEC dental claims.

The continuity protection applies specifically to endodontic treatment and other
high-cost but schedulable market-layer dental events. It does not extend to cosmetic
or elective services.

### Calibration Trigger

If DoDA monitoring detects that the ratio of acute dental SEC claims to market-layer
dental utilization in low-income cohorts rises above a defined threshold — specified
in the DoDA monitoring framework — HETA is authorized to adjust the income-graduated
subsidy for endodontic treatment upward without waiting for the next legislative
cycle. This adjustment is bounded, transparent, and subject to DoDA certification
of the underlying signal.

The adjustment authority exists because calibration errors in this specific category
are predictable, detectable, and correctable without structural change to the
framework. The boundary between market-layer endodontics and SEC-covered acute
infection is correct. The affordability calibration may need tuning. Those are
different problems with different solutions, and the framework treats them that way.

---

## Bottom Line

This framework closes the dental gap without rebuilding dental insurance.

Routine dental care moves into the same transparent, account-based, rail-settled
market layer as other routine care. SEC remains reserved for severe dental events.
Employer HTA contributions help part-time, gig, seasonal, and dependent-contractor
workers afford routine care without relying on full-time benefit thresholds.
Income-graduated subsidies stabilize affordability without cliffs. SSI and UPI
attestations verify preventive utilization without exposing sensitive data.
DoDA-certified actuarial models allow the system to return part of the expected
savings from prevention to households.

The result is a cleaner dental architecture: market pricing where care is shoppable,
SEC protection where care becomes severe, portable financing where labor creates
routine-care obligations, and evidence-based credits where prevention lowers risk.
