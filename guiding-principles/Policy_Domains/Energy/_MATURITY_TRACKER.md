# Domain Maturity Tracker: Energy

**Last Updated:** 2026-06-04
**Overall Domain Phase:** 3
**Domain Owner:** TBD

---

## Phase Model Reference

- **Phase 0** – Problem Framing
- **Phase 1** – Strategic Constraints
- **Phase 2** – Structured Exploration
- **Phase 3** – Outcomes & Decision Rules
- **Phase 4** – Sequencing & Execution Design
- **Phase 5** – External Validation
- **Phase 6** – Messaging & Rebuttal

---

## Domain Overview

**Purpose:**
Achieve energy abundance as the foundation of economic competitiveness — through a portfolio-neutral supply expansion strategy (nuclear, gas, renewables, distributed), regulatory modernization that removes unnecessary permitting friction, a siting model that distributes economic participation, and PCA capital instruments that replace opaque subsidy with recyclable investment.

**Key Questions:**
- How do we expand energy supply fast enough to meet manufacturing reindustrialization demand?
- What regulatory framework removes friction without removing safety accountability?
- How do we deploy capital at scale without creating subsidy dependency?
- How do we handle grid reliability during transition?

**Success Criteria:**
- Energy Regulatory Modernization Sandbox (RMS) active in at least 3 jurisdictions
- PCA energy portfolio capitalized with clear deployment sequence
- Portfolio-neutral supply expansion underway: nuclear permitting reform, gas reliability backstop, distributed solar/storage deployment
- Siting model deployed with community economic participation requirements

---

## Subdomain Status Matrix

| Subdomain | Phase | File Count | Word Count | Key Gaps | Dependencies | Next Action | Target Date |
|-----------|-------|------------|------------|----------|--------------|-------------|-------------|
| Strategy | 3 | 2 | ~3,707 | Demand forecast tied to manufacturing reindustrialization | Manufacturing | Demand forecast integration with manufacturing ramp | TBD |
| Deployment_Architecture | 3 | 2 | ~1,756 | Deployment sequence and pilot geography | public-capital-authority, execution-corps-spec | Deployment sequence spec; pilot geography selection | TBD |
| Regulatory_Modernization | 3 | 1 | ~1,977 | Sector-specific regulatory overlay depth; FERC coordination | energy-regulatory-modernization-sandbox, Institutional-Modernization (Regulatory_Compression) | FERC interface; sector-specific RMS overlay | TBD |
| Siting_and_Participation | 3 | 1 | ~1,403 | Community participation spec; revenue sharing structure | public-capital-authority | Revenue sharing design | TBD |
| Demand_Cost_Allocation | 0 | 0 | 0 | **TODO: Hyperscaler demand delta coverage brief** — large new commercial loads (data centers, AI compute facilities) must pay for the incremental grid infrastructure their demand delta creates; costs not socialized to existing ratepayers; pre-interconnection grid impact study establishes demand baseline and delta; hyperscaler pays for all transmission, substation, and distribution upgrades attributable to their load; ongoing capacity charge reflects their grid infrastructure share; creates accurate location incentives (choose sites with existing headroom, invest in on-site generation/storage, participate in demand response); closes the gap where abundance-side price reductions are offset by infrastructure cost socialization from large new loads; cross-ref: energy-regulatory-modernization-sandbox (interconnection reform), energy-siting-and-distributed-participation-overlay (prosumer participation), Technology_and_Data (hyperscalers as IDP compute infrastructure) | energy-regulatory-modernization-sandbox, public-capital-authority | Write demand delta coverage brief | TBD |
| PCA_Finance | 3 | 1 | ~2,812 | Portfolio-level exit strategy; recycling timeline | public-capital-authority-and-allocation-framework | Exit strategy spec; recycling cadence | TBD |

---

## Dependency Map

### Hard Dependencies (Blocking)
| This Domain Requires | From Domain | Status | Risk Level |
|---------------------|-------------|--------|------------|
| Capital deployment instrument | Budget_and_Fiscal_Policy (PCA) | Phase 3 | Low — PCA spec exists |
| Regulatory modernization instrument | Institutional-Modernization (Regulatory_Compression / RMS) | Phase 2 | Low — RMS spec exists |

### Soft Dependencies (Coordination)
| This Domain Benefits From | From Domain | Status | Notes |
|--------------------------|-------------|--------|-------|
| Manufacturing demand signal | Manufacturing | Phase 3 | Energy demand driven by reindustrialization |
| Execution instrument | Institutional-Modernization (Execution Corps) | Phase 3 | Construction/deployment corps |
| Grid resilience risk framing | Climate_Risk | Phase 3 | Climate risk as energy supply risk |

### Provides To (Downstream Impact)
| Other Domain | What We Provide | Criticality |
|--------------|-----------------|-------------|
| Manufacturing | Energy cost certainty; supply adequacy for industrial demand | Critical |
| National_Security | Energy independence as strategic asset | High |
| Housing_and_Public_Infrastructure | Grid reliability and local energy resilience | Medium |
| Climate_Risk | Reliable low-carbon transition architecture | Medium |

---

## Gap Analysis

### Tier 1: Critical Gaps (Missing Foundation)
- [x] **Abundance strategy** — energy-abundance-strategy-overview.md + abundance-first-decarbonization-and-reliability-transition.md: portfolio-neutral supply expansion, reliability-first framing, demand growth modeling ✅
- [x] **Deployment architecture** — energy-deployment-architecture.md: deployment sequence, grid integration, capital structure ✅
- [x] **Portfolio mix** — energy-portfolio-mix.md: nuclear, gas, renewable, distributed storage — portfolio governance framework ✅
- [x] **Regulatory modernization sandbox** — energy-regulatory-modernization-sandbox.md: RMS overlay for energy sector; permitting compression; pilot governance ✅ (also referenced in Institutional-Modernization/Regulatory_Compression as sector overlay)
- [x] **Siting and participation** — energy-siting-and-distributed-participation-overlay.md: community economic participation, revenue sharing architecture ✅
- [x] **PCA finance strategies** — pca-finance-strategies.md: PCA energy portfolio design, debt/equity instruments, recycling mechanics ✅

### Tier 2: Structural Gaps (Incomplete Coverage)
- [ ] **Hyperscaler demand delta coverage** — BRIEF NEEDED: large new commercial loads (data centers, AI compute) pay for the incremental grid infrastructure their demand creates; pre-interconnection impact study establishes demand delta; all upgrade costs (transmission, substations, distribution) attributed to the new load, not socialized to existing ratepayers; ongoing capacity charges reflect grid infrastructure share; Northern Virginia/Dominion Energy pattern is the documented failure mode — consumer advocates have flagged residential ratepayers subsidizing trillion-dollar corporation grid buildouts; accurate cost attribution changes hyperscaler location decisions toward sites with existing grid capacity and creates incentives for on-site generation, storage, and demand response participation; pairs with supply-side abundance work to complete the consumer price protection picture: abundance brings prices down, demand delta coverage prevents large new loads from pushing them back up through rate base socialization — Target: Phase 2
- [ ] **Nuclear permitting reform** — specific NRC reform pathway, small modular reactor (SMR) permitting doctrine — Target: Phase 4
- [ ] **Grid reliability during transition** — gas backstop governance; reliability standards under renewable penetration — Target: Phase 4
- [ ] **Manufacturing demand integration** — energy demand forecast tied to manufacturing reindustrialization ramp — Target: Phase 4

### Tier 3: Enhancement Gaps (Nice-to-Have)
- [ ] **Hydrogen** – Production, transport, and end-use governance – Target: Phase 4
- [ ] **Critical minerals** – Domestic supply for energy infrastructure (lithium, cobalt, rare earths) – Target: Phase 4

---

## Phase Advancement Checklist

### Requirements for Phase 4 (Sequencing & Execution)
- [ ] PCA energy portfolio initial capitalization and deployment sequence
- [ ] RMS energy overlay pilot geography (3+ jurisdictions)
- [ ] Nuclear permitting reform pathway (NRC, congressional authorization)
- [ ] Grid reliability backstop during transition (gas role, reserve margin standards)
- [ ] Siting revenue sharing design (community benefit agreement structure)

---

## Recent Activity Log

| Date | Subdomain | Change | Phase Impact |
|------|-----------|--------|--------------|
| 2026-06-04 | Demand_Cost_Allocation | TODO logged: hyperscaler demand delta coverage brief — large new commercial loads pay for incremental grid infrastructure their demand delta creates; cost causer pays principle applied to data center interconnection; prevents supply-side price reductions being offset by infrastructure cost socialization; Northern Virginia Dominion pattern as documented failure mode; cross-ref Energy RMS (interconnection reform) and siting overlay (prosumer participation) | New subdomain at Phase 0 |
| 2026-05-13 | All | Domain decomposed from Economic_Prosperity; YAML updated (domain: Energy, subdomain: Energy, slug prefix /energy/); maturity tracker created | Domain established |
| 2026-01-28 | All | Domain created (as subdomain of Economic_Prosperity); 7 files; YAML standardized | 0 → 3 |

---

## Notes & Context

- Domain has **7 files** totaling ~11,655 words
- **Decomposed from Economic_Prosperity** on 2026-05-13 — previously a subdomain, now a standalone domain
- **Abundance-first framing** is deliberate: avoids the left/right culture war on climate by leading with supply expansion and reliability; decarbonization follows from the portfolio mix and investment structure, not from mandate
- **energy-regulatory-modernization-sandbox.md** exists in both Energy domain and is referenced in Institutional-Modernization/Regulatory_Compression as the Energy sector RMS overlay — canonical version is in Energy; the Regulatory_Compression RMS spec describes the packet structure that the energy overlay implements
- **PCA finance** is the most technically detailed energy document — debt structuring, co-investment mechanics, exit timeline; complements the institutional PCA spec in Budget_and_Fiscal_Policy
- Deployment architecture is thin (~1,064 words) — needs prose depth on grid integration and transmission investment
- Manufacturing domain is the primary energy customer — energy cost certainty is the prerequisite for industrial reindustrialization economics
