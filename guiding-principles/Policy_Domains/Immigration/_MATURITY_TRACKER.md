# Domain Maturity Tracker: Immigration

**Last Updated:** 2026-05-16
**Overall Domain Phase:** 2–3
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
Create an immigration system that treats immigration as a strategic national asset: matching legal immigration to labor market needs, separating asylum and economic migration cleanly, securing the border with operational discipline, converting enforcement into a dignified rule-of-law system, and retaining talent that American institutions train. ISA (Immigration Services and Administration) is the execution instrument that replaces ICE/USCIS with a unified service-first model.

**Key Questions:**
- How do we match labor immigration to actual demand signals without over-issuing or under-issuing?
- What enforcement architecture maintains rule of law without humanitarian crisis?
- How do we process asylum claims with integrity and speed?
- How do we retain the talent America trains in its universities?

**Success Criteria:**
- ISA (Immigration Services and Administration) as unified replacement for ICE + USCIS
- Labor immigration tied to employer accountability and real-time demand signals
- Asylum separated cleanly from economic migration with defined processing capacity
- Student-to-industry retention pathways operational
- Transparent oversight dashboards with DoDA integration

---

## Subdomain Status Matrix

| Subdomain | Phase | File Count | Word Count | Key Gaps | Dependencies | Next Action | Target Date |
|-----------|-------|------------|------------|----------|--------------|-------------|-------------|
| System_Architecture | 3 | 1 | ~1,031 | Implementation sequencing; ISA charter language | Institutional-Modernization (execution-corps-spec) | ISA statutory language | TBD |
| ISA_and_Enforcement | 2–3 | 2 | ~1,617 | ISA full operational charter; ICE transition plan | execution-corps-spec | ISA charter spec; ICE transition sequencing | TBD |
| Labor_Immigration | 2–3 | 3 | ~2,315 | Real-time demand signal integration; visa category operationalization | Manufacturing (WCA), Labor_and_Economic_Security | Demand signal architecture; visa category spec | TBD |
| Asylum | 2 | 1 | ~1,049 | Processing capacity design; adjudicator training | None | Capacity spec; adjudicator pipeline | TBD |
| Border_Operations | 2 | 1 | ~622 | Technology layer spec; physical infrastructure standards | Technology_and_Data (SSI) | Technology deployment spec | TBD |
| Student_and_Talent_Retention | 2–3 | 1 | ~530 | OPT reform specifics; startup visa operationalization | entrepreneurship-visas | OPT reform + STEM retention spec | TBD |
| Entrepreneurship | 2 | 1 | ~799 | Investor visa reform details; startup visa criteria | None | Investor criteria spec | TBD |
| Integration_and_Civic | 2 | 1 | ~720 | Civic programming detail; language access spec | Education | Civic integration program design | TBD |
| Oversight_and_Transparency | 2–3 | 1 | ~423 | DoDA dashboard integration spec; metric catalog | department-of-data-and-accountability | Dashboard integration spec; metric catalog | TBD |
| National_Security_Restrictions | 2 | 1 | ~513 | Country-specific criteria; National_Security domain alignment | National_Security (China_Strategy, Foreign_Policy) | Criteria specification; NS alignment | TBD |

---

## Dependency Map

### Hard Dependencies (Blocking)
| This Domain Requires | From Domain | Status | Risk Level |
|---------------------|-------------|--------|------------|
| Execution instrument for ISA deployment | Institutional-Modernization (Execution Corps) | Phase 3 | Low — spec exists |
| Manufacturing labor demand signals | Manufacturing (WCA) | Phase 3 | Low — WCA demand coord exists |

### Soft Dependencies (Coordination)
| This Domain Benefits From | From Domain | Status | Notes |
|--------------------------|-------------|--------|-------|
| Digital identity | Technology_and_Data (SSI/UPI) | Phase 2–3 | Visa tracking, identity verification, ZKP consent |
| Manufacturing demand signal | Manufacturing (industrial-demand-coordination-system.md) | Phase 3 | Real-time labor demand for visa activation |
| National security alignment | National_Security | Phase 3 | Country-based restrictions, adversarial state screening |

### Provides To (Downstream Impact)
| Other Domain | What We Provide | Criticality |
|--------------|-----------------|-------------|
| Manufacturing | Labor supply through targeted circular work visas | High |
| National_Security | Country-based restriction framework; border security architecture | High |
| Labor_and_Economic_Security | Workforce supply; employer accountability enforcement | High |
| Education | International student pipeline; talent retention pathway | Medium |

---

## Gap Analysis

### Tier 1: Critical Gaps (Missing Foundation)
- [x] **System architecture overview** — immigration-system-architecture-overview.md: ISA concept, three-stream architecture (labor/asylum/family), enforcement separation ✅
- [x] **ISA instrument** — immigration-services-and-administration.md: ISA as unified replacement for ICE/USCIS, service-first model ✅ (thin ~974 words; charter spec TBD)
- [x] **Labor immigration** — workforce-immigration-skill-mobility-system.md + targeted-labor-immigration-and-circular-work-visas.md: skill mobility, circular work visas, employer accountability ✅
- [x] **Asylum reform** — asylum-reform.md: clean asylum/economic migration separation, processing architecture ✅
- [x] **Border operations** — border-operations-and-physical-security.md: operational discipline framework ✅
- [x] **Enforcement reform** — immigration-and-customs-enforcement-reform.md: ICE → ISA transition, use-of-force protocols, accountability ✅

### Tier 2: Structural Gaps (Incomplete Coverage)
- [ ] **ISA full operational charter** — immigration-services-and-administration.md is thin (~974 words); needs charter-level spec (org structure, regional offices, performance metrics, relationship to Execution Corps) — Target: Phase 3
- [ ] **Real-time demand signal integration** — labor visa activation should connect to WCA demand coordination system (Manufacturing) and DoDA metric triggers — Target: Phase 4
- [ ] **DACA/existing undocumented population** — no brief on resolution pathway for ~11 million undocumented residents — Target: Phase 3
- [ ] **Citizenship backlog** — no brief on processing existing naturalization backlogs — Target: Phase 3

### Tier 3: Enhancement Gaps (Nice-to-Have)
- [ ] **Family reunification** — policy on family-based immigration categories — Target: Phase 3
- [ ] **Refugee resettlement** — distinct from asylum; strategic refugee admission framework — Target: Phase 4

---

## Phase Advancement Checklist

### Requirements for Phase 3 (Outcomes & Decision Rules)
- [x] System architecture defined ✅
- [x] ISA concept established ✅
- [x] Three-stream separation (labor/asylum/family) defined ✅
- [ ] ISA full operational charter
- [ ] DACA/undocumented resolution framework
- [ ] Demand signal integration architecture

### Requirements for Phase 4 (Sequencing & Execution)
- [ ] ISA statutory language (draft)
- [ ] ICE → ISA transition sequencing
- [ ] Labor visa activation trigger design (demand-signal connected)
- [ ] Asylum processing capacity specification

---

## Recent Activity Log

| Date | Subdomain | Change | Phase Impact |
|------|-----------|--------|--------------|
| 2026-05-16 | All | Tracker updated: file count 11 → 14 active; word count ~7,560 → ~10,624; all new files added; phase 2 → 2–3; ISA instrument recognized as cross-domain with Manufacturing deployment | N/A |
| 2026-04-07 | ISA_and_Enforcement | isa-execution-corps-deployment.md now lives in Manufacturing/workforce-training-and-immigration/ (domain: Manufacturing, subdomain: Labor_Mobility) — ISA deployment model for manufacturing corridors is the primary instantiation; immigration-services-and-administration.md remains the institutional spec | Cross-domain |
| 2026-01-28 | Labor_Immigration | entrepreneurship-visas-and-conversion-pathways.md, student-to-industry-retention-pathways.md added | New |
| 2026-01-28 | Oversight | transparency-metrics-and-oversight-dashboards.md added | New |
| 2026-01-28 | National_Security | national-security-and-country-based-restrictions.md added | New |
| 2025-01-25 | All | YAML standardized, moved from People_Skills_Health | N/A |

---

## Notes & Context

- Domain has **14 active files** totaling ~10,624 words (excluding `(old- now isa)-immigration-and-customs-enforcement-(ICE)-reform.md`)
- **ISA (Immigration Services and Administration) is the organizing concept** — replaces both ICE and USCIS with a unified service-delivery model. The ISA Execution Corps deployment model lives in Manufacturing/workforce-training-and-immigration/ (isa-execution-corps-deployment.md) as the primary manufacturing corridor instantiation; immigration-services-and-administration.md here is the institutional charter spec
- **Most files are thin (~500–1,000 words)** — the architecture is correct and the subdomains are well-defined, but prose depth is consistently Phase 2; the path to Phase 3 is deepening each subdomain brief, not adding new subdomains
- **Real-time demand signal integration** is the key Phase 4 feature — connecting manufacturing labor demand (WCA/industrial-demand-coordination-system.md) to visa activation triggers directly addresses the historical mismatch between visa supply and actual labor market conditions
- **DACA/undocumented resolution** is politically the most explosive gap — the platform doesn't have a position yet; it's a genuine pending decision, not an oversight
- **Country-based restrictions** connect directly to the National_Security domain (China Strategy, Foreign Policy) — this subdomain should be co-authored or at minimum co-reviewed with National_Security
- **Employer accountability** is the enforcement backstop that makes labor immigration honest — employers who exploit workers face escalating consequences; this connects to Labor_and_Economic_Security domain enforcement architecture
