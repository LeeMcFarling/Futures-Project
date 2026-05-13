# Domain Maturity Tracker: Climate_Risk

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
Build financial and physical resilience to climate-driven catastrophic risk — through a national reinsurance backstop, wildfire governance reform, and aquifer/water security — without treating climate as a carbon-tax ideological frame. Focus is on risk management, insurance market stabilization, and infrastructure resilience.

**Key Questions:**
- How do we prevent private insurance market collapse in high-risk geographies without moral hazard?
- What wildfire governance structure aligns land management, local fire codes, and state/federal coordination?
- How do we govern aquifer depletion before it becomes irreversible?

**Success Criteria:**
- National Catastrophe Reinsurance System (NCRS) operational with risk-based premium structure
- Wildfire mitigation governance deployed in at-risk western jurisdictions
- Aquifer governance frameworks established in critical overdraft regions

---

## Subdomain Status Matrix

| Subdomain | Phase | File Count | Word Count | Key Gaps | Dependencies | Next Action | Target Date |
|-----------|-------|------------|------------|----------|--------------|-------------|-------------|
| Overview | 3 | 1 | ~1,265 | Deployment sequencing; sector-specific risk maps | department-of-data-and-accountability | Regional risk mapping spec | TBD |
| Catastrophe_Reinsurance | 3 | 1 | ~1,654 | Actuarial methodology; premium-setting governance; phase-in sequencing | public-capital-authority | Actuarial design spec; PCA capitalization structure | TBD |
| Wildfire_Governance | 3 | 1 | ~1,401 | Enforcement authority; land management agency coordination (USFS, BLM, state); prescribed burn liability reform | execution-corps-spec | Agency coordination spec; liability reform language | TBD |
| Water_and_Aquifer | 3 | 1 | ~1,748 | Aquifer-specific governance enforcement; interstate compact design; monitoring infrastructure | Agriculture, department-of-data-and-accountability | Interstate compact framework; DoDA monitoring spec | TBD |

---

## Dependency Map

### Hard Dependencies (Blocking)
| This Domain Requires | From Domain | Status | Risk Level |
|---------------------|-------------|--------|------------|
| Capital backstop for NCRS | Budget_and_Fiscal_Policy (PCA) | Phase 3 | Low — PCA spec exists |

### Soft Dependencies (Coordination)
| This Domain Benefits From | From Domain | Status | Notes |
|--------------------------|-------------|--------|-------|
| Measurement backbone | Institutional-Modernization (DoDA) | Phase 3 | Risk monitoring, outcome tracking |
| Execution instrument | Institutional-Modernization (Execution Corps) | Phase 3 | Wildfire mitigation deployment |
| Water governance | Agriculture | Phase 3 | Overlapping water-and-aquifer-resilience file |
| Energy regulatory sandbox | Energy | Phase 3 | Grid resilience as climate risk interface |

### Provides To (Downstream Impact)
| Other Domain | What We Provide | Criticality |
|--------------|-----------------|-------------|
| Housing_and_Public_Infrastructure | Insurance market stability; flood/fire zone governance | High |
| Agriculture | Water governance framework | Medium |
| Energy | Grid resilience risk framework | Medium |

---

## Gap Analysis

### Tier 1: Critical Gaps (Missing Foundation)
- [x] **National Catastrophe Reinsurance System** — national-catastrophe-reinsurance-system.md: federal backstop, risk-based premium structure, private market phase-in, moral hazard mitigation ✅
- [x] **Wildfire Mitigation Governance** — wildfire-mitigation-and-landscape-risk-governance.md: land management coordination, prescribed burn governance, risk scoring, local code enforcement ✅
- [x] **Water and Aquifer Resilience** — water-and-aquifer-resilience.md: aquifer governance, overdraft triggers, irrigation efficiency, interstate compact architecture ✅

### Tier 2: Structural Gaps (Incomplete Coverage)
- [ ] **NCRS Actuarial Methodology** — premium-setting governance, risk classification criteria, anti-adverse-selection rules — Target: Phase 4
- [ ] **Wildfire Agency Coordination** — USFS/BLM/state land management coordination spec; prescribed burn liability reform — Target: Phase 4
- [ ] **Flood Risk Integration** — flooding as distinct risk category from wildfire; FEMA NFIP reform interface — Target: Phase 3

### Tier 3: Enhancement Gaps (Nice-to-Have)
- [ ] **Extreme heat governance** – Urban heat island mitigation; labor protections under extreme heat — Target: Phase 4
- [ ] **Sea level rise** – Coastal infrastructure governance, managed retreat doctrine — Target: Phase 4

---

## Phase Advancement Checklist

### Requirements for Phase 4 (Sequencing & Execution)
- [ ] NCRS capitalization structure and PCA backstop sizing
- [ ] NCRS premium-setting methodology and risk classification
- [ ] Wildfire agency coordination protocol
- [ ] Aquifer governance enforcement trigger design
- [ ] DoDA monitoring infrastructure spec for climate risk metrics

---

## Recent Activity Log

| Date | Subdomain | Change | Phase Impact |
|------|-----------|--------|--------------|
| 2026-05-13 | All | Domain decomposed from Economic_Prosperity; YAML updated (domain: Climate_Risk, subdomain: Climate_Risk, slug prefix /climate-risk/); maturity tracker created | Domain established |
| 2026-03-04 | All | Climate_Risk files moved to Economic_Prosperity/Climate_Risk subdomain; YAML standardized; subdomain domain field set to Economic_Prosperity | 0 → 3 |

---

## Notes & Context

- Domain has **4 files** totaling ~6,068 words
- **Decomposed from Economic_Prosperity** on 2026-05-13 — previously subdomain Climate_and_Resilience, now standalone domain Climate_Risk; subdomain field also corrected from Climate_and_Resilience → Climate_Risk
- **Framing is risk management, not carbon ideology** — NCRS, wildfire governance, and water security are risk instruments that command bipartisan support; the brief does not require climate agreement as a political precondition
- **NCRS is the insurance market stabilization instrument** — prevents the market failure already underway in California, Florida, and Louisiana where private insurers are withdrawing; the alternative (state last-resort insurers) creates fiscal instability for state governments
- **Water-and-aquifer-resilience.md** is shared with Agriculture domain — both domains reference the same physical infrastructure; governance framing differs (Agriculture: farmer economic risk; Climate_Risk: systemic resource depletion)
- The wildfire RMS overlay in Institutional-Modernization/Regulatory_Compression (energy-regulatory-modernization-sandbox.md) is the regulatory reform complement to this domain's governance framework
- Domain is thin but focused — 4 files is intentional; risk management instruments are the right scope for this domain; broader climate energy transition lives in Energy domain
