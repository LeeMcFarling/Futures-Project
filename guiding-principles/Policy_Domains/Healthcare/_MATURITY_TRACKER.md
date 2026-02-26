# Domain Maturity Tracker: Healthcare

**Last Updated:** 2026-02-26
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
| Care_Delivery_and_Insurance | 3 | 4 | ~3,200 | Payer transition details | Budget.Healthcare | Add transition mechanics | TBD |
| Execution_and_Transition | 3 | 6 | ~5,200 | State pilot criteria | None | Define pilot selection | TBD |
| Pharmaceutical_Reform | 3 | 8 | ~6,500 | FDA coordination | None | Add regulatory pathway | TBD |
| Public_Health_Nutrition | 2 | 5 | ~3,800 | Pilot program design | Agriculture | Add pilot selection criteria | TBD |
| Mental_Health | 0 | 0 | 0 | **Not started** | None | Create initial file | TBD |
| Maternal_Health | 0 | 0 | 0 | **Not started** | None | Create initial file | TBD |
| Rural_Access | 0 | 0 | 0 | **Not started** | Public_Infrastructure | Create initial file | TBD |

---

## Dependency Map

### Hard Dependencies (Blocking)
| This Domain Requires | From Domain | Status | Risk Level |
|---------------------|-------------|--------|------------|
| Healthcare financing model | Budget | Not started | High |

### Soft Dependencies (Coordination)
| This Domain Benefits From | From Domain | Status | Notes |
|--------------------------|-------------|--------|-------|
| Rural infrastructure | Public_Infrastructure | Phase 2 | Telehealth, access |
| Digital identity | Technology_and_Data | Phase 2 | Patient records |

### Provides To (Downstream Impact)
| Other Domain | What We Provide | Criticality |
|--------------|-----------------|-------------|
| Economic_Prosperity | Reduced employer burden | High |
| Education | Student health services | Medium |

---

## Gap Analysis

### Tier 1: Critical Gaps (Missing Foundation)
- [ ] **Mental Health** – Crisis services, parity, access – Target: Phase 2

### Tier 2: Structural Gaps (Incomplete Coverage)
- [ ] **Maternal Health** – Prenatal, delivery, postpartum – Target: Phase 2
- [ ] **Rural Access** – Telehealth, facility sustainability – Target: Phase 2

### Tier 3: Enhancement Gaps (Nice-to-Have)
- [ ] **Long-term care** – Elder care, nursing homes – Target: Phase 3
- [ ] **Dental/vision** – Coverage expansion – Target: Phase 3

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
| 2025-01-25 | All | YAML standardized, moved from People_Skills_Health | N/A |

---

## Notes & Context

- Domain has 23 files totaling ~18,700 words (largest domain)
- Most mature domain in repository
- OLD-* files show policy evolution (preserved as archived)
- Strong pharmaceutical reform coverage
- Emergency/trauma as utility model is innovative
