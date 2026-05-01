---
id: preventive-dental-hta-actuarial-integration
<title>Preventive Dental, HTA Settlement, and Actuarial Risk Attenuation Framework</title>
sidebar_label: Preventive Dental & HTA
sidebar_position: TBD
slug: /healthcare/care-delivery/preventive-dental-hta-actuarial-integration
domain: Healthcare
subdomain: Care_Delivery_and_Insurance
policy_type: Cross-Domain Integration Framework
status: Draft
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

# Preventive Dental, HTA Settlement, and Actuarial Risk Attenuation Framework

## Purpose and Scope

This brief defines how routine preventive dental care integrates with the Health Transition Account / Transitional Health Account structure, the Severe Event Coverage architecture, and the labor-domain employer healthcare contribution floor.

The purpose is to prevent dental care from remaining a carved-out pseudo-insurance market while preserving the core distinction of the healthcare framework: routine, predictable, shoppable services operate in the market layer, while severe, acute, non-elective events are covered through SEC.

This brief establishes three rules.

First, routine dental care is paid through the same HTA/THA routine-care account used for other market-layer healthcare services.

Second, severe dental events are covered through SEC when they cross defined clinical triggers.

Third, verified preventive dental utilization may be used as an actuarial risk attenuation signal, allowing the system to recognize lower expected downstream risk without converting routine dental care into insurance coverage.

This brief does not create a separate dental insurance program. It does not create a provider network. It does not make routine dental care part of SEC. It defines how routine dental care is financed, displayed, settled, and recognized in actuarial modeling through existing healthcare and labor rails.

---

## Problem Statement

Dental care is structurally misclassified in the current U.S. healthcare system.

Routine dental services are predictable, schedulable, and highly price-comparable. Cleanings, examinations, X-rays, fluoride treatments, sealants, fillings, crowns, dentures, root canals, and orthodontic services can usually be scheduled in advance and compared across providers. They are therefore poorly suited to traditional insurance claims processing.

At the same time, the existing dental insurance market does not provide genuine risk protection for most households. Many dental plans function as capped discount products with narrow networks, annual benefit maximums, waiting periods, exclusions, and administrative friction. The result is underutilization of preventive care, delayed treatment, avoidable emergency dental episodes, and higher downstream health costs.

The current system also embeds a labor-market distortion. Workers with full-time employer-sponsored coverage may receive some dental support, while part-time, seasonal, gig, and dependent-contractor workers often receive none. This reproduces the hour-threshold problem found in employer-sponsored healthcare more broadly: firms can avoid benefit obligations by structuring work below coverage thresholds, and workers absorb the cost through deferred care or out-of-pocket exposure.

The reformed healthcare and labor stacks create the tools needed to correct this. HTA/THA accounts provide a portable routine-care financing vehicle. The benefits gradient provides income-based affordability support without cliffs. The employer healthcare contribution floor requires firms to contribute to routine-care costs regardless of full-time status. SSI and UPI provide privacy-preserving eligibility, utilization, and settlement rails. SEC remains available for acute, severe, high-cost dental events.

The missing piece is an integration rule that connects routine dental care to this architecture without rebuilding the failed dental insurance model.

---

## Core Design Principle

Routine dental care is market-layer care. Severe dental events are SEC-covered care. Preventive utilization is an actuarial signal.

This distinction governs the entire framework.

Routine dental care should not be insured through SEC because it is predictable and shoppable. It should be priced transparently, compared regionally, paid through portable routine-care accounts, and supported by income-based credits where appropriate.

Severe dental events should be covered by SEC when the clinical situation becomes acute, systemic, traumatic, surgical, or medically integrated with a covered episode.

Preventive dental utilization should be recognized by the actuarial system when evidence supports a measurable relationship between routine prevention and lower downstream risk. The system should not moralize preventive care. It should treat verified prevention as a risk attenuation input.

---

## Domain Placement

### Routine Dental Care — Market Layer

The following services remain market-layer services and are eligible for HTA/THA settlement:

- Routine examinations
- Preventive cleanings
- Dental X-rays within defined frequency limits
- Fluoride treatments
- Sealants
- Oral cancer screening
- Periodontal maintenance where clinically indicated
- Fillings
- Crowns
- Bridges
- Inlays and onlays
- Non-emergency root canals
- Dentures
- Scheduled implants
- Orthodontics
- Cosmetic dental services, subject to any statutory limits on subsidized use

These services are not SEC-covered merely because they are expensive. The governing test is clinical urgency and non-shoppability, not price alone.

### Severe Dental Events — SEC Layer

SEC covers dental events when they cross defined clinical triggers, including:

- Oral and maxillofacial surgery arising from trauma, fracture, abscess, pathology, or other covered medical event
- Dental care required as part of a covered medical episode, including pre-surgical extraction or infection control before cardiac surgery, organ transplant, chemotherapy, or other high-risk medical treatment
- Acute dental infection with systemic involvement, including fever, facial swelling, airway risk, or inpatient management
- Trauma-related dental injury, including avulsed, fractured, or displaced teeth resulting from an injury event covered as emergency or trauma care
- Dental procedures requiring general anesthesia or IV sedation where the clinical trigger meets SEC criteria

Routine root canals, crowns, periodontal treatment, implants, and orthodontic services remain market-layer services unless the clinical context independently triggers SEC.

---

## HTA/THA Eligibility Rule

Routine dental care shall be eligible for payment through the same HTA/THA account used for other market-layer care.

Eligible account sources may include:

- Worker-owned HTA/THA balances
- Monthly employer healthcare contribution floor deposits
- Income-graduated routine-care subsidies
- Patient direct contributions
- Approved supplemental discount wrap instruments
- Public or philanthropic dental-access credits where authorized

The rail combines these sources at settlement. The provider receives a confirmed payment and standardized reference code. The provider does not see the patient's employer contribution balance, income subsidy, public credit, private account mix, or actuarial classification.

The patient sees the full breakdown through the health wallet or public portal.

---

## Employer Contribution Integration

Under the Portable Healthcare Contribution Floor, employers make monthly contributions into worker-owned healthcare accounts. These contributions apply across full-time, part-time, seasonal, gig, and dependent-contractor work where the statutory employment or dependent-work test is satisfied.

This brief clarifies that routine dental care is an eligible use of those employer-funded account balances.

The contribution obligation is not dental insurance. It is not employer-sponsored coverage. It is a portable routine-care contribution that follows the worker, accumulates across employers where applicable, and may be combined with income-based public credits.

This rule solves the old hour-threshold distortion. A worker does not lose routine dental support because they work twenty hours instead of forty. The employer contribution may be proportional, but the right to receive portable contributions does not disappear at an arbitrary full-time boundary.

---

## Benefits Gradient Integration

Income-graduated routine-care subsidies may apply to dental services in the market layer.

Subsidies must taper under the Benefits Gradient rules so that additional earnings do not create a net loss in household resources. Dental affordability support should therefore phase down in coordination with other covered benefits, rather than operating through a separate cliff-based eligibility threshold.

The subsidy should be invisible to providers. The patient-facing portal may display the net price after applicable credits, but the provider receives only the settled amount. Providers may not price discriminate based on subsidy eligibility, employer contribution status, or account balance.

Dental affordability support should be calibrated by region, household income, household size, and local price distribution. DoDA should monitor whether subsidy increases are being captured by provider price increases in supply-constrained markets.

---

## Preventive Utilization Attestation

A qualifying preventive dental visit may generate a privacy-preserving preventive utilization attestation.

For an individual to satisfy the baseline preventive dental utilization standard, the individual must complete two qualifying preventive dental visits within a defined period, typically a calendar year or rolling twelve-month period, subject to clinical exceptions and access safeguards.

A qualifying visit may include:

- Dental examination
- Preventive cleaning
- Oral cancer screening
- Indicated X-rays within frequency limits
- Fluoride or sealant treatment where age- or risk-appropriate
- Periodontal maintenance where clinically indicated

The attestation records only that the utilization standard was satisfied. It does not expose detailed dental records to employers, insurers, providers, or public benefit administrators beyond what is required for settlement, audit, and fraud prevention.

The attestation should be held through the patient's SSI health wallet and verified through UPI-compatible settlement logic. The rail confirms status through a binary or limited-scope proof, such as:

> Preventive dental utilization standard satisfied: yes/no.

This attestation may be renewed annually or on another evidence-based cadence.

---

## Actuarial Risk Attenuation

Verified preventive dental utilization may be used to place an individual into a lower actuarial reference category where DoDA-certified evidence supports a measurable reduction in expected downstream risk.

Relevant downstream risk categories may include:

- Emergency dental utilization
- Acute infection risk
- High-cost oral surgery episodes
- Avoidable restorative escalation
- Missed work associated with untreated dental disease
- Complications in covered medical episodes where oral infection is a known risk factor
- Chronic disease management interactions where evidence supports a dental-health relationship

Actuarial recognition may take the form of:

- HTA/THA top-up
- Preventive utilization credit
- SEC premium offset, where applicable
- Routine-care subsidy enhancement
- Lower actuarial reference classification
- Reduced required reserve level within the HTA/THA account
- Payroll or refundable tax credit where legislatively authorized

The credit should be calibrated to expected savings, not political preference. DoDA certifies the evidence base and model specification. HETA configures the rail logic. The patient receives the credit automatically.

---

## Upside-Only Rule

Preventive utilization recognition shall be upside-only during initial phases.

A person who satisfies the preventive utilization standard may receive a credit, lower classification, or account benefit. A person who does not satisfy the standard remains in the ordinary reference category.

Non-utilization may not be used to deny SEC coverage, increase point-of-care charges, increase employer obligations tied to that specific worker, or impose punitive premiums during the initial implementation period.

This rule is necessary because non-utilization may reflect access barriers rather than risk preference. Rural provider shortages, transportation limits, disability, unstable work schedules, lack of childcare, distrust caused by prior medical mistreatment, language barriers, and local capacity constraints can all prevent routine dental use.

No punitive use of non-utilization may be authorized unless DoDA certifies regional access adequacy and Congress affirmatively authorizes a later-stage rule.

---

## Price Transparency and Portal Display

Routine dental services must appear in the same public portal used for other market-layer care.

For each covered dental service, the portal should display:

- Provider name and credential status
- Posted price
- Standard service bundle definition
- Local median price
- Local percentile range
- SEC or DoDA reference band where applicable
- Patient net price after available credits
- Available appointment windows
- Provider quality and safety indicators where validated
- Whether the provider accepts UPI settlement
- Whether the provider participates in approved discount wrap products

The portal should allow users to filter by service type, price, distance, availability, language, accessibility, sedation capability, pediatric availability, and regional health center participation.

Dental price comparison should use standardized procedure bundles where possible. HETA should define and version the service taxonomy to prevent providers from fragmenting comparable services into non-comparable billing units.

---

## Settlement Flow

The standard routine dental settlement flow is as follows.

First, the patient selects a dental service through the portal or receives care from a participating provider.

Second, the provider submits the standardized service code and posted price through the unified payment rail.

Third, the rail checks the patient's available HTA/THA balance, employer contribution deposits, income-graduated routine-care subsidy eligibility, and approved supplemental instruments.

Fourth, the rail calculates the patient's net responsibility and displays the settlement breakdown to the patient.

Fifth, payment settles to the provider through UPI. The provider receives the confirmed amount and reference code, but not the payer mix.

Sixth, if the service qualifies as a preventive utilization event, the rail updates the patient's preventive utilization attestation.

Seventh, if the patient satisfies the utilization standard, the rail applies the authorized actuarial risk attenuation credit or classification update.

---

## Privacy and Anti-Surveillance Guardrails

This framework must not become a health surveillance or social scoring system.

The preventive utilization attestation may only confirm that the standard was satisfied. It may not expose diagnosis, procedure detail beyond qualifying category, employer identity, exact income, subsidy amount, or full dental record.

Employers may not access individual utilization attestations. Employers satisfy their obligation by making monthly HTA contributions through payroll or approved settlement infrastructure.

Providers may not access a patient's actuarial classification, income subsidy status, employer contribution balance, or full account history.

Insurers and SEC administrators may use aggregate, de-identified, DoDA-certified utilization data for actuarial modeling, but individual-level classification changes must be executed through privacy-preserving proofs wherever technically feasible.

Public reporting should occur at aggregate levels sufficient for accountability without exposing individual behavior.

---

## Fraud, Gaming, and Abuse Controls

The rail must detect and deter abuse without creating a high-friction claims process.

Potential abuse patterns include:

- Providers submitting preventive visits that did not occur
- Upcoding routine services as preventive events
- Splitting one visit into multiple qualifying events
- Excessive frequency of X-rays or adjunctive services
- Steering patients into unnecessary add-ons
- Coordinated price increases following subsidy activation
- Creating low-value preventive appointments solely to trigger credits

Controls should include:

- Standardized qualifying-event definitions
- Frequency limits
- Provider attestation under penalty of law
- Randomized audit sampling
- Regional outlier detection
- Patient confirmation of completed service
- Peer comparison of service mix
- Automatic flags for anomalous preventive-event volume
- Suspension of credit-trigger eligibility for providers with unresolved fraud flags

The enforcement model should be pattern-based. Patients should not be forced into paperwork-heavy reimbursement processes because of provider-side gaming risk.

---

## Access Safeguards

Preventive utilization credits should not be scaled in regions where dental appointment supply is inadequate.

Before full activation, DoDA should certify regional access adequacy using metrics such as:

- Dental providers per covered population
- Appointment availability within defined time windows
- Preventive dental utilization by income quintile
- Geographic travel time to participating providers
- Regional health center dental capacity
- Mobile clinic availability
- Pediatric dental access
- Medicaid-transition population access where applicable
- Price dispersion and provider participation rates

Where access is inadequate, HETA and PCA may prioritize dental capacity expansion through Regional Health Centers, FQHCs, dental school partnerships, mobile clinics, hygienist scope expansion where state law permits, and transition support for independent dental practices connecting to the rail.

Credits may still be offered in inadequate regions if they increase access without creating penalties, but non-utilization may not be interpreted as an individual risk choice.

---

## Relationship to Regional Health Centers

Regional Health Centers should provide baseline dental capacity in underserved regions.

At minimum, covered centers should support:

- Preventive dental exams
- Cleanings
- Basic X-rays
- Fillings
- Periodontal maintenance
- Pediatric preventive services
- Oral surgery referral coordination
- Emergency dental stabilization and transfer coordination where needed

Regional Health Centers do not replace private dental practices. They establish a floor of access where market capacity is insufficient and provide a reliable pathway for low-income, rural, and high-barrier populations to satisfy preventive utilization standards.

---

## Relationship to SEC

This framework preserves SEC actuarial integrity.

Routine dental care does not become an SEC claim. Preventive dental utilization does not require SEC adjudication. HTA/THA settlement does not alter the SEC trigger boundary.

SEC remains responsible for dental events that become acute, systemic, traumatic, surgical, or medically integrated with a covered episode.

The only connection between preventive dental utilization and SEC is actuarial: verified prevention may reduce expected future severe-event risk and may therefore be recognized in risk modeling, credits, or reserve calibration.

---

## Relationship to Labor Enforcement

Employer HTA contributions must be enforceable through the labor stack.

Contribution failures, underreporting of hours, dependent-contractor evasion, payroll manipulation, or misclassification designed to avoid healthcare account obligations should trigger the Labor Stack Enforcement Framework.

Consequences may include automatic reporting flags, formula-based civil penalties, PCA access suspension, enhanced enforcement, and debarment where warranted.

The dental framework depends on this enforcement. If employers can evade monthly HTA top-ups by fragmenting labor relationships, routine-care stabilization fails and the system recreates the old full-time benefit cliff under a new name.

---

## Metrics and Evaluation

DoDA should evaluate the framework using pre-specified metrics.

Key metrics include:

- Preventive dental utilization rate by income quintile, age, region, and employment type
- HTA/THA dental spending by service category
- Employer contribution adequacy relative to routine-care costs
- Income-graduated dental subsidy utilization
- Dental appointment availability and wait times
- Price dispersion for standardized dental services
- Provider participation in the unified rail
- Emergency dental utilization rates
- Acute dental infection episodes
- Trauma and maxillofacial SEC claims
- Avoidable restorative escalation rates
- Patient out-of-pocket dental burden
- Credit uptake and distribution
- Fraud and anomalous billing patterns
- Impact on SEC claim frequency and severity where measurable

Evaluation should distinguish between utilization growth caused by improved access and cost growth caused by provider price inflation. Increased preventive utilization is an intended effect. Unexplained price acceleration is not.

---

## Phase Strategy

### Phase 0 — Definition and Baseline

HETA defines standardized dental service bundles. DoDA establishes baseline utilization, access, price, and emergency dental metrics. The portal displays routine dental prices voluntarily where providers opt in.

### Phase 1 — HTA Eligibility and Price Display

Routine dental services become eligible for HTA/THA settlement. Participating providers post machine-readable prices. Patients can compare providers through the portal. Employer HTA contributions may be used for qualifying routine dental services.

### Phase 2 — Income-Graduated Dental Credits

Income-graduated routine-care subsidies apply to preventive dental services. Provider-side blindness is enforced. DoDA monitors subsidy capture, access, and price movement.

### Phase 3 — Preventive Utilization Attestation

SSI/UPI preventive utilization attestations activate. Patients completing the defined preventive utilization standard receive account credits or related benefits where authorized.

### Phase 4 — Actuarial Risk Attenuation

DoDA-certified models permit preventive utilization attestations to update actuarial reference classifications or reserve requirements. Credits remain upside-only unless Congress later authorizes a stronger rule after access adequacy certification.

### Phase 5 — National Scaling and Adjustment

The model expands nationally after pilot evaluation. HETA updates bundle definitions, anti-gaming rules, and settlement logic based on evidence from pilot regions.

---

## What This Is Not

This is not dental insurance.

This is not a return to employer-sponsored health plans.

This is not a new Medicaid dental carveout.

This is not a punitive wellness program.

This is not a provider network.

This is not a social credit system.

This is not SEC coverage for routine dental services.

It is a market-layer financing and settlement framework that makes routine dental care payable through the same account architecture as other routine care, while allowing verified prevention to improve actuarial modeling and return part of the expected savings to households.

---

## Draft Statutory Language Sketch

### Section 1. Routine Dental HTA Eligibility

Routine dental services, as defined by the Secretary through HETA-maintained service bundle standards, shall be eligible for payment through Health Transition Accounts and Transitional Health Accounts on the same basis as other market-layer healthcare services.

### Section 2. Preservation of SEC Boundary

Nothing in this Act shall be construed to make routine dental services covered under Severe Event Coverage. SEC coverage for dental services shall apply only where the dental event satisfies the clinical trigger criteria established under the Severe Event Coverage framework.

### Section 3. Preventive Dental Utilization Attestation

HETA shall establish, in coordination with DoDA and the healthcare infrastructure layer, a privacy-preserving attestation for qualifying preventive dental utilization. Such attestation shall confirm only whether the individual satisfied the preventive utilization standard and shall not disclose underlying clinical records except as required for audit, fraud prevention, or lawful patient-authorized exchange.

### Section 4. Actuarial Risk Attenuation Credit

Where DoDA certifies that qualifying preventive dental utilization is associated with a measurable reduction in expected downstream cost or severe-event risk, HETA may configure the unified payment rail to apply an actuarially calibrated credit, account contribution, premium offset, reserve adjustment, or related benefit to the individual.

### Section 5. Upside-Only Protection

Failure to satisfy the preventive dental utilization standard shall not be used to deny coverage, increase point-of-care charges, increase baseline SEC obligations, or impose punitive premiums during the initial implementation period.

### Section 6. Employer Contribution Use

Monthly employer healthcare contributions made under the Portable Healthcare Contribution Floor may be used for qualifying routine dental services. Employers shall have no access to individual preventive utilization records, dental service history, subsidy status, or actuarial classification.

### Section 7. Provider-Side Blindness

Providers shall receive only the confirmed settlement amount and standardized reference code. Providers may not receive information regarding the patient's income-based subsidy, employer contribution balance, public credit, preventive utilization classification, or payer mix.

### Section 8. Anti-Gaming and Enforcement

HETA shall maintain anti-gaming rules for qualifying preventive dental events, including frequency limits, service definitions, attestation requirements, anomaly detection, audit procedures, and provider suspension authority where fraudulent or abusive patterns are identified.

---

## Summary

This framework closes the dental gap without rebuilding dental insurance.

Routine dental care moves into the same transparent, account-based, rail-settled market layer as other routine care. SEC remains reserved for severe dental events. Employer HTA contributions help part-time, gig, seasonal, and dependent-contractor workers afford routine care without relying on full-time benefit thresholds. Income-graduated subsidies stabilize affordability without cliffs. SSI and UPI attestations verify preventive utilization without exposing sensitive data. DoDA-certified actuarial models allow the system to return part of the expected savings from prevention to households.

The result is a cleaner dental architecture: market pricing where care is shoppable, SEC protection where care becomes severe, portable financing where labor creates routine-care obligations, and evidence-based credits where prevention lowers risk.
