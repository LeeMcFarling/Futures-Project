# Domain Maturity Tracker: Agriculture

**Last Updated:** 2026-05-13
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
Restore farm-level agency, reduce structural risk, and rebuild food system resilience through integrated data transparency, equipment rights, seed IP reform, competitive financing, and water security — without top-down consolidation or bureaucratic production management.

**Key Questions:**
- How do we lower structural risk for farmers without insulating them from market signals?
- What data rights and equipment rights reform creates genuine farmer agency?
- How do we secure long-run water and supply chain resilience without new federal mandates?

**Success Criteria:**
- Farmers have real-time market signal access and equipment ownership over their data
- Seed IP reform restores competition and reduces single-point-of-failure risk
- Water and aquifer governance frameworks deployed in at-risk regions
- Supply chain risk audited and diversification incentives activated

---

## Subdomain Status Matrix

| Subdomain | Phase | File Count | Word Count | Key Gaps | Dependencies | Next Action | Target Date |
|-----------|-------|------------|------------|----------|--------------|-------------|-------------|
| Overview | 3 | 1 | ~850 | Regional differentiation; crop-specific instantiation | None | Regional overlays | TBD |
| Data_and_Market_Signals | 3 | 1 | ~1,525 | Platform integration spec; DoDA linkage | department-of-data-and-accountability | DoDA integration spec | TBD |
| Finance | 3 | 1 | ~1,285 | PCA lending instrument spec; credit union integration | public-capital-authority | PCA lending instrument | TBD |
| Equipment_Rights | 3 | 1 | ~1,330 | Enforcement mechanism; FTC role | Regulatory_Compression | Enforcement spec | TBD |
| Supply_Chain | 3 | 1 | ~1,245 | Critical chokepoint audit; domestic sourcing alternatives | manufacturing-domain | Chokepoint audit methodology | TBD |
| Farmer_Economics | 3 | 1 | ~1,340 | Risk reduction pilot design; SSI/UPI integration | ssi-self-sovereign-identity-framework | Pilot selection criteria | TBD |
| Seed_IP | 3 | 1 | ~1,400 | Antitrust application roadmap | Regulatory_Compression | Antitrust pathway spec | TBD |
| Water_and_Aquifer | 3 | 1 | ~1,235 | Aquifer governance enforcement; interstate compact design | Climate_Risk | Interstate compact framework | TBD |

---

## Dependency Map

### Hard Dependencies (Blocking)
| This Domain Requires | From Domain | Status | Risk Level |
|---------------------|-------------|--------|------------|
| PCA lending instrument design | Budget_and_Fiscal_Policy | Phase 3 | Medium |

### Soft Dependencies (Coordination)
| This Domain Benefits From | From Domain | Status | Notes |
|--------------------------|-------------|--------|-------|
| Measurement backbone | Institutional-Modernization (DoDA) | Phase 3 | Farm-level outcome tracking |
| Regulatory modernization | Institutional-Modernization (Regulatory_Compression) | Phase 2 | Equipment rights, seed IP enforcement |
| Water governance | Climate_Risk | Phase 3 | Overlapping water-and-aquifer-resilience file |
| SSI/UPI identity layer | Technology_and_Data | Phase 2 | Farm data ownership + market signal access |

### Provides To (Downstream Impact)
| Other Domain | What We Provide | Criticality |
|--------------|-----------------|-------------|
| Healthcare (Public_Health_Nutrition) | Supply chain integrity for school procurement | Medium |
| Climate_Risk | Water governance architecture inputs | Medium |
| Trade_Policy | Domestic food security baseline for trade negotiation | Medium |

---

## Gap Analysis

### Tier 1: Critical Gaps (Missing Foundation)
- [x] **Farm economics and risk reduction** — farmer-economics-and-risk-reduction.md: structural risk overlay, insurance alternatives, income floor design ✅
- [x] **Data rights and market signals** — agricultural-data-and-market-signals.md: ownership architecture, price transparency, market signal access ✅
- [x] **Equipment rights** — agricultural-right-to-repair-and-data-rights.md: right-to-repair doctrine, data rights framework ✅
- [x] **Seed IP reform** — seed-ip-and-research.md: competitive seed market, R&D commons architecture ✅
- [x] **Water and aquifer resilience** — water-and-aquifer-resilience.md: aquifer governance, irrigation efficiency, interstate compact framework ✅

### Tier 2: Structural Gaps (Incomplete Coverage)
- [ ] **Pilot program design** — farm-level pilot selection criteria, DoDa outcome metrics for agricultural interventions — Target: Phase 4
- [ ] **Regional overlays** — crop-specific and geography-specific instantiations (Midwest grain belt, western water stress, southern specialty crops) — Target: Phase 4
- [ ] **PCA lending instrument** — specific lending structures for farm finance through PCA — Target: Phase 3

### Tier 3: Enhancement Gaps (Nice-to-Have)
- [ ] **Food system security** – Domestic production baseline, import dependency audit – Target: Phase 4
- [ ] **Rural economic integration** – Linkage to Labor/rural workforce and Housing/rural access – Target: Phase 4

---

## Phase Advancement Checklist

### Requirements for Phase 4 (Sequencing & Execution)
- [ ] Pilot selection criteria defined (which regions, which instruments first)
- [ ] PCA lending instrument specified
- [ ] DoDA agricultural metric catalog
- [ ] Enforcement pathway for equipment rights and seed IP (FTC/DOJ coordination)
- [ ] Water interstate compact framework drafted

---

## Recent Activity Log

| Date | Subdomain | Change | Phase Impact |
|------|-----------|--------|--------------|
| 2026-05-13 | All | Domain decomposed from Economic_Prosperity; YAML updated (domain: Agriculture, subdomain: Agriculture, slug prefix /agriculture/); maturity tracker created | Domain established |
| 2026-01-28 | All | Domain created (as subdomain of Economic_Prosperity); 8 files; YAML standardized | 0 → 3 |

---

## Notes & Context

- Domain has **8 files** totaling ~10,200 words
- **Decomposed from Economic_Prosperity** on 2026-05-13 — previously a subdomain, now a standalone domain
- Water-and-aquifer-resilience.md is shared with Climate_Risk domain (same file, different domain context)
- Agriculture reform is deliberately non-interventionist in production decisions — focuses on market transparency, data rights, and structural risk reduction; not subsidy architecture or production quotas
- Equipment rights (right-to-repair) has cross-domain antitrust enforcement linkage with Regulatory_Compression
- Seed IP reform is the highest-leverage structural intervention — single-company concentration creates civilizational food system risk
- Farmer economic security instruments connect to SSI/UPI for income attestation and risk-indexed support delivery
