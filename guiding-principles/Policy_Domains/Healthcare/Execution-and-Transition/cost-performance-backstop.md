---
id: cost-performance-backstop
title: Cost Performance Backstop — Escalation Framework and DoDA Healthcare Telemetry
sidebar_label: Cost Performance Backstop
sidebar_position: 7
slug: /healthcare/execution/cost-performance-backstop
tags:
  - healthcare
  - cost-control
  - doda
  - telemetry
  - subsidy
  - workforce
  - state-sequencing
  - capital-recycling
status: Draft
version: 0.1
author: Futures Project
dependencies:
  - department-of-data-and-accountability
  - healthcare-transition-phase-strategy
  - healthcare-transition-and-state-pilot-framework
  - insurance-architecture-sec
  - healthcare-infrastructure-layer
  - regional-health-center-network
  - HETA-revised-charter
  - public-capital-authority
description: >
  Defines the pre-specified escalation pathway that activates if the healthcare
  transition fails to reduce total consumer cost to the defined glide path,
  establishes the DoDA telemetry framework for healthcare workforce and cost
  metrics, and formalizes the state sequencing and capital recycling model
  that manages supply-demand balance across the rollout.
---

## Purpose and Scope

This brief defines two tightly coupled mechanisms:

1. The **Cost Performance Backstop** — a pre-specified, DoDA-triggered escalation
   pathway that activates if total consumer healthcare cost fails to meet the
   defined reduction glide path, providing a sequenced set of interventions
   ordered from least to most interventionist without nationalizing the system

2. The **DoDA Healthcare Telemetry Framework** — the specific metrics DoDA
   tracks for healthcare, with particular attention to physician and specialist
   supply-demand ratios as a gating condition on phase advancement and subsidy
   calibration

These mechanisms are inseparable. The backstop is only legitimate because DoDA
produces the measurement independently. The telemetry is only actionable because
the backstop defines what happens when thresholds are crossed.

This brief also formalizes the **state sequencing and capital recycling model**
that governs how the transition rolls out across cohorts to manage the
supply-demand balance and convert early-cohort savings into late-cohort capital.

---

## The Cost Problem This Brief Addresses

The healthcare transition framework is designed to reduce total consumer cost
through price transparency, administrative overhead elimination, SEC actuarial
stabilization, and recoupment-bound drug pricing. These savings are real but
back-loaded — they accrue as markets mature, providers adjust pricing, and
administrative complexity drains out of the system.

The honest scenario this brief addresses is:

> Transition is complete. Markets are functioning. SEC is universal. Prior
> authorization has been eliminated. Administrative overhead has dropped.
> But total consumer cost — primary care subscription plus SEC premium plus
> out-of-pocket for market-layer services — is roughly flat compared to
> pre-reform premiums. Not a disaster. Not the promise.

This scenario does not indicate system failure. It indicates that market
competition alone has not yet compressed prices sufficiently, that subsidy
calibration needs adjustment, or that supply constraints in specific regions
are limiting the competitive pressure the framework depends on.

Each cause has a different remedy. The backstop framework exists to diagnose
which cause is operative and apply the correct remedy in the correct sequence
without reaching prematurely for blunt instruments.

---

## The North Star Metric

DoDA tracks one primary cost metric for the healthcare system:

**Total population healthcare expenditure per capita, net of administrative
overhead, measured on a rolling 12-month basis, adjusted for demographics
and exogenous shocks, disaggregated by state and coverage tier.**

This metric is:

- Publicly reported on a quarterly basis
- Compared against a pre-specified national glide path established at
  authorization and updated by DoDA within predefined adjustment bands
- Disaggregated to show whether cost performance differs by state cohort,
  density tier, coverage type, and demographic group
- Compared against matched control states during the pilot phase using
  difference-in-differences methodology pre-specified by DoDA

Secondary cost metrics tracked alongside the north star:

- Total consumer cost per individual (subscription + premium + OOP)
- SEC claim frequency and severity by state and demographic
- Drug cost per covered life before and after recoupment step-down
- Administrative cost as a share of total healthcare spending
- Provider pricing distribution by service type and region

---

## DoDA Healthcare Telemetry Framework

DoDA tracks the following metric categories for healthcare. These are mandatory
reporting requirements for all entities receiving federal capital support,
SEC reimbursement, or regulatory backstop.

### 1. Workforce Supply-Demand Metrics

Physician and specialist supply is the binding constraint on the transition.
Markets cannot compress prices through competition if there are not enough
providers to compete. Subsidy increases cannot expand access if demand outpaces
supply. Phase advancement cannot proceed safely if primary care density is
below the threshold needed to absorb redirected demand.

DoDA tracks at the state and sub-state level:

**Primary care supply**
- Active primary care physicians per 10,000 residents, by county
- Panel capacity utilization rates (available vs. filled panels)
- New practice formation rates by phase and region
- Time-to-appointment for new patients at regional health centers and
  private DTC practices
- Physician attrition and retirement rates with 3-year forward projections

**Specialist supply**
- Active specialists by category per 100,000 residents, by state
- Wait times for specialist referrals from primary care
- Telehealth specialist utilization as a share of total specialist encounters
- Geographic distribution of specialist capacity relative to regional centers

**Workforce pipeline**
- Medical school enrollment and graduation trends
- Residency match rates by specialty and geographic preference
- PA and NP workforce growth and scope of practice utilization
- Foreign medical graduate licensing pipeline and clearance rates
- Loan repayment program participation rates for rural and underserved placement

**Supply-demand balance certification**
- DoDA certifies regional supply adequacy before HETA activates enforcement
  phases in any district
- Supply adequacy certification is a hard gate — enforcement does not activate
  in regions where primary care density is below the certified threshold
- Certification is updated quarterly and triggers automatic phase pause if
  supply deteriorates below threshold after enforcement has begun

### 2. Cost and Affordability Metrics

- Total consumer cost per individual by income quintile and state
- SEC premium trends vs. actuarial projections
- Market-layer price convergence by service type and region
- Provider price distribution relative to regional benchmarks
- Subsidy credit utilization rates by income tier and region
- Out-of-pocket expenditure distribution across covered population
- Discount wrap enrollment and utilization rates
- Drug price trajectories pre- and post-recoupment step-down

### 3. Access Metrics

- Time-to-care by service type, region, and density tier
- Regional health center utilization and capacity utilization
- Transport utilization rates and geographic coverage
- ED diversion rates (urgent care and primary care absorbing appropriate demand)
- Dental, vision, and mental health utilization rates by income quintile
- Telehealth utilization in frontier and remote tiers

### 4. Market Function Metrics

- Price transparency compliance rates by provider type and region
- Provider participation in unified payment rail
- Discount wrap competition (number of competing products per market)
- SEC product classification distribution (SEC-Comparable, SEC-Plus, SEC-Worse)
- Anti-gaming enforcement actions and outcomes
- Practice consolidation rates and anti-consolidation threshold compliance

### 5. Capital Recycling Metrics

- PCA instrument repayment rates by cohort and instrument type
- Regional health center break-even performance vs. projections
- Provider transition instrument utilization and outcomes
- Capital deployed vs. capital recycled by cohort and fiscal year
- Cost-per-covered-life for regional health center infrastructure by density tier

---

## The State Sequencing and Capital Recycling Model

### Why State-by-State Sequencing

The transition cannot and should not activate everywhere simultaneously.
Three constraints make sequencing mandatory:

**Supply constraint.** Physician and specialist shortages predate this framework.
Activating enforcement phases in states with inadequate primary care density
before supply builds would redirect demand without supply to absorb it,
producing wait times and access failures that would delegitimize the reform.

**Capital constraint.** The upfront cost of regional health center buildout,
PCA instrument deployment, and HETA field office establishment is substantial.
Spreading it thinly across all states simultaneously produces inadequate
infrastructure everywhere rather than adequate infrastructure in sequenced cohorts.

**Learning constraint.** Early cohorts produce the evidence that validates
the playbook for later cohorts. A simultaneous national rollout has no
control states, no comparative evidence, and no ability to course-correct
before problems are national in scale.

### Cohort Design

States are organized into sequenced cohorts of approximately five states each,
with new cohorts activating at annual decision gates per the State Pilot Framework.

**Cohort composition principles:**

- Geographic diversity within each cohort
- Mix of population density profiles (not all rural, not all urban)
- Baseline health burden diversity — healthier states paired with higher-burden
  states within the same cohort

**The pairing logic:** A state with lower baseline utilization, stronger primary
care density, and lower per-capita SEC claims reaches actuarial stability faster.
Its SEC claims come in below projection, recoupment pricing steps down on schedule,
and administrative overhead drains more quickly. The capital freed by that early
stability funds the buildout for higher-burden states in the same or subsequent
cohort. The healthier state also provides the proof-of-concept evidence that
reduces political risk for the higher-burden state's transition.

Pairings are determined by DoDA using pre-specified matching methodology
published before pairings are announced. The methodology uses propensity score
matching on:

- Baseline per-capita healthcare expenditure
- Primary care physician density
- Insurance mix (employer-sponsored, Medicaid, uninsured rates)
- Baseline health burden (chronic disease prevalence, premature mortality rates)
- Demographic profile and urbanicity distribution

Pairings are published with full methodology disclosure. They are not
negotiated politically. States that believe their pairing is incorrect may
request methodological review through DoDA's published dispute process.

### Capital Recycling Mechanism

The federal appropriation funds the first cohort fully. Subsequent cohorts
are funded through a combination of new appropriation and recycled capital
from earlier cohorts.

Recycling sources:

- PCA instrument repayments from regional health centers reaching financial
  sustainability above break-even
- SEC actuarial savings where claims come in below projection — the surplus
  is returned to the recycling pool, not absorbed into general revenue
- Administrative overhead savings from prior auth elimination and billing
  simplification, captured through mandatory reporting and returned
  proportionally to the capital pool
- Provider transition instrument repayments from practices that stabilized
  successfully and are repaying revenue-linked instruments

DoDA tracks capital recycling performance by cohort and certifies when
recycled capital is sufficient to reduce the new appropriation ask for the
next cohort. This certification is a core input to the annual Congressional
reauthorization request.

The Congressional appropriations ask over time therefore shrinks as a share
of total deployment cost — early cohorts are heavily federally funded, later
cohorts are increasingly self-funded through recycling. DoDA makes this
trajectory visible and auditable.

---

## The Cost Performance Backstop

### What Triggers the Backstop

DoDA certifies a **Cost Performance Shortfall** when total consumer healthcare
cost per capita fails to meet the pre-specified glide path for two consecutive
annual measurement periods in a state or cohort.

The glide path is defined at authorization and specifies:

- Expected year-over-year cost reduction percentage
- Acceptable variance bands
- Adjustment methodology for exogenous shocks (pandemic, natural disaster,
  demographic shift)

A shortfall certification is not a system failure declaration. It is a
technical finding that triggers a pre-specified diagnostic and escalation
sequence. It does not authorize HETA to act unilaterally. It initiates
a structured review that determines which escalation lever, if any, is
appropriate.

### Diagnostic First: Cause Identification

Before any escalation lever is activated, DoDA produces a **Shortfall
Diagnostic Report** determining whether the cost shortfall is:

**Type A — Geographic concentration**
Costs are not meeting the glide path in specific regions with thin markets,
inadequate provider density, or supply constraints. The rest of the state or
cohort is performing adequately.

**Type B — Market compression failure**
Prices have not compressed as expected despite adequate supply, suggesting
that competitive pressure is insufficient, anti-gaming enforcement has gaps,
or transparency mechanisms are not producing the expected behavioral change.

**Type C — Actuarial miss**
SEC claims are coming in above projection, either because the baseline
actuarial model was wrong or because utilization is higher than expected.
This is a modeling problem, not a market problem.

**Type D — Subsidy calibration gap**
Market prices have compressed as expected but total consumer cost remains
high because subsidy credits are not reaching eligible populations at
sufficient levels. The infrastructure is working; the dial hasn't been
turned far enough.

**Type E — Systemic**
Cost shortfall is broad, not concentrated, and not explained by supply,
market, actuarial, or subsidy factors. This is the most serious finding
and triggers the most interventionist escalation pathway.

Each type has a distinct remedy sequence. The diagnostic prevents applying
a Type D remedy (increase subsidies) to a Type A problem (thin supply),
which would inflate prices rather than reduce costs.

### Escalation Sequence by Cause Type

**Type A — Geographic: Supply-first response**

1. DoDA flags specific regions below supply adequacy threshold
2. HETA pauses enforcement phase advancement in affected regions
3. PCA deploys targeted capacity instruments — practice formation credits,
   regional health center expansion, diagnostic equipment instruments
4. Workforce pipeline signals activated for affected specialties and regions
5. Subsidy increases withheld in affected regions until supply adequacy
   certified — this is the critical supply-demand discipline rule
6. Reassess at next annual measurement window

**Type B — Market compression failure: Enforcement tightening**

1. HETA audits anti-gaming compliance in affected markets
2. Price transparency enforcement intensified
3. Anti-consolidation thresholds reviewed and tightened if concentration
   has increased
4. SEC product classification published with emphasis on SEC-Worse products
   to increase consumer switching pressure
5. If compression still fails after one measurement window, regional price
   reference bands activated — not administered prices, but published
   benchmarks with explicit public disclosure of providers priced above them
6. Administered price bands considered only if market compression has failed
   across two consecutive measurement windows despite enforcement tightening

**Type C — Actuarial miss: Model recalibration**

1. DoDA recalibrates SEC actuarial model with observed claims data
2. SEC premium adjustments issued within pre-authorized bands
3. If claims exceed model by more than defined threshold, HETA reviews
   SEC trigger event definitions for potential misclassification
4. Recoupment drug pricing review — if drug costs are driving actuarial miss,
   recoupment ceilings tightened for specific categories

**Type D — Subsidy calibration gap: Dial adjustment**

This is the cleanest escalation because the infrastructure is already in
place. SSI and UPI rails are operational. The subsidy credit amount is a
configuration parameter, not a new program.

1. DoDA certifies that supply is adequate in the affected region (prerequisite —
   subsidies do not increase where supply is inadequate)
2. DoDA certifies that market prices have compressed as expected (prerequisite —
   subsidies do not substitute for market compression that hasn't happened)
3. HETA requests Congressional authorization for subsidy credit adjustment
   within pre-authorized adjustment bands
4. If within bands: HETA adjusts subsidy credits through payment rail
   configuration — no new legislation required, no new bureaucracy
5. If beyond bands: formal reauthorization request to Congress with DoDA
   shortfall certification as the evidentiary basis

The supply adequacy prerequisite is the critical safeguard. Increasing
demand through subsidy without adequate supply produces price inflation,
not cost reduction. DoDA's supply adequacy certification is what prevents
this failure mode structurally rather than relying on discretionary judgment.

**Type E — Systemic: Full escalation review**

1. DoDA publishes Systemic Shortfall Report with full diagnostic methodology
2. HETA pauses phase advancement nationally
3. Congressional review triggered — not optional, mandatory under the
   backstop statute
4. Joint HETA-DoDA-PCA review of whether framework design gaps require
   statutory correction vs. execution adjustment
5. Congress determines whether to authorize additional escalation levers
   including broader price reference bands, accelerated regional health
   center deployment, or modified SEC design

Type E is the honest acknowledgment that if the system is failing broadly,
the answer is democratic deliberation rather than administrative escalation.
DoDA provides the evidence. Congress makes the call.

---

## The Supply-Demand Discipline Rule

This rule is stated explicitly because it is the most important safeguard
in the entire backstop framework and the easiest to violate under political
pressure.

**Subsidy credits do not increase in regions where primary care supply
is below the DoDA-certified adequacy threshold.**

The logic is straightforward. Subsidizing demand for a service that is
already supply-constrained does not lower costs. It raises prices. The
providers who exist capture the subsidy as margin rather than patients
capturing it as savings. This is the documented failure mode of demand-side
healthcare subsidies historically.

The sequencing rule therefore is always: supply first, subsidy second.

Where supply is inadequate, the remedy is capacity instruments through PCA
and workforce pipeline activation — not subsidy increases. Subsidy increases
follow supply adequacy certification, not precede it.

DoDA's quarterly supply adequacy certification is what makes this rule
operationally enforceable rather than an aspiration.

---

## Workforce Pipeline Integration

Physician and specialist shortages require a longer lead time than any
other framework component. A medical school enrollment increase today
produces a practicing physician in 7-11 years. The framework cannot
wait for shortfalls to appear before activating the pipeline.

DoDA therefore tracks **forward-looking supply adequacy** — not just
current density but projected density under current pipeline conditions
3, 5, and 10 years out. This projection is updated annually and published.

When projected supply adequacy falls below threshold in a region or
specialty before it is currently below threshold, the following activates:

- Loan repayment programs for the affected specialty and region
- Residency slot expansion funding through PCA where hospital capacity
  constrains residency availability
- Scope of practice review for PAs and NPs in affected specialties —
  the framework does not mandate scope expansion but flags where it
  would relieve projected shortfalls
- International medical graduate licensing streamlining in affected
  specialties where pipeline is globally undersupplied
- Telehealth specialist coverage as a bridge in affected regions while
  pipeline fills

These are not emergency measures. They are forward-deployed responses
to DoDA's projected supply signals, activated before shortfalls are acute.

---

## What This Framework Is Not

This framework is not:

- A price control system — administered prices are the last resort in
  Type B escalation, not the default response to any cost shortfall
- A nationalization pathway — every escalation lever operates within
  the existing market structure, adjusting parameters rather than
  replacing markets
- A blank check subsidy program — supply adequacy certification is a
  hard prerequisite for subsidy increases, not a soft guideline
- A congressional bypass — escalation beyond pre-authorized adjustment
  bands requires Congressional action, not administrative discretion
- A system failure declaration — a DoDA shortfall certification means
  "the dial needs adjusting," not "the reform has failed"

---

## Bottom Line

The healthcare transition will produce meaningful cost reduction for most
Americans in most regions. But "most" is not "all," and the timing is
uneven. This framework exists for the regions and populations where the
transition takes longer than projected.

The answer to "what if costs don't fall fast enough" is not panic,
nationalization, or abandonment of the market structure. It is a
pre-specified, evidence-triggered, sequenced escalation through
instruments that are already in place — turning the subsidy dial where
supply is adequate, building supply where it is not, tightening enforcement
where markets have failed to compete, and returning to Congress where
the problem is genuinely systemic.

DoDA makes the diagnosis. HETA adjusts the instrument. PCA builds the
capacity. Congress decides if the framework needs structural revision.

The supply-demand discipline rule is the load-bearing safeguard.
Everything else follows from it.
