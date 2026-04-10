---
id: pharmaceutical-cost-attestation-anti-gaming
title: Pharmaceutical Cost Attestation & Anti-Gaming Framework
sidebar_label: Pharma Anti-Gaming
sidebar_position: 7
slug: /healthcare/pharma/cost-attestation-anti-gaming
domain: Healthcare
subdomain: Pharmaceutical_Reform
policy_type: Enforcement Framework
status: Draft
version: 0.1
author: Futures Project
last_updated: 2026-04-10
dependencies:
  - recoupment-bound-pricing
  - public-capital-backed-drug-discovery
  - pbm-pharmacy-reform
  - sec-administration-heta-steady-state
  - insurance-architecture-sec
  - upi-privacy-preserving-payment-rail
  - ssi-self-sovereign-identity-framework
  - immutable-government-ledger
  - government-outflow-integrity-framework
  - department-of-data-and-accountability
  - idp-industrial-capacity-defense-production
related_initiatives:
  - alliance-industrial-target-map
  - trade-policy-overview
  - healthcare-infrastructure-layer
tags:
  - healthcare
  - pharmaceuticals
  - anti-gaming
  - cost-attestation
  - recoupment
  - drug-pricing
  - international
  - treaty
  - idp
---

# Pharmaceutical Cost Attestation & Anti-Gaming Framework

## What This Is

The recoupment-bound pricing framework defines the end state for pharmaceutical pricing — costs are recovered explicitly, predictably, and once, after which prices step down automatically to cost-plus levels. This document defines how that end state is enforced.

The core problem with any recoupment-based system is that the two inputs — attested costs and tracked revenues — can both be manipulated if the framework relies on self-reporting. Firms can inflate the cost base to extend the recoupment window. They can structure revenue flows to suppress the apparent US revenue count. They can allocate international costs aggressively to justify domestic prices. Without a verification architecture, recoupment-bound pricing is a promise with no enforcement mechanism.

This framework closes that gap using the same institutional logic applied elsewhere in the ecosystem: mandate standardized cost attestation under perjury-backed legal obligation, track revenue through the UPI rail rather than relying on self-reporting, compare attested costs against peer submissions to surface anomalies, and audit outliers against the immutable ledger. HETA operates the enforcement function. DoDA certifies the methodology. The ledger records everything.

The domestic architecture addresses the attestation and revenue tracking problem. The international extension — a treaty-based shared ledger with IDP-allied nations — addresses the global pricing arbitrage problem that domestic mechanisms alone cannot reach.

---

## Core Principle

Pharmaceutical firms that benefit from US market access must be able to demonstrate that their pricing reflects documented costs and legitimate returns. The framework does not set prices. It verifies the inputs that determine when prices must step down. Firms that attest honestly and price accordingly operate without friction. Firms that cannot defend their cost claims against their own attestations and their peer comparisons face escalating consequences.

The same logic that governs government outflows — standardized format, perjury-backed attestation, immutable ledger, peer comparison, audit escalation — applies here. The government's tolerance for opacity in pharmaceutical pricing is the same as its tolerance for opacity in government spending: none.

---

## Eligible Cost Base — What Goes Into the Recoupment Clock

### Domestic Default

The default recoupment clock is US-only. Only costs that meet all of the following criteria are eligible for inclusion in the recoupment base:

- R&D conducted within the United States, or conducted internationally but funded through US-based legal entities and directly attributable to the drug being recouped
- Manufacturing scale-up and validation costs for US-market supply
- Regulatory costs associated with US market authorization (FDA, clinical trials required for US approval)
- A pro-rated share of failed program costs from the same development portfolio, calculated using the standardized portfolio allocation methodology defined below
- A capped return multiple on eligible costs, set by statute and published in advance

Costs that are not eligible for the domestic recoupment base:

- International R&D not funded through US entities
- Marketing, advertising, and promotional expenditure
- Lobbying and government affairs
- Executive compensation above a defined statutory cap
- Costs already recouped through a prior drug from the same development program
- Costs associated with lifecycle management extensions (new formulations, new dosing regimens) unless those extensions involved genuinely novel clinical development

### Portfolio Allocation Methodology

Pharmaceutical development involves portfolio risk — firms invest in multiple compounds knowing that most will fail. The framework acknowledges this by allowing failed program costs to be pro-rated into the recoupment base of successful drugs from the same portfolio.

The allocation methodology is standardized:

- Failed programs are allocated to the recoupment base of successful programs in the same therapeutic category and development generation
- Allocation is proportional to development stage reached — a program that reached Phase III before failing contributes more to the portfolio allocation than one that failed in preclinical
- The total portfolio allocation cannot exceed a defined statutory cap as a percentage of the direct program costs of the successful drug
- The allocation methodology is attested at the time of recoupment clock establishment and cannot be revised retroactively

Firms with genuinely high failure rates in high-risk therapeutic areas receive meaningful portfolio credit. Firms that allocate failed programs from unrelated therapeutic areas, or that retroactively reclassify programs to inflate the allocation, face the perjury consequences of having attested to a methodology they are not following.

---

## The Cost Attestation Schema

### Format and Submission

Manufacturers submit cost attestations through the SEC/UPI rail using a standardized machine-readable schema. The schema captures:

- Direct R&D expenditure by phase (preclinical, Phase I, II, III) with supporting documentation requirements
- Personnel costs by category and FTE count
- Contract research organization (CRO) costs with counterparty identification
- Material and compound costs
- Manufacturing scale-up and validation costs by facility
- Regulatory filing costs with FDA reference numbers
- Failed program portfolio allocation with the methodology and calculation shown explicitly
- Capital cost allocation methodology and basis
- Return multiple claimed and statutory authority cited

Submissions are line-item detailed. A top-line number with a narrative justification is not sufficient. The schema requires the same level of specificity as a government contract audit — because that is functionally what this is.

### The Perjury Attestation

Every cost submission is signed with the manufacturer's SSI organizational credential and carries a legally binding attestation that:

- The submitted figures accurately reflect actual costs incurred
- The cost allocation methodology conforms to the standardized framework
- No eligible costs have been double-counted across multiple drugs or recoupment periods
- The submitting officer has personal knowledge of the accuracy of the submission

The attestation creates criminal exposure for material misrepresentation. This is not a compliance checkbox — it is the mechanism by which the cost base becomes legally defensible and legally vulnerable simultaneously. A firm that attests to $2 billion in R&D costs and cannot produce the underlying documentation in an audit has committed a federal offense, not a regulatory violation.

Manufacturers are informed of the attestation obligation and its legal consequences at market authorization. HETA maintains clear guidance on what constitutes material misrepresentation versus legitimate cost accounting variation, published in advance and versioned in the ULRR.

### Timing of Attestation

Cost attestations are submitted at the time of US market authorization and locked. The recoupment clock is established from the attested cost base at that moment. Post-authorization revisions to the cost base are not permitted except in narrowly defined circumstances — discovery of a material accounting error, with full documentation of the error and its correction, subject to HETA review and public disclosure.

Firms cannot submit a preliminary attestation and then revise it upward after seeing competitive dynamics. The clock is set at authorization and runs from that point.

---

## Revenue Tracking — The Rail-Based Recoupment Clock

### Why Self-Reporting Fails

If the recoupment clock relies on manufacturer-reported US revenue, firms can structure revenue flows to suppress the count. Transfer pricing arrangements, distribution fee structures, rebate mechanics, and international revenue allocation all create opportunities to manage apparent US revenue downward while actual cash flows to the firm remain unchanged. Self-reported revenue for recoupment purposes would be gamed within the first development cycle.

### The Rail Solution

Every US transaction involving a recoupment-tracked drug flows through the UPI rail. This includes:

- Wholesale acquisition cost payments from distributors to manufacturers
- Gross-to-net adjustments including rebates, chargebacks, and distribution fees
- PBM and pharmacy service fees paid by manufacturers
- Any other payment flowing between a manufacturer and any downstream US entity related to a covered drug

The rail records each transaction in the immutable government ledger with a standardized drug identifier, transaction type, gross amount, and net amount after adjustments. The recoupment clock is computed by HETA from the observed transaction data — not from manufacturer-reported revenue figures. The manufacturer sees the same clock the government sees, updated in real time as transactions flow through the rail.

Gross-to-net adjustments are logged separately from gross revenue. The recoupment clock runs on net US revenue — the actual cash the manufacturer receives after all adjustments. This prevents the practice of posting artificially high list prices, paying large rebates back through PBMs, and claiming the gross revenue while the net is much lower. Net revenue is what matters for recoupment and net revenue is what the rail tracks.

### Rail Enrollment as a Condition of Market Access

Participation in the UPI pharmaceutical rail is a condition of US market access for all drugs subject to recoupment-bound pricing. Manufacturers who do not enroll in the rail cannot sell in the SEC-covered market. This is not a penalty — it is the same condition that applies to every provider and facility participating in the SEC system. The rail is the infrastructure through which the market operates.

Generic and post-recoupment drugs operating at cost-plus pricing continue to flow through the rail for market transparency and fraud detection purposes, but are not subject to recoupment clock tracking.

---

## The Peer Comparison Database

### Structure

HETA maintains a therapeutic category cost database built from all submitted cost attestations. For each therapeutic category and development pathway — mRNA platform, small molecule oncology, antibiotic, rare disease biologic — the database maintains the distribution of attested costs across all firms that have submitted for drugs in that category.

The database is updated as new attestations are submitted. It is de-identified at the firm level for competitive sensitivity purposes, but the statistical distribution — median, standard deviation, percentile bands — is published and accessible to all market participants. Firms submitting new attestations can see where their claimed costs fall in the distribution before they submit.

### Anomaly Detection

HETA's fraud detection model runs every new cost attestation against the peer comparison database. Attestations that fall outside defined thresholds relative to the peer distribution are flagged for review.

Flagging thresholds vary by category:

- **Phase-level cost anomalies:** Attested costs for a specific development phase (e.g., Phase III clinical trials) that exceed the peer median by more than a defined multiple trigger a phase-level inquiry. The inquiry requests documentation supporting the cost differential — larger trial size, more complex endpoints, unusual patient population, specialized CRO requirements.

- **Portfolio allocation anomalies:** Failed program allocations that exceed peer norms for the therapeutic category trigger a portfolio allocation inquiry. The firm must demonstrate that the allocated programs were genuinely related to the successful drug and that the allocation methodology was applied correctly.

- **Total cost anomalies:** Overall attested cost bases that place in the top percentile of the peer distribution trigger a full attestation audit. This is the most serious flag and initiates the escalation sequence described below.

Most anomaly inquiries resolve at the documentation request stage. Firms with genuinely unusual cost structures — large multinational trials, complex manufacturing requirements, first-in-class compounds — can generally produce documentation that justifies their position in the distribution. The inquiry is diagnostic before it is punitive.

### Novel Compounds — Independent Expert Review

For first-in-class compounds with no peer comparators, the statistical peer comparison is not meaningful. These drugs — the ones where the most important innovation happens — require a different validation mechanism.

For novel compounds designated as first-in-class by FDA at the time of market authorization, cost attestations are subject to independent expert review rather than peer comparison. HETA convenes a panel of independent experts — clinical researchers, health economists, former FDA reviewers, academic cost accounting specialists — who evaluate the attested cost base against:

- Published literature on comparable development programs
- HETA's internal database of development program costs from analogous therapeutic areas
- The submitting firm's own historical cost attestations for prior programs, to assess internal consistency

The expert panel produces a written assessment of whether the attested cost base is within a defensible range. The assessment is not binding — it informs the audit priority queue but does not automatically trigger enforcement. Firms whose attestations fall outside the panel's defensible range face heightened audit scrutiny and must produce detailed documentation justifying the differential.

This mechanism is slower and more resource-intensive than the automated peer comparison, which is appropriate — novel compounds represent a smaller share of submissions and require more careful treatment.

---

## Escalation and Enforcement

### Inquiry

All anomaly flags initiate with a structured inquiry — a documentation request, not an enforcement action. The firm receives notification through their SEC rail account that a submitted attestation has been flagged, with the specific anomaly type and the peer comparison data that triggered the flag. They are asked to provide supporting documentation within a defined response window.

The inquiry is handled by HETA's pharmaceutical compliance function, operating under the enforcement firewall established in the HETA charter. It is explicitly not handled by any function with a relationship to the firm's ongoing market access or regulatory status. The inquiry is a cost verification interaction, not a punitive proceeding, unless the firm's response reveals intentional misrepresentation.

### Audit

Firms that cannot resolve anomaly flags through documentation requests are escalated to full audit. The audit has access to:

- All supporting documentation underlying the cost attestation
- Financial records relevant to the attested cost categories
- CRO contracts and invoices
- Manufacturing cost records
- Internal communications related to cost allocation decisions

Audit authority is established by statute as a condition of market access. Firms that deny audit access or produce materially incomplete documentation trigger automatic escalation to enforcement.

### Enforcement Consequences

Confirmed material misrepresentation in a cost attestation triggers a defined consequence sequence:

1. Recoupment clock correction — the clock is reset based on the audited cost base, which may shorten the remaining recoupment period or trigger immediate step-down to cost-plus pricing if the corrected base is already recouped
2. Financial penalty — a statutory multiplier applied to the revenue collected during the period of misrepresentation
3. Enhanced audit requirements for all subsequent attestations from the same firm for a defined period
4. Public disclosure — the attestation discrepancy, the audit finding, and the corrective action are published in the ULRR with full documentation

For egregious or repeated misrepresentation:

5. Market access suspension — SEC rail access for specific drugs or across the firm's portfolio, depending on the scope of the violation
6. Criminal referral for the attesting officers — the perjury attestation creates personal liability, not just corporate liability

The consequence sequence is graduated and proportionate. A firm that made a genuine accounting error and corrected it fully upon documentation request faces minimal consequences. A firm that systematically inflated its cost base and denied audit access faces market exclusion and criminal referral.

---

## International Extension — The Treaty Framework

### Why Domestic Mechanisms Alone Are Insufficient

A US-only recoupment clock with US-only cost attestation gives firms a legitimate grievance: US revenue is subsidizing global R&D, and the US-only clock does not credit the global contribution. This grievance is partially valid. Pharmaceutical R&D is genuinely global. A drug developed with meaningful international investment should be able to credit international revenue against the global cost base.

The problem is that without verified international revenue data, allowing international credits opens an enormous gaming opportunity. Firms can claim global revenue is low (to keep the global clock running) while claiming global R&D costs are high (to inflate the cost base). Without a shared verification infrastructure, there is no way to distinguish legitimate global R&D from transfer pricing manipulation.

The treaty framework resolves this by extending the attestation and rail architecture to allied nations. Firms that participate in the treaty framework get a global recoupment clock — which is more favorable to them if they genuinely invest globally. In exchange, their revenue in every treaty jurisdiction flows into the shared ledger, and their cost attestations are subject to peer comparison across the combined dataset of all treaty jurisdictions. The information asymmetry that enables gaming is eliminated because the data is mutual and verified.

### The Treaty Architecture

The pharmaceutical cost transparency treaty operates as an extension of the IDP alliance framework into the economic governance of a strategically important sector. It is not a defense treaty but it uses the same institutional logic — allied nations coordinating against a common structural problem that no single country can solve unilaterally.

**Treaty membership:** IDP-aligned nations that have existing pharmaceutical pricing and cost assessment infrastructure — Germany, France, the Netherlands, the UK, Japan, South Korea, Canada, Australia. These countries already conduct sophisticated cost-effectiveness analysis. What they lack is verified cost data. The treaty offers them something genuinely valuable.

**The shared ledger:** Treaty member nations operate a shared pharmaceutical transaction ledger using compatible UPI-equivalent rails. Every drug sale in every treaty jurisdiction is recorded in the shared ledger with the same standardized identifiers. No single nation controls the ledger — it is governed by the treaty body with representation from all members. Firms cannot manipulate revenue reporting in one jurisdiction without the discrepancy being visible across the ledger.

**The shared cost attestation database:** Firms selling in treaty markets attest costs under the shared standardized schema. Attestations are verified against the combined peer comparison database of all treaty jurisdictions — a substantially larger and more statistically robust dataset than any single country could maintain. Cost gaming that might not be detectable against US peers alone becomes visible against the full treaty dataset.

**The global recoupment clock:** Firms enrolled in the treaty framework have their recoupment clocks computed from verified global revenue across all treaty markets. Global costs that meet the treaty's eligibility criteria — conducted in or funded by entities in treaty member nations — are eligible for the global cost base. The clock is favorable to firms with genuine global R&D investment and unfavorable to firms gaming the allocation.

### The Leverage Mechanism

The treaty is attractive to IDP-allied nations for substantive reasons — they get verified cost data they have never had access to before, and they get a coordination mechanism that prevents firms from playing countries against each other. European health ministries are genuinely frustrated by their inability to verify pharmaceutical cost claims. The offer of a shared attestation and revenue ledger is something they would receive seriously, and discussions within the EU on pharmaceutical regulation reform since 2022 create a receptive environment.

For firms, the incentive structure is:

- Firms with genuine global R&D investment choose the treaty framework because the global clock credits their international revenue and is more favorable than the US-only clock
- Firms gaming the allocation resist the treaty framework because the shared ledger eliminates the information asymmetry they depend on

Resistance to treaty enrollment is itself informative. A firm that cannot or will not participate in verified global revenue tracking has something to hide about the relationship between its international pricing and its cost structure. That resistance becomes a public data point.

**Market access conditionality for non-participants:**

Firms that do not participate in the treaty framework operate under the US-only clock with no international cost or revenue credits. They cannot claim that US prices are subsidizing global R&D if they are unwilling to verify either the global costs or the global revenues. Their US recoupment period is computed purely from domestic costs and domestic revenues — the most conservative possible basis.

For drugs where domestic compliers exist — where another firm has developed a therapeutically equivalent or superior drug and has enrolled in the treaty framework — non-participating firms face competitive disadvantage in the SEC formulary classification system. Domestic compliers receive preferred formulary placement. Non-participants receive standard placement. Over time the competitive pressure from compliant firms makes non-participation increasingly costly without requiring explicit exclusion.

For drugs with no domestic complier alternative — genuine first-in-class innovations with no equivalent — the leverage is market access conditionality rather than formulary competition. The consequence sequence for non-participation is the US-only clock, no international credits, and heightened audit scrutiny. This is not a ban. It is a pricing environment structured to make compliance the economically rational choice.

### Allied Enforcement Coordination

Treaty member nations agree to apply parallel enforcement consequences for firms found to have committed material misrepresentation in their shared attestations. A firm that inflates its cost base in the shared system faces consequences not just in the US market but across all treaty markets simultaneously.

This coordinated enforcement eliminates the current dynamic where firms can manage pricing pressure from one country by threatening to withdraw a drug, knowing that other countries will continue to provide revenue. Coordinated withdrawal of SEC rail access across treaty member nations simultaneously is a consequence that no pharmaceutical firm can absorb without fundamental restructuring.

The treaty body maintains a joint enforcement coordination function — not a supranational regulatory body, but a coordination mechanism that allows member nations to synchronize enforcement actions where the same misrepresentation affects multiple markets.

---

## Interaction with the PCA Drug Discovery Framework

Drugs developed with PCA support — where public capital absorbed upstream R&D risk — operate under modified attestation rules.

PCA-supported programs attest costs in the same standardized format, but the PCA contribution is recorded as a separate line item that reduces the privately-funded cost base eligible for recoupment. If PCA funded 40% of Phase I and Phase II costs, the firm's recoupment base reflects the remaining 60% of direct program costs plus eligible portfolio allocation. The PCA recovers its contribution through the revenue-linked instruments established in the drug discovery framework.

This prevents double-counting — the firm cannot recoup costs that the public already funded. It also ensures that the public return on PCA investment flows through the established PCA recovery mechanisms rather than being quietly absorbed into extended recoupment periods.

Drugs developed under PCA partnership receive the same treaty framework benefits as privately developed drugs. PCA partnership does not reduce access to the global clock — it simply ensures that the public contribution to the cost base is accurately reflected.

---

## DoDA's Role

DoDA certifies the methodology underlying the cost attestation framework — the cost accounting standards, the portfolio allocation rules, the peer comparison statistical models, the revenue tracking verification approach. DoDA does not operate the database or conduct audits.

DoDA publishes:
- The certified cost attestation methodology in versioned, machine-readable form in the ULRR
- Aggregate statistics on attestation submissions — distribution of attested costs by therapeutic category, anomaly flag rates, audit escalation rates — without firm-level identification
- Annual assessment of whether HETA's operational practices conform to certified methodology
- Trend analysis on recoupment clock progression across the drug portfolio

If HETA's practices diverge from DoDA's certified methodology, DoDA flags it publicly and Congress receives notification through the cost performance backstop reporting cycle. This preserves DoDA's independence as a measurement institution while keeping HETA accountable for operational integrity.

---

## Guardrails

1. **Attestation is locked at authorization.** The cost base cannot be revised upward after the recoupment clock is established. Downward corrections for accounting errors are permitted with full documentation and public disclosure. Upward revisions are not permitted under any circumstances.

2. **The rail is the revenue source of truth.** Manufacturer-reported revenue figures are not used for recoupment clock computation. The clock runs on observed UPI rail transactions. Discrepancies between manufacturer-reported revenue and rail-observed revenue are treated as material anomalies requiring explanation.

3. **Portfolio allocation is capped.** Failed program costs cannot be allocated without limit. The statutory cap on portfolio allocation as a percentage of direct program costs prevents firms from bundling the costs of an entire R&D portfolio into a single successful drug's recoupment base.

4. **Treaty enrollment is a choice, not a mandate.** Firms that do not enroll operate under the US-only clock with no international credits. The incentive structure makes enrollment rational for firms with genuine global R&D. Non-enrollment is not penalized — it is simply unfavorable relative to enrollment for firms that can defend their global cost claims.

5. **Enforcement is graduated and public.** Consequences escalate from documentation request through audit through financial penalty through market access consequences. Each stage is public — the anomaly flag, the audit finding, the corrective action, and the consequence are all published in the ULRR. Transparency is the primary deterrent.

6. **Criminal liability is personal, not only corporate.** The perjury attestation creates individual criminal exposure for the attesting officers, not just corporate liability for the firm. This prevents the standard corporate defense of blaming a process rather than a person.

---

## Known Gaps — Pending Development

**Biologics biosimilar interaction.** The recoupment framework for biologics and the competitive dynamics of biosimilar entry need more specificity. Biosimilar entry should accelerate the step-down to cost-plus for the reference biologic, but the interaction between the recoupment clock and biosimilar market entry timing is not fully defined.

**Orphan drug and rare disease carve-outs.** The rare disease category receives longer recoupment periods under the base framework. The attestation and peer comparison methodology for orphan drugs — which by definition have thin peer comparison databases — needs more specificity beyond the independent expert review mechanism.

**Generic drug supply chain integrity.** Generic drugs operating at cost-plus prices are not subject to recoupment tracking, but the generic supply chain has its own integrity problems — API sourcing concentration, quality failures, shortage dynamics. This framework does not address generic supply chain resilience, which needs its own treatment.

**Treaty negotiation sequencing.** The treaty framework requires diplomatic negotiation that takes time. This doc describes the end state. The sequencing of treaty negotiations — which countries first, what the interim bilateral arrangements look like before a multilateral treaty is in force, how the domestic framework operates during the negotiation period — needs a dedicated transition architecture doc.
