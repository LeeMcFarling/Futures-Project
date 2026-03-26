---
id: digital-nutrition-label
title: Digital Nutrition Labeling & Epistemic Integrity System
sidebar_label: Digital Nutrition Label
sidebar_position: 4
slug: /technology/digital-nutrition-label
domain: Technology_and_Data
subdomain: Information Integrity & Platform Governance
policy_type: Instrumentation Framework
status: Draft
version: 0.3
author: Futures Project
dependencies:
  - ssi-self-sovereign-identity-framework
  - department-of-data-and-accountability
  - execution-corps-spec
  - Platform_Regulation
related_initiatives:
  - AI Governance
  - Algorithmic Attention Initiative
  - Anti-Capture Competition Framework
  - Institutional Modernization
  - UPI Payment Rail
non_goals:
  - content removal
  - viewpoint moderation
  - algorithmic censorship
  - identity disclosure mandates
  - requiring allied nations to adopt shared identity infrastructure
tags:
  - information-integrity
  - platform-governance
  - epistemic-infrastructure
  - transparency
  - civic-participation
  - ad-fontes
  - doda
  - execution-corps
last_updated: 2026-03-26
---

# Digital Nutrition Labeling & Epistemic Integrity System

## Summary

This brief proposes a standardized, platform-integrated **Information Nutrition Label** for digital content.

The system does **not** determine whether content is right or wrong, true or false, or how left or right it is. No government agency makes these judgments and no central authority controls classification.

Credibility signals are produced through a transparent, auditable process combining:

- Civic panels selected by **random draw** from verified citizen pools in participating democracies
- **Federated cross-national scoring** where independent panels in different countries rate the same content, with results compared rather than merged
- **Ad fontes regression** as the shared analytical standard — rating distance from primary sources rather than ideological valence
- A **three-layer training architecture** that enforces calibration statistically rather than through mandatory certification
- Open-source machine learning models subject to public scrutiny, used for provisional scoring during the breaking news window
- Institutional dimension checks against known reference sources (wire services, official statements, cross-outlet corroboration)

The role of the state is limited to setting interoperability standards and transparency requirements. All evaluative judgments are aggregated, averaged, and published as metadata attached to content at scale.

The objective is to make information quality legible at the point of consumption — similar to how nutrition labels inform food choices — without suppressing speech or delegating truth to the government.

---

## Problem Statement

Digital information systems suffer from three structural failures:

1. Opacity around sourcing, evidence, and confidence
2. Asymmetric amplification of low-confidence or extreme claims
3. Large-scale abuse via automation and coordinated inauthentic behavior

Existing moderation approaches are opaque, discretionary, and politically fragile. Any system that produces credibility scores on content — however well-designed its governance — risks being characterized as government speech suppression by one side and corporate capture by the other.

This framework addresses both failure modes through structural design: random civic selection removes the "who picks the pickers" problem, and federated cross-national scoring means no single government controls the composition or outcome of the rating process.

---

## Governance Design

### Random Civic Selection

Panelists are selected by **random draw** from verified citizen pools within each participating democracy. Each country runs its own selection process under its own civic participation norms and identity infrastructure. No shared identity system is required across nations.

In the United States, the SSI Self-Sovereign Identity Framework provides the verification layer for the citizen pool. The selection pipeline is fully open source and operates as follows:

1. An open source API queries the SSI infrastructure for the eligible pool — verified adult citizens who have not served in the current calendar year. The API returns anonymized tokens only. No personally identifiable information is transferred.
2. A public numpy-based random draw runs against the eligible pool. The random seed is publicly committed via cryptographic hash *before* the draw occurs, so the selection cannot be manipulated after the pool composition is known. Anyone can verify the draw post-hoc by replaying it with the published seed.
3. Selected tokens receive civic duty notification through their SSI wallet. The panel body knows only the token; it does not know who was selected.
4. On session completion, the panelist's SSI credential is updated to reflect service this year, automatically excluding them from the next draw. No record is retained of what they rated or how they scored it.

The eligible pool size is published in real time. Anomalous pool shrinkage — for example from mass SSI revocations — is immediately visible and auditable.

This model mirrors jury duty: participation is civic, time-bounded, and randomly assigned. No agency, committee, or editorial board selects who rates content. The randomness is the governance.

Panel size per draw is set in the range of 150–300 participants per national panel per content batch — sufficient for statistical validity while remaining a proportionate civic ask.

### Federated Cross-National Scoring

Rather than requiring allied nations to adopt shared infrastructure, each country convenes independent panels that rate the same content against the same **ad fontes regression standard**. Outputs are compared across panels rather than pooled into a single pipeline.

This design:

- Preserves national sovereignty — each country's panels operate under domestic law and civic norms
- Eliminates single-point capture — no one country's government controls the aggregate signal
- Makes convergence meaningful — when panels across multiple democracies independently reach similar scores, that agreement is a stronger signal than any single panel's verdict
- Makes divergence informative — high variance across panels flags genuine cross-cultural interpretive disagreement rather than hiding it

Panels operate on a **rolling cadence**, similar to jury duty rotations, ensuring continuous coverage without requiring permanent institutional staff.

### Ad Fontes Regression Standard

The shared analytical standard is **ad fontes** — rating content by its distance from primary sources and the integrity of its evidence chain. This is a measurable claim about provenance, not a judgment about ideological conclusions.

Panelists assess four dimensions:

| Dimension | What it measures |
|---|---|
| Source proximity | How close is the claim to a verifiable primary source? |
| Evidence chain | Is the path from claim to evidence traceable and intact? |
| Claim specificity | Are assertions concrete and falsifiable? |
| Context completeness | Is relevant context included or omitted? |

These dimensions are rated independently. The aggregate score is a mean across dimensions and across national panels.

Where possible, panelists rate content **source-blind** — without seeing the outlet name or author, only the text and cited sources. This ensures raters are evaluating the evidence chain, not the brand.

---

## Panel Training Architecture

Online rating without calibration produces noise rather than signal. Raters applying their own intuitive definitions of "credibility" rather than the ad fontes standard introduces inconsistency that degrades the aggregate score and creates a gaming surface for coordinated influence operations.

The system uses a three-layer training architecture that enforces calibration statistically rather than through mandatory certification. The total time ask on a panelist is approximately 20 minutes of onboarding plus 45 minutes per rating session, two to four times per year — comparable to jury duty.

### Layer 1 — Async onboarding module

A self-paced module of approximately 20 minutes completed once before a panelist's first session. Its purpose is shared vocabulary, not certification. It explains what ad fontes means, what each dimension measures, and walks through worked examples of high, medium, and low scores across content types. There is no pass/fail gate. The module is open source and its content is version-controlled — changes require a public changelog entry certified by the international governance body described below.

### Layer 2 — Anchor rating calibration

The load-bearing layer. Every rating session opens with two to three **gold standard items** drawn from the federated anchor library. The panelist does not know these are calibration items. Scores on anchors are compared to the established distribution. Panelists whose anchor scores fall outside acceptable bands are statistically down-weighted before their session scores enter the aggregate.

This means calibration is enforced by outcome rather than trust. A panelist who skipped the module, rated carelessly, or attempted to game the system all present the same way: as anchor outliers. The layer degrades gracefully — if population-level calibration slips, it appears in inter-rater agreement statistics that are published continuously, triggering a review of the module or interface rather than a system crisis.

### Layer 3 — Embedded calibration questions

Short contextual prompts embedded in the rating interface at the moment of scoring. Not a separate quiz — a dimension-specific reminder at the point of decision. For example: "Source proximity measures how directly this claim links to a verifiable primary document. Does this claim cite a primary source, a secondary report, or an unnamed source?" This reinforces module vocabulary without adding friction and prevents raters from drifting toward intuitive credibility judgments mid-session.

---

## Federated Gold Standard Library

The anchor calibration layer depends on a library of gold standard items — content that panels have scored with high inter-rater agreement across multiple cycles. This library **cannot sit with any single national body**, including the US Department of Data and Accountability. Unilateral control of the anchor library is equivalent to editorial control of the calibration standard, which recreates the capture risk the whole system is designed to prevent.

### Admission criteria

An item graduates to the gold standard library only when it meets high inter-rater agreement *across* national panels, not merely within one. Content that American panels consistently score one way but German or Japanese panels score differently does not qualify — it reflects genuine cross-national interpretive disagreement and is filtered out. Only items where the evidentiary assessment is stable regardless of civic context become calibration anchors. The library is therefore self-cleansing politically: anything with real cross-national interpretive variance never enters.

### Governance structure

The library is governed by a small **international calibration body** with representation from each participating democracy. Representation rotates on staggered terms misaligned with electoral cycles in any single country. No single nation holds a blocking vote on item admission or retirement. The body's mandate is strictly methodological — it cannot influence panel ratings, adjust scores, or modify the draw pipeline.

Each participating nation contributes candidate items from its own panel history. The international body reviews cross-national agreement statistics and makes admission decisions according to published thresholds. All admission and retirement decisions are logged publicly.

### Maintenance and recalibration

Items are retired from the library when inter-rater agreement degrades below a defined threshold across panels — typically indicating that the content domain has become politically contested in ways that weren't present at admission. The recalibration schedule is public. DoDA and its international counterparts publish inter-rater agreement statistics per session as a continuous system health signal.

### DoDA's role

Within the United States, DoDA owns the domestic interface to the federated library. It validates that the onboarding module has not been modified without a changelog entry, certifies draw integrity, sets domestic anchor down-weighting thresholds, and publishes inter-rater agreement statistics. It does not have unilateral authority over the library itself, does not see individual panelist scores, and cannot modify the draw pipeline without a public governance process.

---

## Institutional Dependencies

### Panel selection body

A small standing technical body — on the order of a dozen engineers and a governance board — owns the open source SSI query API, the numpy draw pipeline and seed commitment protocol, the wallet notification interface, the exclusion list (served-this-year flag), the rating interface and ad fontes dimension tooling, and score aggregation and publication to DoDA. It owns no editorial function. It cannot see who was selected, cannot influence how panelists rate content, and cannot adjust scores post-aggregation. Algorithm changes require a public notice period and sign-off from the international calibration body.

Leadership terms are staggered and misaligned with electoral cycles. No administration appoints a majority of the board in a single term.

### Department of Data and Accountability (DoDA)

DoDA certifies domestic draw integrity, maintains the US interface to the federated anchor library, publishes inter-rater agreement statistics, and certifies that pilot adoption thresholds have been met to trigger phase expansion. It does not own the panel body, the rating interface, or the gold standard library. Its authority is measurement and certification only.

### Execution Corps

The initial deployment of SSI-integrated civic panel infrastructure is a mission-bound Execution Corps problem: cross-agency, time-bounded, with a clear handoff point to the standing panel body. An Execution Corps deployment coordinates SSI onboarding for the citizen pool, builds the rating interface, and establishes the wallet notification channel before sunsetting. The standing panel body then operates the infrastructure independently.

### Compensation

Panelists receive nominal compensation for session completion, delivered via UPI to their SSI wallet. The amount is set at a level sufficient to signal the civic ask is valued but insufficient to attract gaming. This also exercises the UPI and SSI infrastructure the system depends on, providing a regular operational stress test of both rails.

---

## User Interface

### Default Inline Label

The inline label is deliberately minimal. It displays:

- Content type (news, analysis, opinion, satire)
- Domain tag (economic policy, geopolitical, health, etc.)
- Source quality indicator (primary sources cited / secondary / anonymous / circular)
- A single flag button showing the **cross-national mean score** and, where applicable, a variance flag

The label does not display individual country scores, dimension breakdowns, or institutional assessments inline. All detail lives behind the click.

> **Design principle:** The inline label should feel like infrastructure, not editorial judgment. A calm, consistent visual register across all content states — including breaking news — is part of what makes the system trustworthy over time.

![Inline label — default state](./assets/label-default.png)

### Drill-Down Panel

When a user clicks the flag button, a panel expands showing:

**Cross-national mean score** with panel size and cadence metadata.

**Democracy continuum** — national panel scores plotted as dots on a confidence axis. Dot clustering indicates cross-national agreement; spread indicates interpretive divergence. Users hover to see which country each dot represents.

**Ad fontes dimensions** — bar breakdown of source proximity, evidence chain, claim specificity, and context completeness.

**Institutional dimensions** — automated checks against reference sources:

- Wire service match (Reuters / AP)
- Official government or institutional statement
- Cross-outlet corroboration count
- Prior domain credibility of the outlet
- Academic citation index (where applicable)

**Provenance metadata** — panel size, algorithm version, last updated, score type (provisional or panel-confirmed).

![Drill-down panel — expanded state](./assets/label-drilldown.png)

---

## Provisional Scoring and the Breaking News Window

### The Lag Problem

The system's most exploitable vulnerability is the gap between when breaking news spreads and when panels can evaluate it. A coordinated influence operation does not need to win the long game — it only needs the first 6–12 hours, which is exactly when breaking news travels fastest and audience priors get set.

### Provisional Label Tier

During the breaking news window, content receives a **provisional label** rather than a panel-confirmed score. The provisional label:

- Appears immediately via automated pipeline
- Uses ML models trained on historical panel data to generate a baseline score
- Displays institutional dimension checks (wire match, corroboration count, velocity signal) that do not require panel deliberation
- Shows an explicit "unscored — breaking / panel opens in ~Xh" indicator rather than suppressing the label entirely

The provisional label uses the same visual grammar as the confirmed label. It does not use alarm-style design. The difference between provisional and confirmed is surfaced in the metadata, not in the emotional register of the interface.

> **Rationale:** A provisional score on a single-source breaking claim will typically be low — not because the system has judged the claim false, but because the evidentiary state is genuinely thin at that moment. That is honest and useful information. It is also difficult to attack as censorship because it describes what is known, not what to believe.

![Provisional label — breaking news state](./assets/label-provisional.png)

### Score Replacement

Once a panel quorum is reached across four or more participating democracies, the ML provisional score is replaced by the panel-confirmed score. The metadata layer records both scores and the transition timestamp for auditability.

---

## Algorithm Cadence

ML models and scoring pipelines are updated on a defined public cadence. Each label displays the algorithm version used to generate the score. Changes to the algorithm — including threshold adjustments for variance flags — require a documented governance process involving the international calibration body and are published in advance.

> **Capture prevention:** The variance flag threshold is defined in the public algorithm specification. Changing it requires governance review from the international body, not unilateral action by any national institution. This closes the hole where the threshold itself becomes a de facto editorial lever.

---

## Governance and Safeguards

- No centralized truth authority
- No integration into ranking algorithms by default
- Random civic selection via open source pipeline removes institutional capture at the panel level
- Federated national panels remove single-government capture at the aggregate level
- Federated gold standard library removes single-nation capture at the calibration level
- Public algorithm specification with versioned changelog
- International calibration body with staggered rotating representation
- DoDA certifies domestic procedural integrity only — no editorial authority
- Independent audits and appeals process
- Per-platform decentralized identifiers with rotation
- Variance flag surfaces disagreement rather than suppressing it
- Source-blind rating interface where technically feasible

---

## Phase Strategy

**Phase 1 — Voluntary pilots**
Execution Corps deploys SSI civic panel infrastructure in 2–3 democracies. ML provisional scoring active. Institutional dimension checks automated. Platforms publish experimental label dashboards on opt-in basis. International calibration body formed with founding member nations.

**Phase 2 — Cross-national panel federation**
Rolling panel cadence established across 4–6 participating democracies. Federated gold standard library operational with cross-national admission criteria enforced. Ad fontes regression standard finalized and published. Variance flag thresholds set through international governance process. UPI compensation channel active.

**Phase 3 — Cross-platform standardization**
Interoperability standards adopted. Label metadata portable across platforms. SSI-backed amplification integrity for high-reach civic content. Gold standard library open to additional allied democracies under admission criteria.

---

## Non-Goals

This framework does not:

- Remove or suppress content
- Require allied nations to adopt shared identity infrastructure
- Mandate real-name participation
- Integrate label scores into algorithmic ranking by default
- Create a centralized truth authority
- Give any single nation editorial control over calibration standards
- Replace courts, defamation law, or platform moderation policies

---

## Relationship to Other Initiatives

The Digital Nutrition Label depends on the **SSI Self-Sovereign Identity Framework** for domestic civic panel selection — SSI provides the cryptographic proof of unique human participation without identity disclosure, and delivers panelist compensation via the **UPI Payment Rail**.

It depends on the **Department of Data and Accountability** for domestic draw integrity certification, inter-rater agreement publication, and pilot phase expansion triggers.

It depends on a **mission-bound Execution Corps** deployment for initial infrastructure build and SSI onboarding before handoff to the standing panel body.

It complements the **Algorithmic Attention Initiative** — the aggregate recommendation environment signals the Attention Initiative needs slot naturally into DoDA's telemetry mandate without requiring a separate institution.

It operates independently of the **Anti-Capture Competition Framework** but shares its core concern: preventing any single actor from becoming the de facto governor of informational legitimacy.
