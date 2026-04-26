# Domain Maturity Tracker: Immigration

**Last Updated:** 2026-04-25
**Overall Domain Phase:** 3–4
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
Create a coherent immigration system that aligns legal immigration with labor market needs, maintains strict asylum/labor separation, ensures border security, and enables integration.

**Key Questions:**
- How do we match immigration to actual labor market needs?
- What enforcement mechanisms work without humanitarian crisis?
- How do we process asylum claims efficiently and fairly?

**Success Criteria:**
- Labor immigration tied to employer accountability
- Asylum processed separately from economic migration
- Transparent metrics and oversight dashboards

---

## Subdomain Status Matrix

| Subdomain | Phase | File Count | Word Count | Key Gaps | Dependencies | Next Action | Target Date |
|-----------|-------|------------|------------|----------|--------------|-------------|-------------|
| System_Architecture | 3 | 1 | ~900 | Phased rollout detail | None | Prose build-out | TBD |
| Labor_Immigration | 3 | 2 | ~1,400 | Visa category specifics | Economic_Prosperity.Labor_Mobility | Prose build-out | TBD |
| Asylum | 3 | 1 | ~700 | Processing capacity plan | None | Prose build-out | TBD |
| Border_Security | 3 | 1 | ~600 | Technology integration specs | Technology_and_Data | Prose build-out | TBD |
| Enforcement | 3 | 2 | ~1,200 | ICE accountability depth | None | Prose build-out | TBD |
| Integration | 3 | 1 | ~600 | Civic program pathway detail | Education | Prose build-out | TBD |
| Oversight | 3 | 1 | ~700 | DoDA dashboard spec depth | Technology_and_Data | Prose build-out | TBD |
| Entrepreneurship | 3 | 1 | ~600 | Conversion pathway details | Economic_Prosperity.Labor_Mobility | Prose build-out | TBD |
| Student_Retention | 3 | 1 | ~560 | Industry pathway details | Education | Prose build-out | TBD |
| DACA_Resolution | — | — | — | *Cross-domain: tracked under Social (pathway for existing undocumented residents including DACA recipients)* | Social | See Social tracker | — |
| Citizenship_Backlog | — | — | — | *Cross-domain: tracked under Social (processing backlog resolution for existing applicants)* | Social | See Social tracker | — |

---

## Dependency Map

### Hard Dependencies (Blocking)
| This Domain Requires | From Domain | Status | Risk Level |
|---------------------|-------------|--------|------------|
| Labor market data | Economic_Prosperity | Phase 2 | Medium |

### Soft Dependencies (Coordination)
| This Domain Benefits From | From Domain | Status | Notes |
|--------------------------|-------------|--------|-------|
| Digital identity | Technology_and_Data | Phase 2 | Visa tracking |
| Education integration | Education | Phase 2 | Immigrant education |

### Provides To (Downstream Impact)
| Other Domain | What We Provide | Criticality |
|--------------|-----------------|-------------|
| Economic_Prosperity | Workforce supply | High |
| National_Security | Border security framework | High |

---

## Gap Analysis

### Tier 1: Critical Gaps (Missing Foundation)
- [x] **DACA Resolution** — Cross-domain: tracked under Social (pathway for existing undocumented residents including DACA recipients) ✅
- [x] **Citizenship Backlog** — Cross-domain: tracked under Social (processing backlog resolution) ✅

### Tier 2: Structural Gaps (Incomplete Coverage)
- [ ] **Family Reunification** — Policy on family-based immigration categories — Target: Phase 3
- [ ] **Country-specific strategies** — Bilateral labor agreements, partnership frameworks beyond restriction — Target: Phase 3

### Tier 3: Enhancement Gaps (Nice-to-Have)
- [ ] **Prose depth** — All subdomains at Phase 3; full system ready for Phase 5–6 messaging and rebuttal build-out — Active next step

---

## Phase Advancement Checklist

### Requirements for Phase 3 (Outcomes & Decision Rules) — Substantially Met
- [x] Clear success metrics defined (employer accountability, asylum/labor separation, oversight dashboards)
- [x] Decision criteria established (labor market triggers, enforcement thresholds)
- [x] Risk mitigation strategies documented (enforcement accountability, SSI/UPI accelerants)
- [x] Monitoring framework designed (Oversight subdomain, DoDA integration)

### Requirements for Phase 5 (External Validation) — Active Next Step
- [ ] Prose build-out across all 9 subdomains
- [ ] Attack-line stress testing (enforcement vs. humanitarian, labor displacement objections)
- [ ] Rebuttal language drafted for common objections
- [ ] Family Reunification subdomain initiated

---

## Recent Activity Log

| Date | Subdomain | Change | Phase Impact |
|------|-----------|--------|--------------|
| 2026-04-25 | All | Advanced all 9 subdomain phases 2 → 3; DACA_Resolution and Citizenship_Backlog closed as standalone subdomains — both tracked under Social domain; overall domain phase advanced 2 → 3–4; prose build-out (Phase 5–6) flagged as active next step | 2 → 3–4 |
| 2026-04-10 | Cross-domain note | immigration-services-and-administration.md and workforce-immigration-skill-mobility-system.md added to Immigration folder but declare domain: Economic_Prosperity, subdomain: Labor_Mobility — tracked under Economic_Prosperity/Labor_Mobility | N/A |
| 2026-02-26 | All | SSI/UPI accelerants added to 6 immigration files | N/A |
| 2025-01-25 | All | YAML standardized, moved from People_Skills_Health | N/A |

---

## Notes & Context

- Domain has **11 files** totaling ~7,560 words (plus 2 cross-domain files in folder, tracked under Economic_Prosperity/Labor_Mobility)
- Comprehensive system-level architecture across 9 subdomains — all at Phase 3
- Strong on labor/asylum separation principle; SSI/UPI accelerants integrated throughout
- DACA Resolution and Citizenship Backlog: tracked under Social domain — not immigration architecture gaps
- Active next step: Phase 5–6 prose build-out; all core policy decisions made, needs external validation layer and rebuttal messaging
- Family Reunification is the only substantive policy gap remaining at this stage
