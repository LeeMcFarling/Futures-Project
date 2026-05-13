# Domain Maturity Tracker: Healthcare

**Last Updated:** 2026-05-05
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
| Care_Delivery_and_Insurance | 4 | 7 | ~7,500 | Long-term care (known gap, flagged in SEC admin); international SEC coverage; mental health episode boundaries need more specificity | ssi-self-sovereign-identity-framework, upi-privacy-preserving-payment-rail | Prose build-out; mental health episode boundary spec | TBD |
| Care_Delivery_and_Infrastructure | 4 | 1 | ~3,500 | Long-term care integration; mental health episode boundaries in rural context | Housing_and_Public_Infrastructure | Prose build-out depth; mental health SEC episode boundary for regional center context | TBD |
| Execution_and_Transition | 4–5 | 8 | ~9,500 | State pilot cohort selection criteria; long-term care integration | department-of-data-and-accountability, public-capital-authority | Cohort selection methodology; long-term care interface | TBD |
| Pharmaceutical_Reform | 4 | 9 | ~8,000 | FDA coordination and regulatory pathway; stage-based authorization needs prose depth; regional trial infrastructure prose thin | None | Prose build-out on stage-based authorization, evidentiary sufficiency, regional trials | TBD |
| Public_Health_Nutrition | 2 | 6 | ~5,200 | Pilot program design; lighter than rest of stack | Agriculture | Add pilot selection criteria; deepen substance | TBD |
| Mental_Health | 3 | 1 | ~800 | **Crisis response covered cross-domain** (crisis-response-infrastructure.md in Social/criminal-justice-reform — Fourth Dispatch Framework, 988 integration, ZKP consent, stabilization ecosystem connections); **acute SEC coverage implicit** (psychiatric hospitalization = severe event by definition); remaining gaps: parity enforcement in direct-pay market; explicit acute/inpatient SEC trigger definition | crisis-response-infrastructure (Social domain), dental-vision-mental-health-market-integration | Parity enforcement brief; explicit acute SEC trigger language | TBD |
| Maternal_Health | 2–3 | 1 | ~4,400 | Postpartum recovery center certification spec; HTA integration prose depth; long-term care interface | care-delivery-market-design, regional-health-center-network, benefits-gradient-modernization | Postpartum certification spec; deepen HTA integration prose | TBD |
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
| Rural infrastructure | Public_Infrastructure | Phase 2 | Telehealth, access |
| Digital identity | Technology_and_Data | Phase 2 | Patient records |
| Crisis response infrastructure | Social (criminal-justice-reform) | Phase 3 | Fourth Dispatch Framework (crisis-response-infrastructure.md) covers mental health crisis dispatch, 988 integration, ZKP consent, stabilization ecosystem connections — front door to healthcare for crisis populations |

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
- [~] **Mental Health** — Market integration covered (dental/vision/mental health brief); crisis response covered cross-domain by crisis-response-infrastructure.md (Social/criminal-justice-reform — Fourth Dispatch Framework, 988, ZKP consent, stabilization ecosystem); acute psychiatric SEC coverage implicit in severe-event architecture; remaining gaps are parity enforcement in direct-pay market and explicit acute/inpatient SEC trigger definition

### Tier 2: Structural Gaps (Incomplete Coverage)
- [x] **Maternal Health** — maternal-family-care-hta-integration-v2.md (v0.1): HTA integration framework, postpartum support architecture, SEC trigger boundaries for maternal care, HETA deployment model ✅
- [x] **Rural Access** — Regional Health Center Network covers all four density tiers (urban/rural/frontier/remote), transport obligations, helipad requirements, PE exclusion, DoDA certification, PCA capital instruments ✅
- [~] **Mental Health (depth)** — Crisis response covered cross-domain: `Social/criminal-justice-reform/crisis-response-infrastructure.md` (v0.2) — Fourth Dispatch Framework (fourth 911 option), 988 dispatch integration, behavioral health clinician + peer support model, ZKP consent model (safe-to-call architecture), warm handoff to stabilization ecosystem; acute SEC coverage implicit. Remaining: parity enforcement in direct-pay market; explicit acute/inpatient SEC trigger definition — Target: Phase 4
- [ ] **Long-term care** — Elder care, nursing homes, extended disability support — correctly flagged as known gap in SEC administration doc — Target: Phase 3

### Tier 3: Enhancement Gaps (Nice-to-Have)
- [ ] **Dental/vision** – Coverage expansion – Target: Phase 3

---

## Phase Advancement Checklist

### Requirements for Phase 4 (Sequencing & Execution) — Substantially Met
- [x] Implementation timeline created (state cohort sequencing, phase gates)
- [x] Resource requirements estimated (capital recycling model, appropriation trajectory)
- [x] Coordination mechanisms defined (HETA-DoDA-PCA-state integrated deployment model)
- [x] Fallback plans documented (cost performance backstop, Type A–E escalation sequence)

### Requirements for Phase 5 (External Validation) — Active Next Step
- [ ] Prose build-out on pharma sub-briefs (stage-based authorization, evidentiary sufficiency, regional trial infrastructure)
- [x] Maternal health brief — maternal-family-care-hta-integration-v2.md (v0.1) ✅; rural access covered by Regional Health Center Network ✅
- [ ] Mental health crisis + parity framework
- [ ] Long-term care interface design
- [ ] Stress-testing against known attack lines ("socialized medicine," "government in your doctor's office," "innovation will die")

---

## Recent Activity Log

| Date | Subdomain | Change | Phase Impact |
|------|-----------|--------|--------------|
| 2026-05-05 | Maternal_Health | Added maternal-family-care-hta-integration-v2.md (v0.1, ~4,400 words): HTA integration framework for maternal and family care; postpartum support architecture; SEC trigger boundaries for prenatal/delivery/postpartum; HETA deployment model for maternal services; postpartum recovery center certification (spec TBD); closes Maternal Health Tier 2 gap | New subdomain; 31 → 32 files |
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

- Domain has **32 files** totaling ~31,500 words (plus 2 OLD-* archived files showing policy evolution)
- Architecture is more sophisticated than Medicare for All or ACA expansion — three-layer market design matches governance to economic nature of service type; neither M4A nor ACA does this
- **Cost Performance Backstop** is the most operationally detailed document in the full platform — pre-specified diagnostic types, cause-specific remedy sequences, supply-demand discipline rule as hard structural safeguard
- **HETA Revised Charter** is draft statutory language (numbered sections, enforcement firewall, reporting requirements) — not a policy brief
- **SEC Administration** includes payment routing step-by-step, provider blindness as architectural property, fraud detection taxonomy, PBM transition pathway
- **Pharma attestation** closes the enforcement gap that kills every other recoupment proposal — revenue tracked through UPI rail, costs attested under perjury obligation via SSI
- **Supply-demand discipline rule** is the key insight missing from all demand-side healthcare reforms historically: subsidies cannot precede supply adequacy certification
- Rural Access is NOT a gap — Regional Health Center Network is a detailed Phase 4 brief with four density tiers, transport/air obligations, PE exclusion, network adequacy certification
- Remaining genuine gaps: Mental Health parity enforcement + explicit acute SEC trigger definition (crisis response itself is covered cross-domain); Long-term care interface design; Maternal Health now addressed (Phase 2–3, 1 file)
- **Cross-domain architecture note:** Mental health crisis response lives in `Social/criminal-justice-reform/crisis-response-infrastructure.md` (v0.2, Phase 3) — not in this domain. Fourth Dispatch Framework (fourth 911 option alongside police/fire/EMS), 988 dispatch integration, behavioral health clinician + peer support team model, ZKP consent (safe-to-call design), warm handoff to healthcare-enabled housing and stabilization ecosystem. Healthcare domain owns the financing layer (SEC acute coverage, parity enforcement in direct-pay market); Social domain owns the dispatch and response layer. The two domains are the front door and the financing back-end of the same system.
- Nutrition stack is lighter than care delivery and pharma stacks — needs prose investment
