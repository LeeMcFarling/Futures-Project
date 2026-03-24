---
id: dental-vision-mental-health-integration
title: Dental, Vision, and Mental Health — Market Integration Framework
sidebar_label: Dental, Vision & Mental Health
sidebar_position: 5
slug: /healthcare/care-delivery/dental-vision-mental-health
tags:
  - healthcare
  - dental
  - vision
  - mental-health
  - market-design
  - sec
  - price-transparency
  - upi
  - ssi
dependencies:
  - care-delivery-market-design
  - insurance-architecture-sec
  - healthcare-infrastructure-layer
  - HETA-revised-charter
status: Draft
version: 0.1
author: Futures Project
description: >
  Integrates dental, vision, and outpatient mental health into the restructured
  healthcare market as shoppable direct-pay services, defines SEC trigger events
  for each domain, establishes the optional discount wrap instrument, and specifies
  the patient-side price display requirement through the unified payment rail.
---

## Purpose and Scope

This brief formally integrates **dental care, vision care, and outpatient mental
health** into the restructured healthcare market framework. It defines their placement
in the market layer, establishes Severe Event Coverage (SEC) trigger boundaries for
each domain, specifies the optional low-cost discount wrap instrument, and formalizes
the patient-side price display requirement through the unified payment infrastructure.

This document extends the Care Delivery Market Design framework and the Insurance
Architecture framework. It does not modify their core structures — it applies them
to three service domains that were previously excluded or inconsistently treated.

---

## Why These Three Domains Were Previously Excluded

Dental, vision, and mental health share a structural history: they were carved out
of mainstream insurance markets decades ago and never properly reintegrated. The
result is a patchwork of standalone plans with low annual caps, high administrative
overhead, narrow networks, and chronic underutilization — particularly among
low-income and rural populations.

Traditional dental insurance is a useful illustration of the failure. A typical
plan carries a $1,500 annual benefit maximum — a figure largely unchanged since the
1970s — with deductibles, waiting periods, and exclusions that make it nearly
worthless for anything beyond routine cleanings. It functions more like a discount
card with expensive paperwork than genuine risk protection.

Mental health has been subject to systematic parity violations despite federal law.
Vision insurance similarly operates more as a discount network in most plans than
as true insurance.

This framework corrects the structural misclassification. Routine services in all
three domains belong in the market layer. Acute and severe events belong in SEC.
The boundary between them is clinical, not financial.

---

## Core Design Principle

**Dental, vision, and outpatient mental health are shoppable services.**

They are predictable, schedulable, and comparable. Patients can research providers,
compare prices, and make informed decisions in advance. This makes them market-layer
services under the framework's core design principle.

Insurance is removed from routine services in these domains for the same reason it
is removed from primary care: its presence suppresses price signals, inflates
administrative overhead, and rewards opacity over value.

**Coverage is restored precisely where the shoppable nature breaks down** — when a
clinical event makes the service time-critical, non-elective, and high-cost. Those
events are covered by SEC.

---

## Domain Placement: Market Layer

The following services operate in the direct-pay market layer under this framework:

### Dental — Market Layer Services

- Preventive care: cleanings, examinations, X-rays, sealants, fluoride treatments
- Restorative care: fillings, crowns, bridges, inlays, onlays
- Periodontal maintenance and non-surgical treatment
- Endodontic treatment: root canals for non-emergency presentations
- Prosthodontics: dentures, implants (elective and scheduled)
- Orthodontics: braces, aligners
- Cosmetic procedures

### Vision — Market Layer Services

- Comprehensive eye examinations
- Refraction and prescription determination
- Eyeglasses and contact lens fitting and dispensing
- Elective refractive surgery (LASIK, PRK)
- Routine management of stable chronic conditions (e.g., dry eye, stable glaucoma)

### Mental Health — Market Layer Services

- Outpatient individual therapy and counseling
- Outpatient group therapy
- Outpatient psychiatric medication management
- Outpatient substance use counseling
- Psychological testing and assessment (non-crisis)
- Telehealth mental health services

---

## SEC Trigger Boundaries

Severe Event Coverage activates when a dental, vision, or mental health situation
crosses from shoppable into acute, non-elective, or high-cost territory. The trigger
is clinical, not financial. There is no deductible threshold. Coverage activates
on the defined event.

### Dental SEC Triggers

- **Oral and maxillofacial surgery** arising from trauma, fracture, abscess,
  or pathology requiring surgical intervention under general or IV sedation
- **Dental care required as part of a covered medical episode** — for example,
  dental extraction required prior to cardiac surgery or organ transplant, or
  treatment of oral infection in an immunocompromised patient
- **Acute dental infection with systemic involvement** — abscess with facial
  swelling, fever, or airway risk requiring emergency treatment or inpatient
  management
- **Trauma-related dental injury** — avulsed, fractured, or displaced teeth
  resulting from an injury event covered as an emergency or trauma admission

Routine root canals, crowns, and periodontal treatment that are scheduled and
elective are market layer services. The SEC trigger is the clinical urgency and
systemic involvement, not the procedure type.

### Vision SEC Triggers

- **Acute vision-threatening events** — retinal detachment, acute angle-closure
  glaucoma, sudden vision loss, ocular trauma, chemical burns
- **Vision loss or impairment arising from a covered medical episode** — diabetic
  retinopathy requiring acute intervention, stroke-related vision loss, vision
  complications of covered surgical procedures
- **Ophthalmic surgery required as part of a covered medical episode**

Routine cataract surgery is a scheduled, elective procedure and is covered under
the Scheduled Surgery framework as a bundled episode, not under this domain's
SEC trigger list. Emergent cataract surgery following trauma is SEC-triggered.

### Mental Health SEC Triggers

- **Inpatient psychiatric admission** — voluntary or involuntary hospitalization
  for acute psychiatric crisis, including suicidality, psychosis, severe mania,
  or acute severe depression requiring inpatient stabilization
- **Crisis stabilization unit admission** — residential crisis treatment requiring
  24-hour supervised care
- **Intensive outpatient or partial hospitalization programs** arising from acute
  psychiatric deterioration following a covered inpatient event
- **Substance use disorder requiring medically supervised detoxification** —
  inpatient or residential detox where medical monitoring is clinically required

Ongoing outpatient therapy, medication management, and standard IOP programs
not arising from an acute inpatient event are market layer services.

---

## Mental Health Parity Rule

Outpatient mental health services in the market layer are subject to an explicit
**anti-tiering rule**.

Discount wrap products and any supplemental coverage operating above the SEC floor
may not:

- Apply prior authorization to outpatient mental health services that is not
  applied to comparable medical or surgical outpatient services
- Impose session limits that do not apply to comparable medical services
- Apply higher cost-sharing to mental health services than to comparable
  medical services
- Exclude telehealth mental health services while covering telehealth for
  other market-layer services

This rule applies to all products operating in the market layer for mental health,
including discount wraps, supplemental plans, and employer-sponsored supplemental
packages. It is enforced by HETA as a condition of market participation.

The parity rule reflects the federal Mental Health Parity and Addiction Equity Act
and extends it to the restructured market layer context. It is a structural condition
of market access, not a separate compliance obligation.

---

## The Optional Discount Wrap

Patients may optionally enroll in a low-cost **Discount Wrap** for dental, vision,
and mental health services. The discount wrap is not insurance. It is a negotiated
rate network with a monthly participation fee.

### What the Discount Wrap Is

- A negotiated rate agreement between participating providers and the wrap administrator
- A monthly fee entitling the enrolled patient to discount wrap rates at
  participating providers
- A credential in the patient's SSI health wallet, verified at point of service
  through the unified payment rail
- Explicitly not insurance — no claims processing, no deductible, no annual cap,
  no prior authorization, no adjudication

### What the Discount Wrap Is Not

- Insurance of any kind
- A substitute for SEC coverage
- A requirement for accessing market-layer services
- A closed network — patients may see any provider, but only receive discount
  rates at participating providers

### Pricing and Participation

- Monthly fee is set competitively by wrap administrators operating in the market
- Multiple wrap products may compete; patients select through the unified app
- Wrap administrators must publish participating provider lists and negotiated
  rates in machine-readable format
- Wrap administrators may not impose exclusions, waiting periods, or utilization
  controls of any kind — the product is access to discounted rates, nothing more

### Discount Wrap as a Market Credential

When a patient presents at a participating provider, their wrap credential is
verified through the SSI layer. The payment rail applies the negotiated rate
automatically. The provider receives confirmed payment at the wrap rate. No
manual verification, no phone calls, no claims submission.

---

## Patient-Side Price Display

This is the framework's most important patient-facing feature for these three
domains. It corrects the information asymmetry that has historically made dental,
vision, and mental health markets opaque and inaccessible for lower-income patients.

### The Display Requirement

At the point of service — and through the unified patient app prior to booking —
patients see a single **"your price"** figure for any service at any participating
provider. This figure is calculated silently by the payment rail from three inputs:

1. **Posted market price** — the provider's publicly listed price, mandatory
   and binding under transparency rules
2. **Discount wrap rate** — applied automatically if the patient holds an active
   wrap credential, verified through SSI
3. **Income-adjusted subsidy credit** — applied automatically based on the
   patient's current income tier attestation, verified through SSI without
   disclosing underlying income data to the provider

The patient sees one number. The provider sees a confirmed payment amount. The
subsidy arithmetic is invisible to the provider.

### Why Provider-Side Invisibility Matters

Providers must not be able to see patient subsidy status. If they could:

- Providers would tier availability by payment level, creating de facto
  two-tier access within the market layer
- Providers in low-income areas would price to subsidy rather than to market,
  distorting the regional price signals their dashboard is designed to reflect
- The stigma associated with means-tested benefits would suppress utilization
  among eligible patients

Provider-side invisibility is structural, not discretionary. It is enforced
through the payment rail architecture — providers receive a confirmed payment
amount, not a breakdown of how it was calculated.

### Subsidy Display Framing

For patients, the display is framed as a credit applied to their price, not as
a percentage discount or a poverty indicator. The framing is:

> **Service:** Dental cleaning — $120  
> **Your price:** $34  
> **Subsidy credit applied:** $86

This framing is consistent across all income tiers. A patient receiving a modest
subsidy and a patient receiving a large subsidy see the same format. The amount
differs; the framing does not. Research on benefit program uptake consistently
shows that stigma and complexity are the two primary barriers to utilization among
eligible populations. The display format is designed to minimize both.

### Pre-Visit Price Discovery

The patient-side display is available before booking, not only at checkout. Through
the unified patient app, a patient can:

- Search for dental, vision, or mental health providers in their area
- See their "your price" for any service at any participating provider
- Compare prices across providers before scheduling
- Book directly through the app with price confirmed at time of booking

This pre-visit discovery is where competitive market pressure is actually generated.
Checkout visibility matters, but provider selection is where pricing behavior changes.

---

## Provider Transparency Requirements

Participating dental, vision, and mental health providers must:

- Post all prices in a machine-readable format accessible through the unified
  provider registry
- Update prices on a defined cadence (no more than 30 days lag)
- Honor posted prices as binding — no post-hoc add-ons, facility fees, or
  unbundled charges
- Accept confirmed payment through the unified payment rail as final settlement
  for market-layer services

Subscription and membership models are permitted for dental and mental health
where longitudinal continuity adds clinical value, subject to the same disclosure
requirements as primary care subscriptions under the Care Delivery framework:

- Scope of included services
- Access standards and response times
- Panel size limits
- Per-visit pricing for patients who want episodic access without membership

### Provider Dashboard

Participating providers receive a **regional market positioning dashboard**
through HETA's infrastructure layer. The dashboard shows:

- The provider's price position relative to regional peers (percentile bands)
- Panel-adjusted peer comparisons for similar practice types
- Time-series views of their pricing relative to regional trends

The dashboard is:

- **Non-punitive in early phases** — informational only, with no enforcement
  consequence during the transition window
- **Not granular at the competitor level** — providers see their position
  relative to the market, not individual competitor prices, preventing
  collusion while enabling rational self-adjustment
- **Accessible through the regional office** — case managers can walk providers
  through their dashboard during onboarding and at any point during transition

Provider dashboard data is held under the enforcement firewall provisions of the
HETA Revised Charter Section 9. Case manager access to dashboard data is for
transition support only and cannot be used for enforcement purposes.

---

## Provider Transition Support

Dental, vision, and mental health providers are explicitly included in the HETA
Provider Transition Corps deployment under the revised charter.

These providers face the same structural anxieties as other clinicians — debt
loads, administrative overhead, uncertainty about pricing in a transparent market —
with some domain-specific additions:

- Dentists typically carry high practice acquisition or buildout debt on top of
  school loans, and current pricing structures reflect that debt service load
- Mental health providers already operate on thin margins with high administrative
  burden from existing insurance billing requirements
- Vision providers in retail contexts face a different consolidation dynamic
  than independent practices

The regional office model, case manager assignment, and full suite of PCA
transition instruments are available to providers in all three domains. Instrument
availability is calibrated by domain and practice type.

The non-punitive dashboard period is particularly important for these domains.
Dental and mental health providers need to trust that posting prices and connecting
to the rail does not immediately expose them to enforcement action based on their
current pricing. The transition window is real and its terms are explicit.

---

## Interface with SEC and Emergency Care

When a dental, vision, or mental health situation meets a defined SEC trigger:

- The encounter transitions from market-layer to SEC-covered automatically
- The provider notifies through the unified payment rail using defined clinical
  escalation codes
- SEC coverage activates at the episode level, covering all services required
  to treat the triggering event
- The provider is reimbursed at SEC rates, not market rates, for the covered episode

Providers may not retroactively reclassify routine encounters as SEC trigger events.
Misclassification is subject to the same anti-gaming enforcement as emergency
upcoding under the broader framework.

Legal safe harbor applies to providers who escalate appropriately and in good faith
when a clinical threshold is met.

---

## Transition Timeline

Dental, vision, and mental health market integration follows the same phase
structure as the broader healthcare transition:

- **Phase 0** — regional office establishment, provider outreach, dashboard
  rollout (non-punitive, informational only), discount wrap administrator
  market opens, patient app beta
- **Phase 1** — voluntary price posting, rail connection incentivized but
  not required, wrap credentials operational
- **Phase 2** — price posting required as condition of public program
  reimbursement (Medicaid, subsidized plans)
- **Phase 3** — full market layer enforcement activated in prepared districts

Providers in all three domains are eligible for PCA transition instruments
beginning in Phase 0.

---

## Bottom Line

Dental, vision, and outpatient mental health have been structurally mismanaged
for decades — carved out of mainstream coverage, capped at arbitrary benefit
limits, and left to operate in opaque markets that served neither patients nor
providers well.

This framework ends that by applying the same logic that governs the rest of the
reformed market: direct pay where services are shoppable, SEC coverage where they
are not, transparent prices visible to patients before they walk in the door, and
subsidy credits applied automatically without stigma or administrative friction.

The $5–10 monthly discount wrap is not insurance dressed up as something cheaper.
It is the honest product for routine predictable care — a negotiated rate network
without the overhead. SEC is the honest product for acute care — real coverage
for real events without deductible gamesmanship.

Together they replace three broken coverage silos with a coherent system that
actually functions for the people who need it.
