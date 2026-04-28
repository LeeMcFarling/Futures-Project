---
id: portable-healthcare-contribution-floor
title: Portable Healthcare Contribution Floor Act
sidebar_label: Healthcare Contribution Floor
sidebar_position: 3
slug: /labor-and-economic-security/portable-healthcare-contribution-floor
domain: Labor_and_Economic_Security
subdomain: Healthcare_Transition
policy_type: Transition Framework
status: Draft
version: 1.0
author: Futures Project
dependencies:
  - healthcare-reform-sec-architecture
  - benefits-gradient-modernization
  - worker-classification-parity
  - ssi-self-sovereign-identity-framework
  - upi-privacy-preserving-payment-rail
  - irs-modernization-automated-income-attestation
  - doda-regional-wage-heatmap
related_instruments:
  - real-time-eitc-ctc-delivery
  - codetermination-worker-board-representation
  - regional-wage-modernization-pilot
non_goals:
  - employer-sponsored insurance replacement
  - generalized portable benefits mandate
  - retirement or paid leave mandates
  - permanent employer healthcare subsidy
  - competition with SEC severe-event coverage
tags:
  - labor
  - economic-security
  - healthcare-transition
  - employer-contributions
  - portable-benefits
  - hta
  - routine-care
last_updated: 2026-04-27
---

# Portable Healthcare Contribution Floor Act

## Where This Fits in the Healthcare Architecture

The reformed healthcare system rests on three distinct layers, and this Act occupies a specific and bounded role within them.

The first layer is Severe Event Coverage (SEC). SEC covers emergency and trauma care for everyone, universally, at zero cost at the point of service. This is not means-tested and does not phase out with income. A part-time worker, a gig worker, a seasonal employee — anyone — receives emergency care without a bill. That layer eliminates the catastrophic financial exposure that made employer-sponsored insurance feel essential even for workers who could barely afford it.

The second layer is the income-graduated routine care subsidy coordinated through the Benefits Gradient Modernization Act. As household income rises through the phase-out band, the subsidy for primary care and urgent care visits tapers continuously alongside food assistance and other benefits, all within the combined forty percent effective marginal tax rate ceiling. Lower-income workers pay less out of pocket for routine visits. Higher-income workers pay more. The subsidy is invisible to providers and calculated in near-real time against the worker's income attestation data.

The third layer — the one this Act creates — is the employer contribution. Severe event coverage and income-graduated subsidies together address a worker's healthcare needs as a function of what they earn and what happens to them medically. What they don't address is the question of employer responsibility. When a worker's labor generates value for a firm, does that firm have any obligation to contribute to the worker's healthcare costs? Under the current system, the answer depends on how many hours the worker logs. Above the threshold: yes. Below it: no. That threshold is the distortion this Act removes.

This Act is not coverage architecture. It is employer contribution architecture. It ensures that firms cannot avoid healthcare cost responsibility by keeping workers part-time, gig-classified, or contractor-labeled. The contributions go into portable accounts workers own. The accounts help cover routine care costs that subsidies may not fully reach. And when the healthcare stack matures to the point where those contributions are redundant, the accounts sunset rather than persist.

## The Problem This Solves

The existing employer healthcare mandate is tied to a full-time hour threshold — typically thirty or forty hours per week. Work above that line and your employer owes healthcare contributions. Work below it and they don't.

That structure creates a predictable and widespread employer response: keep enough workers below the threshold to avoid the obligation. A firm that would otherwise employ one person forty hours a week instead employs two people at nineteen hours each, contributes nothing to either worker's healthcare costs, and has effectively externalized that cost onto the workers themselves and onto the public systems they fall back on. The workers pay the difference — in coverage they have to purchase independently, in gaps during job transitions, and in deferred care when out-of-pocket costs make a visit feel unaffordable even after subsidies.

Even in the reformed system, this problem persists in a narrowed form. SEC removes the catastrophic risk. Income subsidies reduce the routine care cost burden. But a part-time worker in a high-cost commuting zone may still find that routine primary and urgent care visits create meaningful out-of-pocket friction — friction that a small per-hour employer contribution could eliminate. And the equity question remains regardless of whether the friction is severe: a firm that directs and benefits from a worker's labor has an obligation proportional to that labor, not one that disappears when the worker's hours fall below an arbitrary threshold.

The per-hour contribution structure this Act establishes is proportional rather than threshold-triggered. Every hour worked generates a contribution. There is no cliff to manage around, no threshold to stay below, no scheduling optimization that produces a healthcare cost advantage. Employers schedule based on what the work requires. Workers receive contributions based on what they actually work.

## What Healthcare Transition Accounts Are

Healthcare Transition Accounts are defined in the Healthcare domain's Employer-Sponsored Coverage Transition Framework. For purposes of this Act, the HTA is the destination account for employer routine-care contributions during the healthcare transition period. The full account architecture — reserve floor, stabilization band, contribution suspension thresholds, privacy-preserving attestation, tax treatment, and sunset conversion rules — is governed by that framework. This Act does not independently define those mechanics and defers to the healthcare domain as the source of truth.

The labor-domain role is narrower: determine when an employer contribution is owed, which workers are covered, how dependent contractors are treated, and how contributions are routed through payroll, Self-Sovereign Identity (SSI), and Unified Payments Interface (UPI) infrastructure.

One operational principle bears stating here because it governs employer administration directly. Employers do not need access to worker account balances, healthcare utilization data, or medical spending history to fulfill their contribution obligations. Contribution status is administered through a privacy-preserving SSI-backed attestation signal from the healthcare account system. The employer receives one of two states: contribution required, or contribution paused. No raw balance is disclosed. No medical data is transmitted. The worker's account state is verified through SSI-linked account infrastructure and settled through the UPI rail without exposing the underlying healthcare information to the employer.

This keeps employer administration simple — closer to payroll routing than benefits management — while preserving worker privacy and preventing the kind of health-status discrimination that would emerge if employers could see which workers were high or low healthcare utilizers.

## The Contribution Structure

All covered employers remit a standardized per-hour healthcare contribution for each employee into that employee's HTA. The rate — set as a flat dollar amount per hour or a percentage of hourly wages — applies uniformly regardless of full-time or part-time status. A worker who logs ten hours receives ten hours of contributions. A worker who logs forty hours receives forty. There is no minimum hours threshold.

The contribution rate is calibrated through rulemaking rather than fixed in the statute, but it operates within a statutory guardrail. The guardrail sets a defined range — expressed as a percentage of hourly wages or a flat dollar amount per hour — within which DoDA may recommend rate adjustments without congressional action. Adjustments outside the statutory range require congressional authorization. This prevents the instrument from becoming an uncapped payroll obligation while preserving the flexibility to respond to what DoDA's effectiveness reviews actually find.

DoDA measures whether the rate is achieving its purpose — specifically, whether HTA-funded workers show lower rates of routine care deferral and lower rates of emergency department substitution for primary and urgent care — and publishes that data as a basis for rate adjustment within the guardrail.

Dependent contractors whose relationships satisfy the dependent contractor test under the Worker Classification Parity Act are subject to employer-equivalent HTA contributions from their hiring entities. The HTA is the account into which those contributions land. This closes the loop between classification parity and portable contribution architecture: when a worker's relationship is correctly classified as economically dependent, the firm owes an employer-equivalent contribution, and the HTA provides a defined, portable account to receive it.

Aggregation rules from the Worker Classification Parity Act apply here as well. Affiliated entities under common control are treated as a single employer for contribution purposes, preventing fragmentation of a workforce across subsidiaries as a mechanism for avoiding the requirement.

## The Conditional Sunset

This Act includes an explicit conditional sunset provision because the right long-run answer depends on how the broader healthcare and wage architecture matures.

DoDA conducts a review of HTA effectiveness at defined intervals — initially at the three-year and five-year marks after national scaling. The review asks two questions. First, are HTAs materially reducing routine care deferral and emergency substitution for the workers they cover, above and beyond what SEC and the income-graduated subsidy already provide? Second, are wage floor improvements and subsidy calibration under the benefits gradient sufficient to make routine care affordable for the relevant worker population without employer contributions?

If the review finds that HTAs are redundant — that SEC coverage, the benefits gradient subsidy, and wage floor improvements together are providing adequate routine care access without the supplementary contribution mechanism — the Act sunsets or narrows on a defined schedule rather than persisting by inertia.

If the review finds that HTAs remain necessary — that employer contributions are still meaningfully reducing care deferral in ways the other instruments don't reach — the Act continues, potentially with rate adjustments based on DoDA findings.

This sunset provision is not a concession. It is the correct design for a transitional instrument. An instrument that was right during the transition should not outlast the conditions that made it necessary. Building the sunset condition in from the start is how the Act avoids becoming a permanent fixture that the system grows around rather than through.

## Employer Cost Discipline and Step-Down Logic

This Act should not be evaluated as an additional mandate layered on top of the current employer-sponsored insurance system. It is designed to operate during the transition away from that system — and the transition is designed to reduce, not increase, the total healthcare cost burden on employers over time.

Under the current structure, employers face high and volatile healthcare costs through private insurance premiums, broker layers, plan administration, network renegotiation, compliance requirements, and full-time eligibility thresholds that encourage scheduling distortions. A firm that wants to avoid benefit obligations keeps workers at nineteen hours. A firm that wants to offer good benefits spends months every year managing plan selection, open enrollment, COBRA administration, and compliance requirements that have nothing to do with whether workers are healthy. The reformed healthcare stack replaces most of that complexity with standardized, proportional, portable obligations. Severe Event Coverage handles catastrophic exposure universally. Transparent direct pricing handles routine care. Income-graduated subsidies handle affordability for lower-income workers. The per-hour HTA contribution is the employer's proportional contribution to routine-care affordability for their workforce — remitted through the same payroll and payment infrastructure already used for wages, tax withholding, and superannuation. The administrative action is direct deposit into a worker-owned account, not management of a private benefits bureaucracy.

Because HTAs are transitional, contribution obligations must be responsive to whether the healthcare stack is actually working. DoDA reviews HTA utilization, routine-care affordability, emergency substitution rates, employer contribution burdens, and regional healthcare cost trends at the three-year and five-year marks after national scaling. If SEC, routine-care subsidies, wage gains, and healthcare cost reforms together make HTAs redundant — if workers are accessing routine care without deferral and without meaningful financial friction — future employer contributions step down, narrow, or sunset on a defined schedule.

Existing worker HTA balances remain worker-owned under the terms of the healthcare-domain framework. Account balance treatment, contribution suspension thresholds, and sunset conversion rules are governed by the Employer-Sponsored Coverage Transition Framework. What this Act guarantees from the labor side is that contributions already made on behalf of a worker are not clawed back by the employer when the instrument sunsets or when the worker's account reaches the contribution suspension threshold.

Where pilot data show that employer contributions materially exceeded measured routine-care need because the healthcare cost curve fell faster than expected, Congress may authorize prospective payroll credits, contribution offsets, or accelerated step-down schedules for covered employers. The purpose is to share system savings with employers without clawing back worker-owned balances. If the system performs better than expected, employers share in the savings.

The design principle is simple: firms should contribute proportionally while the contribution is needed, and should stop contributing when the system no longer needs the instrument. The healthcare contribution floor is a bridge, not a permanent toll booth.

The Act activates in jurisdictions participating in the federal healthcare reform pilot, phasing in concurrently with SEC and the direct-pay routine care markets. It does not apply nationally from day one. Piloting first allows the contribution structure, HTA mechanics, and UPI/SSI settlement infrastructure to be validated in practice before national scaling.

Pilot regions implement the per-hour contribution requirement, HTA capitalization and usage rules, and reporting infrastructure integrated with the healthcare and income support systems operating in the same jurisdiction. The pilot runs for twenty-four to thirty-six months. Evaluation measures hour distribution changes, employer scheduling behavior, hours bunching around previously contribution-sensitive thresholds — to confirm the per-hour structure eliminated the scheduling distortion rather than just shifting it — routine care utilization rates among HTA-covered workers, emergency department substitution rates, coverage continuity during employment transitions, and administrative burden on employers.

National scaling follows pilot evaluation and SSI/UPI readiness certification. The conditional sunset review schedule begins from the date of national scaling.

## The Three-Part Doctrine

The cleanest way to understand this instrument's role is through the three-part doctrine that governs the healthcare and labor stack:

SEC makes workers safe from catastrophic medical exposure. The benefits gradient makes routine-care subsidies taper smoothly as income rises. The Portable Healthcare Contribution Floor makes employer healthcare contributions portable and proportional so that firms cannot avoid health-cost responsibility by keeping workers part-time, gig, seasonal, or contractor-classified.

Each instrument addresses a different failure. SEC addresses the catastrophic risk that left uninsured workers financially exposed to medical bankruptcy. The benefits gradient addresses the cliff in the income support system that previously made earning more potentially leave a household worse off after losing healthcare coverage. This Act addresses the employer-side evasion that allows firms to benefit from workers' labor without contributing proportionally to their healthcare costs.

The three instruments are not redundant. They are complementary. And when the conditions that make this Act necessary have changed enough that DoDA's review finds it redundant, it sunsets — having served its transitional purpose without becoming a structural fixture.

## The Political Frame

There is a simple principle underneath this Act: if a firm benefits from a worker's labor, it has an obligation proportional to that labor — not one that disappears when the worker's hours fall below a line someone drew in 1974.

The threshold-based mandate was not designed to create hour-splitting. It was a side effect of structuring the obligation as an on/off switch rather than a proportional contribution. This Act replaces the switch with a dial. The obligation scales with the work. The employer can't avoid it by scheduling to nineteen hours. The worker accumulates contributions that follow them across jobs. And when the broader healthcare system has matured to the point where the dial is no longer necessary, it turns itself off.

That is a straightforward, defensible instrument. It does not rebuild employer-sponsored insurance. It does not compete with universal severe event coverage. It fills one specific gap — proportional employer contribution for workers whose labor would otherwise generate zero healthcare obligation — and it does so in a way designed to step back when that gap closes.