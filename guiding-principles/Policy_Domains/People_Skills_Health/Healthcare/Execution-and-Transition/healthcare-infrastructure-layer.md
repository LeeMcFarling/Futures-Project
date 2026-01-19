---
title: "Healthcare Infrastructure Layer — Authentication, Authorization, APIs, and Payments"
author: "Lee McFarling"
category: "Health"
subcategories:
  - Digital Infrastructure
  - Interoperability
  - Payments
  - Data Governance
status: Draft
version: 0.1
last_updated: 2026-01-19
tags:
  - SSI
  - UPI
  - healthcare APIs
  - authentication
  - authorization
  - interoperability
  - administrative simplification
---

## Purpose and Scope

This brief defines the **Healthcare Infrastructure Layer** that underpins reformed care delivery, emergency utility regulation, and catastrophic insurance. It specifies the shared technical rails used across the system to authenticate actors, authorize actions, exchange data, and settle payments.

This layer exists to **replace manual, opaque administrative processes**—telephone calls, faxing, prior authorization queues, accessioning teams, and large billing departments—with standardized, machine-verifiable interactions.

This document defines infrastructure standards. It does not define benefit design, care delivery rules, or pricing policy.

---

## Design Goals

The infrastructure layer is designed to:

- Collapse administrative overhead by default  
- Preserve decentralized data custody  
- Enable real-time verification and settlement  
- Prevent surveillance and centralization  
- Support pluralistic vendors and providers  

Infrastructure enables execution; it does not govern care.

---

## Layer Overview

The healthcare infrastructure layer consists of four tightly coupled components:

1. **Authentication** — Who is making a request  
2. **Authorization** — What they are allowed to do  
3. **Data Exchange** — What data moves, how, and in what format  
4. **Payments** — How money settles transparently and finally  

All regulated healthcare interactions occur through these rails.

---

## 1. Authentication: Healthcare Trust Fabric

All system participants authenticate using cryptographic identity.

Participants include:
- Patients  
- Clinicians  
- Provider organizations  
- Facilities  
- Insurers  
- Public programs  

Authentication relies on:
- Decentralized identifiers (DIDs) or equivalent cryptographic identities  
- Verifiable credentials asserting role and authority (license, accreditation, insurer status)  
- Mutual authentication for all regulated requests  

Licensing and accreditation remain with states and existing bodies. The infrastructure layer standardizes **how those credentials are verified**, not who issues them.

---

## 2. Authorization: Purpose-Bound Consent and Eligibility

All actions require explicit, scoped authorization.

Authorization grants are:
- Cryptographically signed  
- Purpose-bound  
- Time-limited  
- Minimally scoped  
- Revocable  
- Logged  

### Patient Consent

Patients approve sharing of specific data bundles with specific recipients for specific purposes and durations. Consent is portable across compliant systems.

Emergency “break-glass” access is:
- Narrowly scoped  
- Automatically logged  
- Subject to mandatory post-event review  

### Eligibility and Coverage

Insurance eligibility and subsidy status are verified through attestations, not disclosure of underlying personal data. Systems confirm *eligibility*, not *identity attributes*.

---

## 3. Data Exchange: Required APIs and Standard Bundles

The infrastructure layer mandates a **minimal, uniform API surface**.

Required APIs support:
- Identity and credential verification  
- Consent verification  
- Record request and delivery  
- Eligibility confirmation  
- Audit logging  

### Standard Data Bundles

HETA defines and versions a small set of required bundles, such as:
- Continuity-of-care packet  
- Pre-operative packet  
- Emergency escalation packet  
- Medication and allergy history  
- Imaging and lab reports  

Payloads use standardized healthcare data formats. Vendors may support more, but these are mandatory.

---

## 4. Payments: Unified Settlement Rail (UPI)

Payments settle through a standardized, real-time rail.

The payment layer supports:
- Direct payment for market-based care  
- Insurance settlement for emergency and catastrophic events  
- Transparent application of subsidies or employer contributions  

Key properties:
- Prices are known and confirmed before payment  
- Settlement is final at point of service  
- No post-hoc balance billing  
- Payment records are auditable and linkable to consent and eligibility grants  

The payment rail does not set prices or benefits. It enforces transparency and finality.

---

## Data Custody and Privacy Boundaries

The infrastructure layer **does not create a centralized medical database**.

- Clinical data remains with originating providers  
- Payments data remains with financial intermediaries  
- HETA receives only aggregated, de-identified system metrics  

Individual-level access logs are visible to the patient.

Statutory prohibitions apply to:
- Cross-domain identity linkage without consent  
- Behavioral or health scoring  
- Secondary use of healthcare data outside stated purpose  

---

## How This Collapses Administrative Bureaucracy

With standardized authentication, authorization, APIs, and payments:

- Eligibility checks are instantaneous  
- Medical records move by API, not fax  
- Prior authorization is replaced by eligibility + consent  
- Billing disputes are structurally reduced  
- Administrative staffing shifts from routine handling to exception management  

Complexity is removed by design, not by enforcement.

---

## Compliance and Adoption

Compliance with the infrastructure layer is a condition of:
- Emergency utility reimbursement  
- Catastrophic insurance reimbursement  
- Participation in regulated care markets  
- Receipt of public subsidies  

Multiple vendors may implement wallets, APIs, and payment interfaces, provided they meet conformance requirements.

---

## What This Layer Is Not

This infrastructure layer is not:
- A single government system  
- A national health database  
- A mandated software vendor  
- A surveillance or monitoring platform  

It is a cryptographically sound shared plumbing that the current system is missing in order to function properly. 

---

## Bottom Line

Healthcare cannot function efficiently without modern infrastructure. By standardizing authentication, authorization, data exchange, and payment—while preserving decentralized control—this layer eliminates the fax-and-phone bureaucracy, lowers administrative costs, and makes the broader healthcare reform executable at scale.