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
domain: Healthcare
subdomain: Care_Delivery_and_Insurance
policy_type: Market Integration Framework
status: Draft
version: 0.1
author: Futures Project
last_updated: 2026-03-23
dependencies:
  - care-delivery-market-design
  - insurance-architecture-sec
  - healthcare-infrastructure-layer
  - heta-revised-charter
related_initiatives:
  - regional-health-center-network
  - cost-performance-backstop
  - emergency-trauma-services
description: >
  Integrates dental, vision, and outpatient mental health into the restructured
  healthcare market as shoppable direct-pay services, defines SEC trigger events
  for each domain, establishes the optional discount wrap instrument, and specifies
  the patient-side price display requirement through the unified payment rail.
---

## Purpose and Scope

This brief formally integrates dental care, vision care, and outpatient mental health
into the restructured healthcare market framework. It defines their placement in the
market layer, establishes SEC trigger boundaries for each domain, specifies the
optional low-cost discount wrap instrument, and formalizes the patient-side price
display requirement through the unified payment infrastructure.

This document extends the Care Delivery Market Design framework and the Insurance
Architecture framework. It does not modify their core structures — it applies them to
three service domains that were previously excluded or inconsistently treated.

---

## Why These Three Domains Were Previously Excluded

Dental, vision, and mental health share a structural history: they were carved out of
mainstream insurance markets decades ago and never properly reintegrated. The result
is a patchwork of standalone plans with low annual caps, high administrative overhead,
narrow networks, and chronic underutilization — particularly among low-income and
rural populations.

Traditional dental insurance illustrates the failure clearly. A typical plan carries a
$1,500 annual benefit maximum — a figure largely unchanged since the 1970s — with
deductibles, waiting periods, and exclusions that make it nearly worthless for
anything beyond routine cleanings. It functions more like a discount card with
expensive paperwork than genuine risk protection.

Mental health has been subject to systematic parity violations despite federal law
requiring equal treatment. Vision insurance similarly operates more as a discount
network in most plans than as true insurance.

This framework corrects the structural misclassification. Routine services in all
three domains belong in the market layer. Acute and severe events belong in SEC. The
boundary between them is clinical, not financial.

---

## Core Design Principle

Dental, vision, and outpatient mental health are shoppable services. They are
predictable, schedulable, and comparable. Patients can research providers, compare
prices, and make informed decisions in advance. That makes them market-layer services
under the same logic that governs primary care and urgent care.

Insurance is removed from routine services in these domains for the same reason it is
removed from primary care: its presence suppresses price signals, inflates
administrative overhead, and rewards opacity over value. Coverage is restored
precisely where the shoppable nature breaks down — when a clinical event makes the
service time-critical, non-elective, and high-cost. Those events are covered by SEC.

---

## Domain Placement: Market Layer

Dental market-layer services include preventive care — cleanings, examinations,
X-rays, sealants, fluoride treatments — as well as restorative care including
fillings, crowns, bridges, inlays, and onlays. Periodontal maintenance and
non-surgical treatment, endodontic treatment such as root canals for non-emergency
presentations, prosthodontics including dentures and scheduled implants, orthodontics,
and cosmetic procedures all operate in the market layer.

Vision market-layer services include comprehensive eye examinations, refraction and
prescription determination, eyeglasses and contact lens fitting and dispensing,
elective refractive surgery, and routine management of stable chronic conditions such
as dry eye or stable glaucoma.

Mental health market-layer services include outpatient individual therapy and
counseling, outpatient group therapy, outpatient psychiatric medication management,
outpatient substance use counseling, psychological testing and assessment outside of
crisis contexts, and telehealth mental health services.

---

## SEC Trigger Boundaries

Severe Event Coverage activates when a dental, vision, or mental health situation
crosses from shoppable into acute, non-elective, or high-cost territory. The trigger
is clinical, not financial. There is no deductible threshold. Coverage activates on
the defined event.

For dental, SEC triggers include oral and maxillofacial surgery arising from trauma,
fracture, abscess, or pathology requiring surgical intervention under general or IV
sedation; dental care required as part of a covered medical episode such as extraction
prior to cardiac surgery or treatment of oral infection in an immunocompromised
patient; acute dental infection with systemic involvement including facial swelling,
fever, or airway risk; and trauma-related dental injury arising from an emergency or
trauma admission. Routine root canals, crowns, and periodontal treatment that are
scheduled and elective remain market-layer services. The SEC trigger is clinical
urgency and systemic involvement, not procedure type.

For vision, SEC triggers include acute vision-threatening events such as retinal
detachment, acute angle-closure glaucoma, sudden vision loss, ocular trauma, and
chemical burns; vision loss or impairment arising from a covered medical episode
including diabetic retinopathy requiring acute intervention or stroke-related vision
loss; and ophthalmic surgery required as part of a covered medical episode. Routine
cataract surgery is a scheduled elective procedure covered under the Scheduled Surgery
framework as a bundled episode. Emergent cataract surgery following trauma is
SEC-triggered.

For mental health, SEC triggers include inpatient psychiatric admission for acute
psychiatric crisis including suicidality, psychosis, severe mania, or acute severe
depression requiring inpatient stabilization; crisis stabilization unit admission
requiring 24-hour supervised care; intensive outpatient or partial hospitalization
programs arising from acute psychiatric deterioration following a covered inpatient
event; and substance use disorder requiring medically supervised detoxification where
medical monitoring is clinically required. Ongoing outpatient therapy, medication
management, and standard IOP programs not arising from an acute inpatient event are
market-layer services.

---

## Mental Health Parity Rule

Outpatient mental health services in the market layer are subject to an explicit
anti-tiering rule. Discount wrap products and any supplemental coverage operating
above the SEC floor may not apply prior authorization to outpatient mental health
services that is not applied to comparable medical or surgical outpatient services,
impose session limits that do not apply to comparable medical services, apply higher
cost-sharing to mental health services than to comparable medical services, or exclude
telehealth mental health services while covering telehealth for other market-layer
services.

This rule applies to all products operating in the market layer for mental health,
including discount wraps, supplemental plans, and employer-sponsored supplemental
packages. It is enforced by HETA as a condition of market participation. It reflects
the federal Mental Health Parity and Addiction Equity Act and extends it to the
restructured market-layer context — not as a separate compliance obligation, but as a
structural condition of access.

---

## The Optional Discount Wrap

Patients may optionally enroll in a low-cost Discount Wrap for dental, vision, and
mental health services. The discount wrap is not insurance. It is a negotiated rate
network with a monthly participation fee.

The wrap entitles enrolled patients to discounted rates at participating providers.
It is a direct arrangement between the patient and the provider network — no insurance
intermediary, no claims processing, no deductible, no annual cap, no prior
authorization, and no adjudication. The patient pays the provider directly at the
negotiated rate. That is the entire transaction. It is a credential in the patient's
SSI health wallet, verified at point of service through the unified payment rail.
Multiple wrap products may compete in the market. Patients select through the unified
app. Wrap administrators must publish participating provider lists and negotiated rates
in machine-readable format and may not impose exclusions, waiting periods, or
utilization controls of any kind. The product is access to discounted rates, nothing
more.

When a patient presents at a participating provider, their wrap credential is verified
through the SSI layer. The payment rail applies the negotiated rate automatically. The
provider receives confirmed payment at the wrap rate. No manual verification, no phone
calls, no claims submission.

---

## Patient-Side Price Display

The patient-side price display is the most important patient-facing feature of this
framework for these three domains. It corrects the information asymmetry that has
historically made dental, vision, and mental health markets opaque and inaccessible
for lower-income patients.

At the point of service — and through the unified patient app prior to booking —
patients see a single "your price" figure for any service at any participating
provider. This figure is calculated silently by the payment rail from three inputs:
the provider's posted market price, the discount wrap rate if the patient holds an
active credential, and the income-adjusted subsidy credit applied automatically based
on the patient's current income tier attestation verified through SSI without
disclosing underlying income data to the provider.

The patient sees one number. The provider sees a confirmed payment amount. The subsidy
arithmetic is invisible to the provider. This is not incidental — it is structural.
Providers who can see patient subsidy status will tier availability by payment level,
price to subsidy rather than to market, and reproduce the two-tier access dynamics
this reform is designed to eliminate. Provider-side invisibility is enforced through
the payment rail architecture, not through discretionary policy.

For patients, the display is framed as a credit applied to their price:

> **Service:** Dental cleaning — $120
> **Your price:** $34
> **Subsidy credit applied:** $86

This framing is consistent across all income tiers. The amount differs; the format
does not. Research on benefit program uptake consistently shows that stigma and
complexity are the two primary barriers to utilization among eligible populations.
The display format is designed to minimize both.

The patient-side display is available before booking, not only at checkout. Through
the unified patient app, a patient can search for providers, see their price for any
service at any participating provider, compare prices before scheduling, and book
directly with price confirmed at time of booking. Pre-visit discovery is where
competitive market pressure is actually generated. Provider selection is where pricing
behavior changes.

---

## Provider Transparency Requirements

Participating dental, vision, and mental health providers must post all prices in
machine-readable format accessible through the unified provider registry, update
prices on a defined cadence with no more than 30 days lag, honor posted prices as
binding with no post-hoc add-ons or facility fees, and accept confirmed payment
through the unified payment rail as final settlement for market-layer services.

Subscription and membership models are permitted for dental and mental health where
longitudinal continuity adds clinical value, subject to the same disclosure
requirements as primary care subscriptions — scope of included services, access
standards, panel size limits, and per-visit pricing for patients who want episodic
access without membership.

Participating providers receive a regional market positioning dashboard through
HETA's infrastructure layer showing their price position relative to regional peers
in percentile bands, panel-adjusted peer comparisons for similar practice types, and
time-series views of their pricing relative to regional trends. The dashboard is
non-punitive in early phases — informational only, with no enforcement consequence
during the transition window. It shows market position, not individual competitor
prices, preventing collusion while enabling rational self-adjustment. Dashboard data
is held under the enforcement firewall provisions of the HETA Revised Charter and
cannot be used for enforcement purposes.

---

## Provider Transition Support

Dental, vision, and mental health providers are explicitly included in the HETA
Provider Transition Corps deployment. These providers face the same structural
anxieties as other clinicians navigating the transition, with some domain-specific
additions. Dentists typically carry high practice acquisition or buildout debt on top
of school loans, and current pricing structures reflect that debt service load. Mental
health providers already operate on thin margins with high administrative burden from
existing insurance billing requirements. Vision providers in retail contexts face a
different consolidation dynamic than independent practices.

The regional office model, case manager assignment, and full suite of PCA transition
instruments are available to providers in all three domains. The non-punitive
dashboard period is particularly important here. Dental and mental health providers
need to trust that posting prices and connecting to the rail does not immediately
expose them to enforcement action based on their current pricing. The transition
window is real and its terms are explicit.

---

## Interface with SEC and Emergency Care

When a dental, vision, or mental health situation meets a defined SEC trigger, the
encounter transitions from market-layer to SEC-covered automatically. The provider
notifies through the unified payment rail using defined clinical escalation codes. SEC
coverage activates at the episode level, covering all services required to treat the
triggering event. The provider is reimbursed at SEC rates, not market rates, for the
covered episode.

Providers may not retroactively reclassify routine encounters as SEC trigger events.
Misclassification is subject to the same anti-gaming enforcement as emergency upcoding
under the broader framework. Legal safe harbor applies to providers who escalate
appropriately and in good faith when a clinical threshold is met.

---

## Transition Timeline

Dental, vision, and mental health market integration follows the same phase structure
as the broader healthcare transition. Phase 0 establishes regional offices, provider
outreach, dashboard rollout on a non-punitive informational basis, and opens the
discount wrap administrator market alongside patient app beta. Phase 1 makes price
posting voluntary with rail connection incentivized but not required and wrap
credentials operational. Phase 2 requires price posting as a condition of public
program reimbursement. Phase 3 activates full market-layer enforcement in prepared
districts. Providers in all three domains are eligible for PCA transition instruments
beginning in Phase 0.

---

## Bottom Line

Dental, vision, and outpatient mental health have been structurally mismanaged for
decades — carved out of mainstream coverage, capped at arbitrary benefit limits, and
left to operate in opaque markets that served neither patients nor providers well.

This framework ends that by applying the same logic that governs the rest of the
reformed market: direct pay where services are shoppable, SEC coverage where they are
not, transparent prices visible to patients before they walk in the door, and subsidy
credits applied automatically without stigma or administrative friction.

The low-cost discount wrap is not insurance dressed up as something cheaper. It is
the honest product for routine predictable care — a negotiated rate network without
the overhead. SEC is the honest product for acute care — real coverage for real events
without deductible gamesmanship. Together they replace three broken coverage silos
with a coherent system that actually functions for the people who need it.
