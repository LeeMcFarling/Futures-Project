---
id: idp-information-integrity-digital-nutrition
title: Information Integrity & Digital Nutrition (IDP)
sidebar_label: Information Integrity & Digital Nutrition
sidebar_position: 6
slug: /idp/information-integrity-digital-nutrition
domain: Technology_and_Data
subdomain: Information Integrity & Platform Governance
policy_type: Alliance Infrastructure Brief
status: Draft
version: 0.2
author: Futures Project
dependencies:
  - Digital Identity (SSI / DIDs)
  - Platform Transparency Standards
  - Civic Rater Programs
related_initiatives:
  - Digital Nutrition Labeling
  - AI Governance
  - Platform Accountability
  - Integrated Defense Partnerships (IDP)
non_goals:
  - truth adjudication
  - content removal
  - viewpoint moderation
  - algorithmic ranking mandates
  - identity disclosure mandates
tags:
  - information-integrity
  - epistemic-infrastructure
  - platform-governance
  - civil-liberties
last_updated: 2026-02-08
---

# Information Integrity & Digital Nutrition (IDP)

## Purpose

This brief defines an alliance-compatible framework for strengthening information integrity by exposing structural signals about *how* information is presented and amplified, without adjudicating truth, moderating viewpoints, or centralizing epistemic authority. The system is explicitly limited to surfacing two descriptive signals to users at scale: (1) relative partisanship and (2) degree of factual language versus opinion or persuasive expression. The objective is to make distortion and bad-faith amplification legible, not to determine what is correct or factually accurate.

This framework is designed under an explicit assumption of **partial capture and bias at all times**. It is structured to expect the bad faith of governments, corporations, platforms, experts, and institutions. Any system operating at scale will be pressured, distorted, or partially captured; the framework is engineered to remain resilient under those conditions by design.

## Core Claim

The modern Western information ecosystem is dominated by corporate platforms operating opaque, engagement-optimized algorithms. Citizens in democratic societies are exposed to a constant firehose of information, much of it presented as “truth,” while context, sourcing, and evidentiary posture are fragmented across platforms, publishers, aggregators, and paywalls. Developing a coherent understanding of any major event increasingly requires navigating multiple proprietary systems optimized for attention rather than comprehension.

The prevalence of divisive and extreme partisanship is not an accidental byproduct of free expression; it is evidence of structural failure in how information is mediated and amplified. At the same time, democratic societies that value freedom of expression cannot and should not appoint any government, alliance, corporation, or institution to decide truth. Citizens also cannot reasonably be asked to trust opaque private systems, corporate incentives, or centralized authorities to act consistently in the public interest.

This framework is built around that reality. The only durable response is not truth adjudication, but the systematic exposure of informational distortion so it becomes visible, contestable, and comparable.

The framework works precisely because it expects bias and capture. Disagreement, variance, and divergence across observers are not failures to be corrected; they are the signal. Legitimacy is preserved not by eliminating bias, but by making it observable.

Democratic societies cannot and should not decide what is true. They can, however, ensure that citizens can plainly see when content is highly partisan, primarily persuasive, weakly evidenced, or structurally amplified in ways that distort perception. This framework restores visibility into information structure rather than asserting epistemic authority.

## Problem Statement

Modern information environments are mediated by highly centralized, engagement-optimized systems that neither governments nor citizens meaningfully govern, audit, or diversify. These systems amplify emotionally salient and identity-reinforcing content, tolerate large-scale automation, and obscure provenance, coordination, and evidentiary posture. Though often described as shared public squares, they function as segmented attention markets in which citizens see reinforcing agreement and only the most extreme caricatures of disagreement.

This creates a systemic vulnerability. Adversarial and bad-faith actors do not need to persuade at scale; they exploit amplification mechanics to flood the environment with hyper-partisan, low-evidence, or purely persuasive content. When these structural properties are hidden, manipulation is cheap and difficult to detect.

## Design Constraint

No democratic society will accept the adjudication of truth by another state or by its own government. Any viable framework must therefore make distortion observable rather than declare what is true. Sovereignty, civil liberties, pluralism, and reversibility are first-order constraints.

## Signal Model: What Is Exposed

The framework exposes **two and only two primary signals**, generated descriptively and comparatively:

1. **Relative Partisanship Signal**  
   A normalized, jurisdiction-specific measure of how politically partisan a piece of content is *relative to other content on the same topic*. This does not judge correctness or intent; it indicates whether language, framing, and comparisons place the content toward the center or extremes of the local political spectrum.

2. **Factual Language vs. Persuasive Expression Signal**  
   A measure of the extent to which content relies on verifiable factual claims and sourcing versus opinionated, emotive, rhetorical, or persuasive language. Content may be persuasive and lawful; this signal simply makes that posture visible.

Content that is not meaningfully political is classified as non-political and excluded from partisanship scoring.

## Human Calibration Layer

Signals are calibrated using trained civic raters serving in short, jury-duty–style tours. Raters are trained on a published rubric modeled on Ad Fontes–style comparative practices. They rate content *relative to other content on the same topic* across evidentiary posture, language type, and partisan framing. Raters self-identify ideological priors solely for stratification and variance analysis, not weighting. Deliberations are recorded for audit and appeal.

Human ratings are aggregated transparently, with disagreement and confidence intervals published as first-class outputs.

## Model Prediction Layer

Open-source models are trained on calibrated human datasets to predict the two signals at scale. Models publish error bounds, confidence scores, and known failure modes. Predictions are probabilistic and descriptive. No model output constitutes a determination of truth or falsity.

Each jurisdiction operates sovereign models trained on its own data. International comparison surfaces variance and deltas; it does not converge outputs into a single score.

## Community Annotation Layer

Community notes may attach post-hoc context, missing information, or dispute indicators. Notes do not compel ranking changes or content removal. When sustained annotations materially alter context, prior viewers receive notification and may re-inspect the content with added context.

## User Experience

Platforms may optionally expose integrity overlays and jurisdictional comparison lenses that allow users to see how the same topic appears under different observational regimes. These are lenses, not feed replacements. They operate on metadata and distributions, not outrage-optimized substitutions.

## Enforcement Boundary

Platforms are not penalized for ideological skew, unpopular speech, or disagreement with model outputs. Enforcement applies only to structural non-compliance: failure to surface required metadata, falsification or suppression of signals, obstruction of audits, or knowing tolerance of coordinated inauthentic amplification after notice.

Divergence from integrity signals is permitted and expected. Persistent divergence must be disclosed or explained, not eliminated.

## Strategic Effect

By exposing partisanship and persuasive posture at scale, the system makes hyper-partisan actors operating in bad faith visible without adjudicating truth. Manipulation becomes expensive, unstable, and detectable across jurisdictions. Citizens retain full agency over belief and expression while regaining the ability to see plainly through algorithmic distortion.

## Bottom Line

This framework governs visibility, not belief. It does not decide what is true. It ensures that citizens can see *how* information is framed, amplified, and presented—locally and across democratic partners—so democratic judgment remains possible under modern informational conditions.

---

## Defense & Boundary Clarifications (Non-Normative)

### Explicit Assumption of Capture and Bias

This framework assumes partial capture, ideological bias, and incentive misalignment as permanent features of large-scale information systems. It presumes neither neutrality nor benevolence from governments, corporations, platforms, experts, or civic institutions. Any component may be biased or strategically influenced at any time.

The framework remains functional because it does not seek convergence or correctness. It surfaces disagreement, variance, and divergence across independent observers. Visible bias is less dangerous than hidden bias.

### Civic, Distributed Signal Generation

Signal calibration is performed by regular citizens serving in short, rotating tours, not permanent authorities. Raters self-identify ideological priors for transparency and are rotated to prevent entrenchment. Their role is comparative and descriptive, not adjudicative.

### What This Framework Explicitly Does Not Do

This framework does not determine truth, require content removal, mandate ranking changes, impose viewpoint balance, compel belief, or require identity disclosure.

### Platform Discretion Affirmation

Platforms retain full discretion over ranking, recommendation, amplification, and monetization. Platforms may lawfully amplify content identified as highly partisan or primarily persuasive without penalty, provided integrity signals are accurately surfaced and auditable.

### Signal Interpretation Safeguard

Integrity signals describe structure and expression, not intent or correctness. High partisanship or persuasive posture does not imply misinformation or wrongdoing.

### Enforcement Limitation

Penalties apply only to structural non-compliance: refusal to surface metadata, falsification or suppression of signals, obstruction of audits, or knowing tolerance of coordinated inauthentic behavior after notice.

### Sovereignty and Non-Convergence Guarantee

Each jurisdiction operates its own models and datasets. No global score is authorized. International views surface variance, not consensus.

### Open Contestability

All rubrics, models, and aggregation methods are open source and may be forked or challenged. Competing interpretations are protected.

### Non-Default Exposure Rule

Jurisdictional comparison lenses shall never be enabled by default or mandated during elections or emergencies absent separate authorization.

### Reversibility and Exit

Participation is reversible. Withdrawal does not impair lawful speech or platform operation. The system must degrade gracefully without centralized failure modes.

---

## Sequencing and Phased Implementation

### Phase 0 — Standards and Voluntary Preparation

Signal definitions, rubrics, audit standards, and APIs are published as non-binding standards. Rater programs are piloted at small scale. Platforms may experiment internally without user exposure.

### Phase 1 — Visibility-Only Pilots

Platforms voluntarily integrate read-only APIs and may expose optional overlays. No ranking changes, moderation actions, disclosures, or enforcement apply.

### Phase 2 — Comparative Diagnostics

Optional jurisdictional and international lenses are introduced. Platforms may publish aggregate transparency reports. Divergence is permitted and expected.

### Phase 3 — Process Obligations

Platforms meeting reach thresholds must surface metadata consistently and maintain audit trails. Penalties attach only to refusal, falsification, or audit obstruction.

### Phase 4 — Continuity Protocols

In narrowly defined crises, temporary visibility measures may be authorized with time limits and oversight. Content removal and ranking mandates remain prohibited.

### Phase 5 — Review and Exit

All obligations sunset absent reauthorization. Platforms and jurisdictions may withdraw. The system must degrade gracefully.

### Sequencing Principle

Authority follows demonstrated restraint and public value. Early phases confer no power and cannot be abused. Later phases remain limited to visibility and process integrity.