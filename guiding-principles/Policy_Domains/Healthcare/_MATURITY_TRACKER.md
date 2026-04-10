# Domain Maturity Tracker: Healthcare

**Last Updated:** 2026-04-10
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
Create a healthcare system with transparent pricing, competitive markets for routine care, utility-regulated emergency services, and reformed pharmaceutical development/pricing.

**Key Questions:**
- How do we create price transparency without disrupting care access?
- What regulatory model works for emergency services as utility?
- How do we reform drug pricing while preserving innovation?

**Success Criteria:**
- Transparent, competitive markets for routine care
- Emergency/trauma services operate as regulated utility
- Drug pricing tied to recoupment with cost-plus transition

---

## Subdomain Status Matrix

| Subdomain | Phase | File Count | Word Count | Key Gaps | Dependencies | Next Action | Target Date |
|-----------|-------|------------|------------|----------|--------------|-------------|-------------|
| Care_Delivery_and_Insurance | 3 | 7 | ~7,500 | Payer transition details | Budget.Healthcare | Add transition mechanics | TBD |
| Care_Delivery_and_Infrastructure | 3 | 1 | ~1,800 | Rural facility density; telehealth integration | Housing_and_Public_Infrastructure | Expand facility siting criteria | TBD |
| Execution_and_Transition | 3 | 8 | ~9,500 | State pilot selection criteria; cost glide-path validation | DoDA, DepartmentOfData | Define pilot selection; finalize glide-path thresholds | TBD |
| Pharmaceutical_Reform | 3 | 9 | ~8,000 | FDA coordination | None | Add regulatory pathway | TBD |
| Public_Health_Nutrition | 2 | 6 | ~5,200 | Pilot program design | Agriculture | Add pilot selection criteria | TBD |
| Mental_Health | 3 | 1 | ~800 | Crisis services, parity, access depth — partially covered via Care_Delivery_and_Insurance | None | Add standalone mental health crisis + parity framework | TBD |
| Maternal_Health | 0 | 0 | 0 | **Not started** | None | Create initial file | TBD |
| Rural_Access | 0 | 0 | 0 | **Not started** | Housing_and_Public_Infrastructure | Create initial file | TBD |

---

## Dependency Map

### Hard Dependencies (Blocking)
| This Domain Requires | From Domain | Status | Risk Level |
|---------------------|-------------|--------|------------|
| Healthcare financing model | Budget | Not started | High |

### Soft Dependencies (Coordination)
| This Domain Benefits From | From Domain | Status | Notes |
|--------------------------|-------------|--------|-------|
| Rural infrastructure | Housing_and_Public_Infrastructure | Phase 3 | Telehealth, access; healthcare-enabled housing pilot active |
| Digital identity | Technology_and_Data | Phase 2 | Patient records |

### Provides To (Downstream Impact)
| Other Domain | What We Provide | Criticality |
|--------------|-----------------|-------------|
| Economic_Prosperity | Reduced employer burden | High |
| Education | Student health services | Medium |

---

## Gap Analysis

### Tier 1: Critical Gaps (Missing Foundation)
- [~] **Mental Health** – Market integration covered via dental-vision-mental-health-market-integration.md; crisis services and parity depth still needed

### Tier 2: Structural Gaps (Incomplete Coverage)
- [ ] **Maternal Health** – Prenatal, delivery, postpartum – Target: Phase 2
- [ ] **Rural Access** – Telehealth, facility sustainability – Target: Phase 2
- [ ] **Mental Health (depth)** – Standalone crisis services, parity enforcement, access framework – Target: Phase 3

### Tier 3: Enhancement Gaps (Nice-to-Have)
- [ ] **Long-term care** – Elder care, nursing homes – Target: Phase 3

---

## Phase Advancement Checklist

### Requirements for Phase 4 (Sequencing & Execution)
- [ ] Implementation timeline created
- [ ] Resource requirements estimated
- [ ] Coordination mechanisms defined
- [ ] Fallback plans documented

---

## Recent Activity Log

| Date | Subdomain | Change | Phase Impact |
|------|-----------|--------|--------------|
| 2026-04-10 | Care_Delivery_and_Insurance | Added sec-administration-heta-steady-state.md (SEC Administration — HETA Steady-State Operating Model; lives in Care-Delivery folder, subdomain Execution_and_Transition); dep HETA-revised-charter case fixed to heta-revised-charter | 6 → 7 files |
| 2026-04-10 | Pharmaceutical_Reform | Added pharmaceutical-cost-attestation-anti-gaming.md (cost attestation + anti-gaming enforcement framework; subdomain fixed Pharmaceuticals → Pharmaceutical_Reform) | 8 → 9 files |
| 2026-03-29 | Public_Health_Nutrition | Added national-health-month-and-food-legibility-campaign.md (fall public activation: national health month + school procurement pilot announcements + ingredient disclosure rollout bundled as single seasonal campaign); YAML overhauled from legacy typed-dependency format to standard slug list | 5 → 6 files |
| 2026-03-23 | Care_Delivery_and_Insurance | dental-vision-mental-health-market-integration.md added: SEC trigger boundaries for dental/vision/outpatient mental health, optional discount wrap, UPI price display requirement | 3 → 3 (deepened) |
| 2026-03-23 | Care_Delivery_and_Infrastructure | regional-health-center-network.md added (new subdomain): federally backstopped contractor-operated network; population density coverage standard; network adequacy as closure gate for legacy subsidies | 0 → 3 |
| 2026-03-23 | Execution_and_Transition | HETA-revised-charter.md added (v0.2): Provider Transition Corps, regional office model, enforcement firewall; cost-performance-backstop.md added: DoDA-triggered escalation framework, healthcare cost glide path, state sequencing + capital recycling model | 6 → 8 files; deepened to Phase 4-adjacent |
| 2026-03-23 | Execution_and_Transition | healthcare-transition-phase-strategy.md YAML standardized (id, domain, slug, slugified dependencies) | N/A |
| 2026-02-26 | Care_Delivery_and_Insurance, Execution_and_Transition, Pharmaceutical_Reform | SSI/UPI accelerants added to 4 files | N/A |
| 2026-03-12 | All | Public_Infrastructure reference updated to Housing_and_Public_Infrastructure | N/A |
| 2025-01-25 | All | YAML standardized, moved from People_Skills_Health | N/A |

---

## Notes & Context

- Domain has **31 files** totaling ~27,100 words
- Most mature domain in repository — Execution_and_Transition now approaching Phase 4 with HETA revised charter + cost backstop + DoDA telemetry
- OLD-* files show policy evolution (preserved as archived)
- Strong pharmaceutical reform coverage
- Emergency/trauma as utility model is innovative
- New Care_Delivery_and_Infrastructure subdomain created for Regional Health Center Network
