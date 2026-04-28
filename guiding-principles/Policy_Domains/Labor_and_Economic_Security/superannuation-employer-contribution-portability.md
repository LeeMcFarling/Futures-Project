---
id: superannuation-employer-contribution-portability
title: Superannuation Employer Contribution and Portability Framework
sidebar_label: Superannuation Contributions
sidebar_position: 6
slug: /labor-and-economic-security/superannuation-employer-contributions
domain: Labor_and_Economic_Security
subdomain: Wealth_Building
policy_type: Cross-Domain Integration Framework
status: Draft
version: 0.3
author: Futures Project
dependencies:
  - universal-superannuation-system
  - worker-classification-parity
  - ssi-self-sovereign-identity-framework
  - upi-privacy-preserving-payment-rail
  - irs-modernization-automated-income-attestation
  - doda-regional-wage-heatmap
related_instruments:
  - portable-healthcare-contribution-floor
  - benefits-gradient-modernization
  - regional-wage-modernization-pilot
  - codetermination-worker-board-representation
  - real-time-eitc-ctc-delivery
non_goals:
  - duplicating superannuation tax treatment or Bucket A/B framework
  - replacing the fiscal domain superannuation brief
  - defining dynasty threshold or inheritance rules
  - defining investment defaults or advisor regulation
tags:
  - labor
  - economic-security
  - superannuation
  - retirement
  - employer-contributions
  - portability
  - capital-formation
  - dependent-contractors
last_updated: 2026-04-27
---

# Superannuation Employer Contribution and Portability Framework

## What This Brief Covers and What It Doesn't

The Universal Superannuation System brief in the Budget and Fiscal domain defines the full architecture of the new retirement system: the cohort-based transition from Social Security, the Bucket A and Bucket B capital regimes, the $50 million dynasty threshold, the birth seed, the tax treatment, the investment defaults, and the macroeconomic case for prefunded capital formation over pay-as-you-go transfer.

This brief covers the labor-domain dimension of that system: specifically, how employer contributions work, which employment relationships trigger them, how portability functions across the kinds of fragmented and non-standard employment that characterize the modern labor market, and how the superannuation contribution obligation connects to the other instruments in the labor stack.

If the superannuation system is the destination — the permanent portable wealth-building floor — this brief describes the contribution mechanics that fill it for every worker, regardless of how their work is structured.

## The Problem Superannuation Solves in Labor Terms

The current retirement system has a labor market problem that is distinct from its fiscal sustainability problem. The fiscal problem — pay-as-you-go dependency on stable worker-to-retiree ratios — is addressed in the fiscal domain brief. The labor market problem is different: retirement adequacy currently depends on employer generosity, job tenure, and the worker's own financial sophistication in ways that systematically leave the most economically vulnerable workers without meaningful retirement savings.

A worker who stays with one employer for thirty years in a firm with a generous 401(k) match and automatic enrollment retires with a reasonable account balance. A worker who changes jobs frequently, works part-time, works through platforms, works as a contractor, or works for small firms without retirement plan infrastructure retires with little or nothing — not because they worked less, but because the retirement system was built around a stable, single-employer career model that describes fewer and fewer working lives.

The universal superannuation system replaces that model with a universal account that follows the worker rather than the employer. The employer contribution is mandatory and proportional rather than discretionary and match-dependent. The account is portable and individually owned rather than tied to a specific plan. And the contribution obligation applies across employment forms — full-time, part-time, gig, seasonal, and dependent contractor — rather than stopping at the edge of W-2 employment.

## How Employer Contributions Work

Covered employers contribute a fixed statutory percentage of wages directly into each worker's superannuation account via payroll. The contribution is mandatory, not discretionary. It does not depend on whether the employer has a retirement plan. It does not require the worker to contribute first to unlock the employer's share. It does not vest over time — the employer's contribution belongs to the worker immediately.

The contribution rate is set in statute. Unlike the Portable Healthcare Contribution Floor, which operates within a DoDA-managed rate range subject to effectiveness review, the superannuation contribution rate is a fixed statutory percentage because the instrument is permanent rather than transitional. Predictability is a design feature: workers and employers need a stable, long-horizon contribution rate to plan around, not one that adjusts with rulemaking cycles.

Initial contribution rates may phase in by cohort, firm size, or regional absorption capacity so that total employer labor-cost obligations — wages, payroll taxes, healthcare contributions, and superannuation — do not compound into a single large shock. The phase-in schedule is determined by statute, not rulemaking, and the final statutory rate is fixed once full implementation is reached. Phase-in is a sequencing mechanism, not a negotiating mechanism. The endpoint is known from the start. DoDA may certify regional absorption conditions and publish implementation-risk findings to inform the phase-in schedule, but the contribution rate and phase-in timeline remain statutory. Technical analysis informs; democratic authorization decides.

Contributions flow through the payroll reporting infrastructure that the IRS Modernization and Automated Income Attestation program establishes. This is the same near-real-time earnings data stream that supports Real-Time Earned Income Tax Credit (EITC) and Child Tax Credit (CTC) delivery and benefits gradient calibration. Superannuation contributions are not a separate reporting burden — they are an extension of payroll reporting to a new destination account, using the same data infrastructure the stack already relies on.

The Self-Sovereign Identity (SSI) framework and Unified Payments Interface (UPI) rail handle account portability. The worker's superannuation account is associated with their SSI identity, not with their employer or a specific plan administrator. When a worker changes jobs, the new employer begins contributing to the same account. There is no rollover, no transfer form, no waiting period, and no risk of a stranded balance sitting in a former employer's plan.

## Dependent Contractors Are Covered

The most important labor-domain extension of the superannuation system is its reach into dependent contractor relationships. The Worker Classification Parity Act establishes that workers who are economically employees — regardless of their contractual label — trigger employer-equivalent obligations. Superannuation contributions are among those obligations.

This means a gig worker, a platform worker, a seasonal worker, or any worker whose relationship with a hiring entity satisfies the dependent contractor test accrues superannuation contributions at the same statutory rate as a comparable W-2 worker. The firm that directs and benefits from the work contributes to the worker's long-run wealth accumulation proportional to the work performed. The contractor label does not exempt the firm from its contribution obligation any more than it exempts the firm from payroll tax equivalents or healthcare transition contributions.

This is the permanent capital-formation counterpart to the temporary routine-care contribution. The Portable Healthcare Contribution Floor ensures that firms cannot avoid healthcare cost responsibility by keeping workers part-time or contractor-classified during the transition period. Superannuation employer contributions ensure that firms cannot avoid retirement wealth-building responsibility permanently. One instrument is transitional. The other is structural. Both apply across the same employment relationships.

The aggregation rules from the Worker Classification Parity Act apply to superannuation contributions as well. Affiliated entities under common control are treated as a single employer. A workforce fragmented across subsidiaries, franchising arrangements, or related entities counts as a single workforce for contribution purposes. The superannuation obligation cannot be gamed through corporate structure.

## Portability Across the Modern Labor Market

The SSI/UPI account portability design resolves the primary structural problem with the current employer-sponsored retirement system: the account doesn't follow the worker.

Under the current system, a worker who changes jobs faces a decision about what to do with their 401(k) balance — roll it over, cash it out, or leave it in the former employer's plan. Each option has costs, administrative friction, and failure rates. Workers who cash out face taxes and penalties. Workers who roll over face paperwork and decision-making complexity that many navigate poorly. Workers who leave balances in former employer plans accumulate stranded accounts across their careers that are difficult to track and optimize. The net result is that job mobility — which is healthy for labor market efficiency — comes with a retirement savings tax that disproportionately affects workers who change jobs frequently, which is disproportionately lower-wage workers.

Under the universal superannuation system, there is no rollover and no decision. The account is the worker's. The employer contributes to it. When the worker leaves, the employer stops contributing and the new employer starts. The balance never moves. The account structure never changes. The worker accumulates contributions across every employer they ever work for, in the same account, without any administrative friction at the point of transition.

This portability is particularly important for the workers the current system serves worst: workers who move between full-time and part-time employment, workers who shift between W-2 and contractor relationships, workers in industries with high turnover, and workers who care for family members in ways that interrupt or reduce their employment continuity. All of those workers accumulate contributions proportional to their actual labor across every employment relationship that satisfies the contribution trigger. None of them lose contributions because they left a job or because their account was in a plan they didn't actively manage.

## The Contribution as a Component of Total Compensation

The superannuation contribution is part of the total cost of labor for covered employers. It belongs in the same analysis as wages, payroll taxes, and healthcare contributions when evaluating total compensation.

This has implications for how wage policy and superannuation interact. The Regional Wage Modernization Pilot sets minimum wage floors by commuting zone. The Benefits Gradient Modernization Act ensures that as wages rise, benefit phase-outs don't absorb the gains. The superannuation contribution adds a proportional retirement wealth-building component on top of those wages — not instead of them, but in addition to them.

The net earnings protection requirement in the Benefits Gradient brief — which requires DoDA to model whether wage floor increases actually reach households after benefit interactions — should account for superannuation contributions in its total compensation picture. A wage floor increase that improves take-home pay while leaving retirement wealth-building unchanged is a genuine improvement. A compensation package that trades wage growth for increased retirement contributions without worker knowledge or consent is a different matter.

Superannuation contributions shall not count toward statutory wage-floor compliance. The regional wage floor measures cash wages. Superannuation is an additional wealth-building contribution on top of wages, not a substitute for wages. A firm cannot satisfy a $17 regional wage floor by paying $15 in cash wages and claiming the superannuation contribution makes up the difference. DoDA may report total compensation including superannuation contributions for informational purposes, but wage-floor compliance is evaluated on cash wages alone. This guardrail prevents the superannuation contribution from becoming a mechanism for suppressing wage growth rather than supplementing it.

## Connection to Codetermination

The Codetermination Act gives workers in firms above defined thresholds board-level standing over strategic decisions including automation deployment, restructuring, and the distribution of productivity gains. One of those standing categories is productivity gain distribution — when automation or AI deployment generates documented cost savings, worker board representatives have standing to propose how a portion of those savings is distributed.

Superannuation contributions are one natural form for productivity gain distribution. A firm that automates a significant portion of its workforce, generating substantial cost savings, and whose worker board representatives propose that a portion of those savings flow into enhanced superannuation contributions for the remaining workforce, is exercising exactly the standing the Codetermination Act is designed to create. The board is required to formally respond to that proposal. The DoDA administrative record captures the response.

This connection is worth naming explicitly because it demonstrates the three-part logic of the labor governance stack in operation: credentialing and heatmap transparency make the labor market legible, wage floors and benefit gradients protect current income, and superannuation builds household balance sheets over time. Codetermination ensures workers have standing when firms make the decisions that determine which of those outcomes actually materializes.

## What This Instrument Is Not

This is not the superannuation system's primary brief. The tax treatment, Bucket A/B framework, dynasty threshold, birth seed, investment defaults, advisor regulation, and macroeconomic analysis all live in the Universal Superannuation System brief in the Budget and Fiscal domain. This brief does not duplicate any of that content.

This is not a retirement policy argument. The case for superannuation over pay-as-you-go — the fiscal sustainability argument, the demographic dependency argument, the national saving argument — is made in the fiscal domain brief. This brief takes that case as given and focuses on the labor-domain mechanics that make the contribution system work across the full range of modern employment relationships.

This is also not a temporary instrument. Unlike the Portable Healthcare Contribution Floor, which includes a conditional sunset provision tied to DoDA's assessment of whether it remains necessary, superannuation employer contributions are permanent. The healthcare contribution floor may become redundant as SEC and the benefits gradient mature. Superannuation employer contributions do not become redundant — the case for proportional employer contribution to workers' long-run wealth-building does not depend on the state of the healthcare system or the income support architecture. It depends on the principle that firms which benefit from workers' labor have an obligation proportional to that labor, permanently.

## The Permanent and Transitional Distinction

The labor stack now contains two portable employer contribution instruments with distinct roles and distinct permanence:

The Portable Healthcare Contribution Floor is transitional. It exists because employer healthcare obligations are currently thresholded and distorted. It may sunset if SEC, routine-care subsidies, and wage floors make employer healthcare contributions redundant. It is bounded, proportional, routine-care-only, and designed to step back when the conditions that make it necessary have changed.

Superannuation employer contributions are permanent. They replace the discretionary, employer-plan-dependent retirement system with a universal, portable, proportional contribution that follows every worker across every covered employment relationship for their entire working life. They do not sunset. They are not contingent on the healthcare or income support architecture. They are the permanent wealth-building floor.

The distinction matters for how each instrument is defended politically and legally. The healthcare contribution floor is defended as a transitional instrument for a specific problem during a specific period. Superannuation employer contributions are defended as a permanent structural feature of what it means to employ someone in the United States — the same category as payroll taxes, minimum wages, and workers' compensation.

## The Political Frame

Every worker who generates value for a firm should accumulate a capital stake from that work. Not a promise that depends on future workers' payroll taxes. Not a balance that vanishes when they change jobs. Not a retirement account that exists only if their employer chose to offer one and they had the financial sophistication to enroll. An owned, portable, compounding capital asset that grows across their entire working life regardless of how that life is structured.

The universal superannuation system provides the account and the seed. The employer contribution fills it proportionally to the work performed. Worker Classification Parity ensures the contribution applies across every economically dependent relationship, not just the ones labeled correctly. SSI and UPI make the account portable without administrative friction. And codetermination gives workers standing to ensure that when firms generate productivity gains, the question of how those gains are shared — including whether they flow into enhanced retirement wealth-building — is one the workforce participates in answering.

That is the complete picture: universal participation, proportional contribution, portable ownership, and governance standing. Not as separate policies, but as a coordinated system designed to work together.