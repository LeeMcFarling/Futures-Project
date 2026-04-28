# Domain Maturity Tracker: Healthcare

**Last Updated:** 2026-04-27
**Overall Domain Phase:** 4
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
Restructure the cost architecture of American healthcare through a three-layer market design (utility regulation for emergency/trauma, direct-pay competitive markets for routine care, event-based universal insurance for severe events), a complete pharmaceutical reform stack (PCA de-risking, recoupment-bound pricing, PBM elimination of spread pricing, perjury-backed cost attestation), and a phased execution architecture (HETA, state cohort sequencing, capital recycling, DoDA-triggered cost backstop).

**Key Questions:**
- How do we create price transparency without disrupting care access?
- What regulatory model works for emergency services as utility?
- How do we reform drug pricing while preserving innovation incentives?
- How does the system respond when cost reduction targets aren't met on schedule?

**Success Criteria:**
- Transparent, competitive markets for routine care; insurance excluded from primary and urgent care
- Emergency/trauma services operating under regulated rate bands with explicit readiness funding
- Universal SEC enrollment producing national actuarial reference class
- Drug pricing through recoupment-bound model with automatic cost-plus step-down
- HETA Provider Transition Corps deployed with enforcement firewall operational
- DoDA supply adequacy certification gating all enforcement phase advances
- Cost Performance Backstop pre-specified and DoDA-measurable before rollout begins

---

## Subdomain Status Matrix

| Subdomain | Phase | File Count | Word Count | Key Gaps | Dependencies | Next Action | Target Date |
|-----------|-------|------------|------------|----------|--------------|-------------|-------------|
| Care_Delivery_and_Insurance | 4 | 7 | ~7,500 | Long-term care (known gap, flagged in SEC admin); international SEC coverage; mental health episode boundaries need more specificity | ssi-self-sovereign-identity-framework, upi-privacy-preserving-payment-rail | Prose build-out; mental health episode boundary spec | TBD |
| Care_Delivery_and_Infrastructure | 4 | 1 | ~3,500 | Long-term care integration; mental health episode boundaries in rural context | Housing_and_Public_Infrastructure | Prose build-out depth; mental health SEC episode boundary for regional center context | TBD |
| Execution_and_Transition | 4–5 | 8 | ~9,500 | State pilot cohort selection criteria; long-term care integration | department-of-data-and-accountability, public-capital-authority | Cohort selection methodology; long-term care interface | TBD |
| Pharmaceutical_Reform | 4 | 9 | ~8,000 | FDA coordination and regulatory pathway; stage-based authorization needs prose depth; regional trial infrastructure prose thin | None | Prose build-out on stage-based authorization, evidentiary sufficiency, regional trials | TBD |
| Public_Health_Nutrition | 2 | 6 | ~5,200 | Pilot program design; lighter than rest of stack | Agriculture | Add pilot selection criteria; deepen substance | TBD |
| Mental_Health | 3 | 1 | ~800 | Crisis services standalone; parity enforcement; SEC episode boundary definition for MH/SUD | None | Standalone mental health crisis + parity framework | TBD |
| Maternal_Health | 0 | 0 | 0 | **Not started** | None | Create initial file | TBD |
| Rural_Access | 4 | — | — | *Covered by Regional Health Center Network: four density tiers (urban/rural/frontier/remote), transport obligations, helicopter pad requirements, PE exclusion, DoDA network adequacy certification, PCA capital instruments* | Housing_and_Public_Infrastructure | Prose depth; telehealth integration detail | TBD |

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
- [x] **Three-layer market architecture** — utility (emergency/trauma), direct-pay market (routine care), SEC insurance (severe events) — fully designed ✅
- [x] **Pharmaceutical reform stack** — PCA de-risking, recoupment-bound pricing, PBM reform, cost attestation & anti-gaming, stage-based authorization ✅
- [x] **Execution architecture** — HETA revised charter (draft statutory language), HETA steady-state operating model, cost performance backstop, state sequencing + capital recycling ✅
- [~] **Mental Health** — Market integration covered (dental/vision/mental health brief); crisis services and parity enforcement depth still needed

### Tier 2: Structural Gaps (Incomplete Coverage)
- [ ] **Maternal Health** — Prenatal, delivery, postpartum — Target: Phase 2
- [x] **Rural Access** — Regional Health Center Network covers all four density tiers (urban/rural/frontier/remote), transport obligations, helipad requirements, PE exclusion, DoDA certification, PCA capital instruments ✅
- [ ] **Mental Health (depth)** — Standalone crisis services, parity enforcement, SEC episode boundary for MH/SUD — Target: Phase 3
- [ ] **Long-term care** — Elder care, nursing homes, extended disability support — correctly flagged as known gap in SEC administration doc — Target: Phase 3

### Tier 3: Enhancement Gaps (Nice-to-Have)
- [ ] **International SEC coverage** — American citizens receiving emergency care abroad — Target: Phase 3
- [ ] **Nutrition stack prose depth** — Ingredient disclosure, food research track, vertical farms are conceptually solid but lighter than care delivery and pharma stacks — Target: Phase 3

---

## Phase Advancement Checklist

### Requirements for Phase 4 (Sequencing & Execution) — Substantially Met
- [x] Implementation timeline created (state cohort sequencing, phase gates)
- [x] Resource requirements estimated (capital recycling model, appropriation trajectory)
- [x] Coordination mechanisms defined (HETA-DoDA-PCA-state integrated deployment model)
- [x] Fallback plans documented (cost performance backstop, Type A–E escalation sequence)

### Requirements for Phase 5 (External Validation) — Active Next Step
- [ ] Prose build-out on pharma sub-briefs (stage-based authorization, evidentiary sufficiency, regional trial infrastructure)
- [ ] Maternal health and rural access standalone briefs
- [ ] Mental health crisis + parity framework
- [ ] Long-term care interface design
- [ ] Stress-testing against known attack lines ("socialized medicine," "government in your doctor's office," "innovation will die")

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

- Domain has **31 files** totaling ~27,100 words (plus 2 OLD-* archived files showing policy evolution)
- Architecture is more sophisticated than Medicare for All or ACA expansion — three-layer market design matches governance to economic nature of service type; neither M4A nor ACA does this
- **Cost Performance Backstop** is the most operationally detailed document in the full platform — pre-specified diagnostic types, cause-specific remedy sequences, supply-demand discipline rule as hard structural safeguard
- **HETA Revised Charter** is draft statutory language (numbered sections, enforcement firewall, reporting requirements) — not a policy brief
- **SEC Administration** includes payment routing step-by-step, provider blindness as architectural property, fraud detection taxonomy, PBM transition pathway
- **Pharma attestation** closes the enforcement gap that kills every other recoupment proposal — revenue tracked through UPI rail, costs attested under perjury obligation via SSI
- **Supply-demand discipline rule** is the key insight missing from all demand-side healthcare reforms historically: subsidies cannot precede supply adequacy certification
- Rural Access is NOT a gap — Regional Health Center Network is a detailed Phase 4 brief with four density tiers, transport/air obligations, PE exclusion, network adequacy certification
- Remaining genuine gaps: Maternal Health (Phase 0), Mental Health crisis services + parity depth, Long-term care interface design
- Nutrition stack is lighter than care delivery and pharma stacks — needs prose investment
