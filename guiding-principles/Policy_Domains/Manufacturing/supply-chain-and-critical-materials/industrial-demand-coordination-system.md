---
id: industrial-demand-coordination-system
title: Industrial Demand Coordination & Supplier Activation System
sidebar_label: Demand Coordination
sidebar_position: 10
slug: /economic-prosperity/manufacturing/demand-coordination
domain: Economic_Prosperity
subdomain: Manufacturing
policy_type: Coordination Infrastructure
status: Draft
version: 0.5
author: Futures Project
dependencies:
  - alliance-industrial-target-map
  - industrial-corridor-viability-criteria
  - manufacturing-pca-instruments-framework
  - factory-jv-deployment-model
  - supplier-credit-facilities
  - domestic-refining-processing-corridors
  - industrial-logistics-spine
  - regional-manufacturing-pilot-playbooks
  - department-of-data-and-accountability
  - execution-corps-spec
  - national-apprenticeship-manufacturing-pipeline
tags:
  - manufacturing
  - supply-chain
  - coordination
  - industrial-policy
  - supplier-ecosystem
  - two-sided-market
  - materials-sovereignty
last_updated: 2026-03-30
---

## Purpose

This document defines the coordination infrastructure that bridges the gap
between raw material inputs and finished factory inputs — the intermediate
layer of castings, forgings, machined components, tool and die work,
subassemblies, and industrial processing that every manufacturer depends on
but that no single manufacturer can build alone.

This is a two-sided coordination problem. Manufacturers who want to source
domestically cannot find qualified domestic suppliers. Potential suppliers
cannot justify capacity investment without visible, credible demand from
manufacturers. Both sides are waiting for the other to move first. The
equilibrium is continued import dependency and a domestic industrial base
that remains permanently thin below the anchor manufacturer layer.

The solution is not primarily capital — though capital is part of it. It is
coordination infrastructure: a system that makes the supply side legible to
manufacturers, makes the demand side legible to suppliers, connects both to
shared workforce pipelines and training systems, and gives existing small and
mid-sized industrial shops access to the same activation stack available to
anchor manufacturers.

The objective is to make the domestic supplier ecosystem discoverable,
investable, and scalable — and to do it as a coordinated system rather than
leaving each manufacturer to solve the problem independently.

The system does not directly allocate capital or mandate supplier formation.
It structures the conditions under which supplier investment becomes legible,
coordinated, and economically rational. Capital deployment through PCA
instruments follows from this layer rather than leading it.

---

## Problem Statement

The primary constraint on domestic manufacturing expansion is not always
capital or finished-goods demand. For a large class of manufacturers who
want to produce in the United States, the binding constraint is the absence
of a visible, qualified, domestic supplier base at the industrial input layer.

This layer includes:

- castings (sand, die, investment, permanent mold)
- forgings (open die, closed die, ring rolling)
- machined components (CNC turning, milling, grinding, EDM)
- tool and die (stamping dies, molds, fixtures, jigs)
- sheet metal fabrication
- heat treatment and surface finishing
- precision welding and joining
- subassembly and kitting

These are not exotic capabilities. They are the foundational manufacturing
processes that every sector — automotive, aerospace, defense, energy hardware,
robotics, medical devices — depends on for physical production.

The failure has multiple causes that compound each other:

**Fragmentation.** Demand for these inputs is spread across hundreds of
manufacturers, each with proprietary specifications, different quality systems,
and non-standardized procurement processes. No individual demand signal is
large enough to anchor supplier investment.

**Invisibility.** Existing domestic suppliers — and there are more than most
manufacturers realize — are not systematically discoverable. There is no
national registry of domestic casting shops by alloy and process capability,
no database of qualified tool and die houses by tolerance and material, no
searchable map of forging capacity by geometry and lot size. Manufacturers
default to known import channels because finding domestic alternatives
requires manual search they cannot cost-justify.

**Temporal misalignment.** Even when demand exists and suppliers are
interested, ramp timelines don't align. A manufacturer committing to a new
product line needs supplier qualification 18 months before production. A
supplier building new capacity needs demand commitment 24 months before
investment. Neither can move without the other moving first.

**Training pipeline gaps.** The skills required for precision machining,
tool and die, and specialty casting are deep and take years to develop.
The workforce pipeline for these trades has been thin for decades. Even
suppliers who want to scale are constrained by their inability to find and
train qualified workers at the pace investment would require.

**Capital access asymmetry.** Small and mid-sized industrial shops — the
backbone of the intermediate supplier layer — have limited access to the
capital markets that serve anchor manufacturers. A 40-person machining shop
that wants to add capacity to serve a new domestic program cannot access
institutional capital efficiently, and the investment is too small to attract
the attention it deserves relative to its strategic importance.

The cumulative effect: manufacturers import inputs they could source
domestically if the ecosystem were legible and investable. Domestic suppliers
operate below potential because demand is invisible and fragmented. The
intermediate layer stays thin, and every new factory that opens in the United
States begins by importing a large share of its inputs.

---

## Strategic Frame

Industrial supply chains fail when intermediate demand is not legible or
reliable and when intermediate supply is not discoverable or investable.

This system addresses both sides simultaneously — which is the only way a
two-sided coordination problem gets solved. Fixing demand visibility without
fixing supply discoverability produces manufacturers who can see that domestic
supply doesn't exist. Fixing supply discoverability without fixing demand
aggregation produces suppliers who can be found but still can't justify
investment.

The system converts demand and supply into three progressively stronger
forms of coordination:

**Visibility** — manufacturers can see what domestic and allied supply
exists; suppliers can see what demand is coming and from where.

**Aggregation** — fragmented demand is pooled into investable signals;
fragmented supplier capabilities are organized into navigable categories.

**Commitment** — demand becomes partially committed through conditional
offtake structures; supply becomes partially committed through qualified
supplier registrations and capacity investment.

This creates a pipeline in both directions simultaneously:

```
Manufacturers:  Demand → Signal → Aggregation → Commitment → Sourcing
Suppliers:      Capability → Registration → Visibility → Demand → Investment
```

Where the two pipelines connect is where the coordination failure dissolves.

---

## System Architecture

The system has six integrated components. They are designed to operate
simultaneously, not sequentially.

---

### Component 1: Industrial Supplier Registry

The foundational infrastructure. A national, publicly accessible, continuously
maintained registry of domestic and IDP-allied industrial suppliers organized
by process capability, material, geometry, tolerance, certification status,
capacity, and geographic location.

**What it covers:**

Every major industrial input process category is represented:

- Casting: alloy, process type (sand, die, investment, permanent mold),
  weight range, dimensional tolerance, certification (NADCAP, AS9100, IATF,
  ITAR if applicable)
- Forging: material, process (open die, closed die, ring), weight and size
  range, press capacity, heat treatment in-house capability
- Machining: CNC turning, milling, grinding, EDM, multi-axis capability,
  material certifications, lot size range, lead time performance
- Tool and die: stamping dies, injection molds, die casting tooling,
  fixturing, material hardness capability, cavity complexity
- Sheet metal: gauge range, material, press tonnage, forming complexity,
  finishing in-house capability
- Heat treatment and surface finishing: process types, specifications met,
  certifications
- Precision welding: process (TIG, MIG, electron beam, friction stir),
  material certifications, structural qualification
- Subassembly and kitting: integration capability, ESD compliance,
  cleanroom capability where applicable

**Geographic tiering:**

Suppliers are tagged by location and corridor assignment, enabling
manufacturers to identify suppliers within viable logistics distance for
their production location. Corridor-specific supplier density maps are
published as part of DoDA corridor readiness dashboards.

**Allied supplier inclusion:**

IDP-allied suppliers from partner countries are included in the registry
under a tiered structure:

- Tier 1 (Domestic): US-based suppliers, preferred default for sourcing
- Tier 2 (IDP-Allied): Suppliers from IDP partner countries (Japan, South
  Korea, Australia, European partners) with established US presence or
  active US-market participation, treated as qualified equivalents for
  sourcing decisions
- Tier 3 (Case-by-case): Other international suppliers assessed individually
  for strategic sensitivity

Allied supplier inclusion directly supports IDP supply chain interoperability
standards and enables manufacturers to build resilient sourcing strategies
that span the alliance without defaulting to adversary-controlled supply
chains.

**Maintenance and verification:**

Registry entries are self-reported by suppliers and verified through a
lightweight certification process: documented quality system, site visit or
remote audit for new entrants, and annual capability update requirement.
DoDA maintains registry integrity standards. The Manufacturing Extension
Partnership (MEP) network serves as the primary onboarding and verification
partner, leveraging existing regional relationships with small and mid-sized
industrial shops.

The registry is free to access for manufacturers. Supplier registration is
free. The public goods character of the infrastructure justifies public
operation — a private registry would create access barriers and data
ownership problems that undermine the coordination objective.

---

### Component 2: Demand Signal Ingestion and Aggregation

DoDA continuously aggregates forward-looking demand for industrial inputs
from multiple sources and converts it into standardized, pooled demand
signals that suppliers can act against.

**Demand sources:**

- Anchor manufacturers in active Factory JV programs
- Manufacturers participating in regional pilot corridors
- Federal procurement pipelines (DoD, GSA, and agency-specific programs)
- Infrastructure and energy deployment programs (grid hardware, transit,
  water systems) that generate large, predictable intermediate input demand
- Allied firm procurement where domestically sourced inputs are preferred
  under IDP supply chain interoperability standards

**Standardization layer:**

Raw demand is normalized into standardized industrial categories using
common process and material classifications. Proprietary specifications are
translated into process-class equivalents that allow demand pooling without
exposing manufacturer IP. The standardization methodology is published and
maintained by DoDA with industry input.

The objective is fungible demand pools — demand that can be evaluated by
any qualified supplier regardless of which specific manufacturer originated it.

**Aggregated demand bundles:**

Standardized demand is aggregated across buyers into:

- Volume-banded pools by process category and material
- Corridor-specific demand clusters showing geographic concentration
- Time-phased demand curves showing when volumes ramp, peak, and stabilize
- Sector-aligned input packages showing which industrial inputs are needed
  together for specific manufacturing programs

Example output:
> "Great Lakes corridor: precision aluminum die casting demand, automotive
> and EV powertrain applications, IATF-certified, 2–15 kg part weight,
> projected 4.2M units/year at steady state, ramp beginning Q3 2027,
> distributed across 6 anchor manufacturers."

This is the signal a casting shop needs to evaluate whether a capacity
investment makes sense. It would take that shop months of individual
manufacturer outreach to assemble this picture independently. The system
produces it continuously and publishes it publicly.

---

### Component 3: Conditional Offtake Commitments

Where demand visibility and aggregation are insufficient to unlock supplier
investment — typically for new capacity builds or significant scale-ups in
categories with thin existing domestic supply — demand bundles are converted
into conditional commitments.

**Structure:**

Conditional commitments are not unconditional purchase guarantees. They are
structured agreements that:

- Commit participating manufacturers to sourcing preference from qualifying
  domestic suppliers for a defined volume over a defined period, conditional
  on the supplier meeting qualification and performance standards
- Establish minimum utilization floors that activate once supplier capacity
  is online and certified
- Set price bands linked to published input cost indices, preventing
  commitment exploitation in either direction
- Include step-down provisions as domestic supply matures and market pricing
  becomes reliable

**Authorization:**

Conditional commitments require DoDA verification that the gap being
addressed meets the threshold criteria: the input category is documented as
domestically deficient, the commitment volume is sufficient to anchor
investment, and the participating manufacturers represent genuine forward
demand rather than speculative volume.

PCA coordinates offtake commitment participation from federal procurement
programs where applicable, consistent with the Alliance Offtake Compact
Participation instrument. Federal procurement is a particularly powerful
commitment anchor for defense-adjacent input categories where the
government is already a significant buyer.

**Anti-gaming design:**

Commitments are structured to prevent suppliers from building capacity
against commitments and then failing to compete on quality or cost once
capacity is online. Commitment activation requires supplier performance
certification by DoDA. Manufacturers cannot exit commitments for convenience;
they can exit for documented supplier underperformance against published
standards. This protects supplier investment without insulating suppliers
from competitive pressure.

Commitments automatically sunset if supplier capacity does not reach defined
milestones within specified timeframes. This prevents indefinite reservation
of demand without corresponding capacity delivery and ensures that demand
signals remain dynamic rather than locked.

---

### Component 4: Supplier Activation Pathways

Suppliers enter the coordination system through three pathways depending on
their starting position. Each pathway connects to the PCA instrument stack
and the workforce pipeline system.

**Pathway A — Domestic Expansion**

Existing domestic shops scaling capacity to serve newly visible demand.
This is the fastest and most capital-efficient pathway and should be the
primary mechanism for filling identified gaps where qualified domestic
suppliers already exist but are operating below potential scale.

Support stack:
- Registry visibility and demand signal access (immediate)
- PCA tooling and equipment finance (primary instrument for capacity
  addition in existing facilities)
- Supplier credit facilities for working capital during ramp
- MEP technical assistance for process optimization and quality system
  upgrades required for new customer qualification
- Workforce pipeline connections for additional skilled trades hiring

**Pathway B — Allied Entry**

IDP-allied suppliers establishing US domestic presence — whether through
greenfield facility, joint venture with US partner, or acquisition of
existing domestic shop — to serve the domestic market and meet IDP supply
chain proximity requirements.

Allied entry is actively encouraged in categories where domestic supply
gaps are large and building domestic capacity from scratch would take too
long. An allied firm establishing a US facility transfers process knowledge,
workforce training capability, and quality systems while creating domestic
employment and reducing import dependency.

Support stack:
- Expedited registry onboarding for allied firms with established
  IDP-partner quality certifications (AS9100, JISQ, KS equivalents)
- PCA tooling finance for US facility establishment
- Corridor activation stack access on equivalent terms to domestic suppliers
- Workforce training partnership with MEP and apprenticeship pipeline to
  ensure knowledge transfer to domestic workforce — not just facility
  presence but genuine capability building

Allied entry does not substitute for domestic capability development. It
accelerates availability in the near term while domestic pathway capacity
builds.

Allied supplier participation is structured as a capacity bridge rather than
a terminal state. Corridor-level targets for domestic capability substitution
are established at the time of allied entry. DoDA tracks domestic-versus-allied
sourcing ratios by category and corridor, with explicit targets for domestic
share growth over time.

**Pathway C — New Formation**

New entrants building capacity in categories where neither domestic nor
allied supply exists at adequate scale. The highest-risk and longest-lead
pathway, reserved for categories where the gap is large, the strategic
importance is high, and no existing supplier can reasonably fill it.

Support stack:
- Demand commitments (typically required before investment is viable)
- PCA first-loss tranches alongside private capital
- PCA tooling and equipment finance
- Factory JV structure where the scale warrants it
- Full corridor activation stack
- Dedicated workforce pipeline activation with apprenticeship programs
  and potentially immigration flex for specialized skills not available
  in domestic labor market

New formation timelines are long — 3–5 years from decision to production
at scale. This pathway must be initiated well ahead of when the capacity
is needed, which requires the demand signal and gap mapping systems to
be operating with sufficient forward horizon.

---

### Component 5: Workforce and Training Pipeline Integration

The intermediate supplier layer is deeply workforce-dependent. Precision
machining, tool and die, casting, and forging are skilled trades that take
years to develop and that the domestic training pipeline has underproduced
for decades.

The coordination system connects directly to the workforce stack:

**Skills gap mapping:**

DoDA maintains a continuous skills demand forecast for industrial input
trades, updated from the same demand signal data used for capacity planning.
The forecast covers: CNC machinists, tool and die makers, pattern makers,
foundry technicians, forge press operators, precision welders, and quality
control technicians.

Skills gap maps are published at the corridor level, enabling training
institutions, apprenticeship programs, and workforce development agencies
to align program capacity with projected demand before the gap becomes acute.

**MEP network integration:**

The Manufacturing Extension Partnership network — a national network of
federally funded regional centers that provide technical assistance to small
and mid-sized manufacturers — is the primary ground-level partner for this
system. MEP centers have existing relationships with the shops this system
is targeting and can serve as:

- Registry onboarding and verification agents
- Technical assistance providers for quality system upgrades
- Connectors between suppliers and workforce training programs
- Local intelligence sources for demand signal validation

MEP integration avoids building parallel infrastructure where effective
infrastructure already exists. The coordination system provides the national
data layer and demand aggregation; MEP provides the regional relationships
and technical depth.

**Apprenticeship pipeline activation:**

Identified workforce gaps in target corridors trigger activation of the
National Apprenticeship Manufacturing Pipeline for the relevant trades.
Apprenticeship programs in precision machining, tool and die, and foundry
operations are deployed at the corridor level in coordination with supplier
capacity investment timelines — so that trained workers are available when
new capacity comes online rather than 18 months after.

Community college and technical institute partnerships are established in
advance in target corridors, with curriculum aligned to the specific process
capabilities identified in the registry and demand signal data.

**Immigration flex:**

For specialized skills where the domestic training pipeline cannot produce
qualified workers within the required timeline — particularly advanced die
design, complex forging process engineering, and precision metrology — the
Strategic Manufacturing Visa Framework provides targeted immigration
pathways. Allied country nationals with relevant certifications receive
expedited processing.

---

### Component 6: Timing and Sequencing Coordination

The Execution Corps manages sequencing across the system to prevent the two
most common coordination failures: premature supplier investment (capacity
built before demand materializes) and delayed input availability (capacity
not ready when anchor factories need it).

**Sequencing principles:**

Demand commitment before supplier investment. Conditional offtake commitments
are activated before PCA instruments deploy for new formation pathways.
Suppliers do not commit capital before demand is partially committed.

Infrastructure before capacity. Corridor power, logistics, and utility
infrastructure milestones are verified before supplier facility construction
begins. A machining shop that builds a new facility and then waits 18 months
for grid interconnection has not solved the availability problem.

Workforce pipeline before hiring ramp. Apprenticeship and training programs
are activated 24–30 months before projected hiring ramp. Suppliers cannot
scale if qualified workers are not available when capacity comes online.

Supplier qualification before anchor factory commissioning. The timeline
for supplier qualification — which can take 12–18 months in regulated
industries — must begin well before the anchor factory needs the inputs.
Execution Corps tracks supplier qualification milestones alongside factory
construction milestones and escalates when qualification is falling behind.

**Corridor-level coordination:**

In active manufacturing corridors, the Execution Corps maintains a live
sequencing map showing:

- Anchor factory construction and commissioning timeline
- Required supplier qualification deadlines by input category
- Supplier ramp timelines against those deadlines
- Workforce pipeline progress against projected hiring needs
- Infrastructure readiness milestones

This map is the operational tool that converts the coordination system from
a data infrastructure into active gap management. When a supplier qualification
is falling behind, the Execution Corps escalates — not to manage the supplier,
but to identify and resolve the constraint causing the delay.

---

## Gap Classification and Response Logic

Not all supplier gaps are equal. The system classifies identified gaps by
severity and responds accordingly.

**Class 1 — Visibility gap:** Domestic supply exists but is not discoverable.
Response: Registry onboarding and MEP outreach. No capital required. Fastest
resolution pathway.

**Class 2 — Scale gap:** Domestic supply exists but at insufficient volume
for the identified demand. Response: Demand signal publication and tooling
finance for domestic expansion. Pathway A.

**Class 3 — Capability gap:** Domestic supply exists in adjacent processes
but not the specific capability required. Response: MEP technical assistance,
targeted training, and tooling finance for capability upgrade. Modified
Pathway A with longer timeline.

**Class 4 — Proximity gap:** Supply exists nationally or in allied countries
but not within viable logistics distance of the demand concentration.
Response: Allied entry pathway (Pathway B) or targeted domestic formation
in the relevant corridor. Demand commitment may be required.

**Class 5 — Existence gap:** No domestic or allied supply exists in the
category at the required scale. Response: New formation pathway (Pathway C)
with demand commitments, first-loss capital, and full corridor activation.
Longest timeline; must be initiated earliest.

DoDA publishes gap classification by category and corridor as part of the
corridor readiness dashboard. Manufacturers can see in advance which input
categories they can expect to source domestically and on what timeline.
This forward visibility allows procurement planning to begin before factory
construction rather than after.

---

## Priority Queue and Allocation Discipline

Not all identified supplier gaps are addressed simultaneously. The system
operates under capital, workforce, and execution constraints, requiring
explicit prioritization across input categories and corridors.

### Priority Drivers

Supplier activation efforts are ranked based on:

**Cascade Risk Severity**
The degree to which absence of the input creates downstream production
failure across multiple sectors. Inputs that sit at the intersection of
several Alliance-Critical domains — a machined component required by energy
hardware, defense sustainment, and automotive simultaneously — rank higher
than single-sector inputs of equivalent volume.

**Target Map Criticality**
Alignment with Category A and B domains in the Alliance Industrial Target
Map. Inputs whose absence would degrade IDP compliance receive priority
over inputs in Globally Competitive or non-designated categories.

**N+2 Gap Distance**
The degree of deviation from required redundancy thresholds. A category
where domestic supply covers 30% of requirement ranks higher than one
covering 80%, all else equal.

**Time-to-Scale**
Expected time required to bring capacity online relative to projected demand
timelines. Categories with long lead times — specialty forgings, precision
tooling, investment casting for aerospace — must be initiated earliest even
if current gap severity appears moderate, because the consequence of
late initiation is supply absence at exactly the moment demand peaks.

**Corridor Readiness**
The ability to deploy capacity quickly given infrastructure, workforce, and
regulatory conditions. A high-priority gap in a Tier I corridor is actioned
before the same gap in a Tier III corridor, because execution is achievable
without enablement investment first.

### Allocation Rules

- Class 4 and Class 5 gaps in Category A domains receive highest priority
  and are addressed before Class 1–3 gaps in lower-priority categories,
  regardless of the relative ease of resolution
- Inputs that unlock multiple downstream sectors are prioritized over single-
  use categories of equivalent strategic classification
- Supplier activation is limited to the minimum set of interventions required
  to eliminate system vulnerability, not to maximize total domestic capacity;
  the objective is resilience sufficiency, not industrial maximalism
- Priority queue is reviewed quarterly and updated as gap closure progresses,
  demand signals shift, and corridor readiness evolves

### Transparency

DoDA publishes:

- The prioritized supplier activation queue by category and corridor,
  updated quarterly
- The rationale for prioritization decisions, including which criteria drove
  relative ranking
- Gap closure status over time, showing movement from initial classification
  through activation to resolution

This ensures the coordination system remains rule-based, auditable, and
insulated from discretionary allocation or political pressure to address
lower-priority gaps ahead of higher-priority ones.

---

## Deployment Triggers

The coordination system is activated — meaning active Execution Corps
engagement, demand aggregation, and PCA instrument deployment — when any
of the following conditions are identified by DoDA:

- Alliance Industrial Target Map identifies critical input gaps in an
  active or planned manufacturing corridor
- Corridor readiness scores show sufficient anchor demand but insufficient
  supplier density for the deployment to proceed without domestic input
  shortfall
- Supplier concentration in a critical input category exceeds IDP
  chokepoint thresholds — defined as more than 60% of domestic supply
  from a single source, or more than 40% from non-allied international
  sources
- DoDA identifies temporal misalignment between supplier qualification
  timelines and anchor factory commissioning dates with fewer than 18
  months to resolve

For ongoing corridor operations, the system runs continuously rather than
being triggered episodically. Demand signals update on a rolling basis.
Gap classifications update as new suppliers register and existing suppliers
report capacity changes.

---

## Failure Modes and Mitigation

**Demand overestimation**
Suppliers build capacity against aggregated demand signals that don't
materialize at projected volumes.
Mitigation: Conservative demand bundling methodology, conditional rather
than guaranteed commitments, phased capacity activation, and DoDA iterative
demand updates that incorporate realized versus projected actuals.

**Registry quality degradation**
Registry entries become stale, inaccurate, or populated with suppliers
who cannot actually perform at registered capability levels.
Mitigation: Annual capability update requirement, MEP verification for
registered suppliers, and manufacturer-reported performance data feeding
back into registry ratings over time.

**Coordination without commitment**
The system produces visibility and aggregation but commitments remain too
weak to unlock investment, particularly for Class 4 and Class 5 gaps.
Mitigation: Federal procurement anchor commitments in defense-adjacent
categories; PCA first-loss instruments for higher-risk new formation;
explicit minimum commitment thresholds that trigger escalation if not
met within defined timeframes.

**Training pipeline lag**
Capacity investment outpaces workforce availability, producing facilities
that cannot hire qualified workers.
Mitigation: Skills gap forecasting initiated 30+ months ahead of projected
hiring demand; apprenticeship program activation timed to capacity
investment decisions, not factory commissioning dates.

**Allied supplier substitution for domestic development**
Pathway B (allied entry) becomes the default response to all gaps,
producing US-facility presence without genuine domestic capability development.
Mitigation: Allied entry is explicitly time-limited as a gap-filling
mechanism. Allied firms accessing the support stack are required to
include domestic workforce development plans with milestone commitments.
DoDA tracks domestic-versus-allied sourcing ratios by category and
corridor over time, with targets for domestic share growth.

---

## Integration with the Full Manufacturing Stack

This system is the connective tissue between the anchor manufacturing
layer (Factory JVs, regional pilot playbooks) and the raw materials layer
(domestic refining and processing corridors, NORAM critical materials).

**Upstream:** Raw material suppliers — steel mills, aluminum smelters,
specialty metals processors — need demand visibility from the intermediate
layer just as intermediate suppliers need it from manufacturers. The
demand signal ingestion system extends upstream where relevant, providing
materials processors with aggregate demand signals from the casting,
forging, and machining layer.

**Downstream:** Anchor manufacturers in Factory JVs and pilot corridors
are required to publish forward input demand through the coordination
system as a condition of PCA instrument access. This is the primary
mechanism for demand signal generation and creates a direct connection
between the anchor layer and the supplier ecosystem.

**Workforce:** The skills gap mapping and apprenticeship pipeline
activation in this system integrate directly with the National
Apprenticeship Manufacturing Pipeline and the Industrial Signal Authority
forecasting model. The coordination system is a demand signal source for
workforce planning, not a parallel system.

**Capital:** PCA instruments deployed through this system — primarily
tooling finance and supplier credit facilities — are coordinated with
corridor-level PCA deployments. Supplier capacity investment is sized
against demand signals and commitment structures, ensuring capital
deployment is grounded in verifiable forward demand rather than
speculative projections.

---

## Success Metrics

**Registry metrics:**
- Domestic supplier coverage by process category and corridor (share of
  known capacity represented in registry)
- Allied supplier coverage for IDP-priority input categories
- Manufacturer adoption rate (share of anchor manufacturers using registry
  for domestic sourcing decisions)

**Demand coordination metrics:**
- Share of anchor manufacturer input demand published through the system
- Demand aggregation pool size by category (total committed volume)
- Conditional commitment activation rate (commitments that triggered
  supplier investment versus total commitments issued)

**Supplier activation metrics:**
- Gap closure rate by classification (Class 1–5)
- Domestic supplier formation and expansion rate in target corridors
- Time from gap identification to domestic supply availability by class

**System-level metrics:**
- Reduction in import dependency for identified critical input categories
- Alignment between supplier qualification timelines and factory
  commissioning dates (Execution Corps sequencing metric)
- Private capital participation in supplier layer (crowd-in ratio for
  tooling finance and supplier credit instruments)
- Domestic sourcing share by input category over time

---

## Closing

The intermediate supplier layer is where most domestic manufacturing
ambitions quietly fail. Manufacturers who want to produce in America
discover that the inputs they need — the castings, forgings, machined
components, and tooling — either don't exist domestically at the right
quality, scale, or location, or exist but are impossible to find without
months of manual search.

This system makes that layer visible, investable, and scalable. It does
not mandate domestic sourcing. It makes domestic sourcing the path of
least resistance by ensuring that the information, demand signals, capital
access, and workforce pipelines that suppliers need to serve domestic
manufacturers are available as a coordinated package rather than a series
of individually unsolvable problems.

The coordination failure is real. The solution is infrastructure — data
infrastructure, commitment infrastructure, training infrastructure, and
capital infrastructure — deployed simultaneously on both sides of the
market.

The system precedes capital deployment and reduces the need for high-risk
intervention by resolving coordination failures upstream of investment.

When a manufacturer can search a registry and find a qualified casting
shop 200 miles away, get a demand signal showing that 12 other manufacturers
need the same input, and connect that shop to tooling finance and an
apprenticeship pipeline to scale — the coordination problem dissolves.

Not because government built the factory. Because government built the
conditions under which the market could.
