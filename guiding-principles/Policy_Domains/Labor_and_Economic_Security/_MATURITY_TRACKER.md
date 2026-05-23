# Domain Maturity Tracker: Labor_and_Economic_Security

**Last Updated:** 2026-05-19
**Overall Domain Phase:** 4–5
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
Fix the structural failures that divorced American workers from the productivity gains of the economy they built — through wage restoration, benefits continuity, income smoothing, credential mobility, worker governance, and portable wealth formation. Each instrument does useful work independently; the full stack becomes dramatically more powerful when SSI, UPI, IRS modernization, and DoDA heatmap are live.

**Key Questions:**
- How do we guarantee every earned dollar leaves a household ahead (benefits cliff elimination)?
- How do we make work credentials portable without rebuilding the licensing system from scratch?
- How do we give workers formal standing in the decisions that determine their economic futures?

**Success Criteria:**
- Benefits gradient: zero households worse off for earning more across the federal stack
- Regional wage pilot: evidence-gated rollout with DoDA-certified evaluation before expansion
- Worker classification parity: dependent contractor arbitrage closed; payroll contributions normalized
- Real-time EITC/CTC delivery: annual lump-sum replaced with continuous income stabilization
- Credential portability: SSI-backed verification eliminates state-line licensing limbo
- Codetermination: worker board seats at PCA-covered firms from Day 1; size-based mandate phased in over 5 years
- Superannuation contributions: portable across employers and classifications; gig/part-time workers covered

---

## Subdomain Status Matrix

| Subdomain | Phase | File Count | Word Count (est.) | Key Gaps | Dependencies | Next Action | Target Date |
|-----------|-------|------------|-------------------|----------|--------------|-------------|-------------|
| Domain_Overview | 4 | 1 | ~3,500 | — | SSI, UPI, IRS modernization, DoDA heatmap | Prose complete ✅ | — |
| Wage_Modernization | 3 | 1 | ~4,000 | YAML modernization needed; sidebar_position missing; v0.1 | doda-regional-wage-heatmap, public-capital-authority | Fix YAML to domain standard | TBD |
| Income_Support | 4 | 1 | ~3,000 | — | doda-regional-wage-heatmap, healthcare-reform-sec-architecture | Prose complete ✅ | — |
| Labor_Market_Integrity | 4 | 1 | ~2,500 | — | irs-modernization-automated-income-attestation | Prose complete ✅ | — |
| Healthcare_Transition | 4 | 1 | ~3,000 | — | healthcare-reform-sec-architecture, benefits-gradient-modernization | Prose complete ✅ | — |
| Income_Smoothing | 4 | 1 | ~2,500 | — | irs-modernization-automated-income-attestation, upi-privacy-preserving-payment-rail | Prose complete ✅ | — |
| Worker_Governance | 4 | 1 | ~3,500 | Anti-capture legislative pathway; NLRA relationship | public-capital-authority, credential-portability | Prose complete ✅ | — |
| Wealth_Building | 4 | 1 | ~2,000 | — | universal-superannuation-system, worker-classification-parity | Prose complete ✅ | — |
| Public_Facing | 5 | 1 | ~2,500 | — | All stack instruments | Employer letter complete ✅ | — |
| Enforcement | 3–4 | 1 | ~3,159 | Enforcement agency home (FTC/NLRB/DoD?); penalty escalation calibration; whistleblower spec | department-of-data-and-accountability, immutable-government-ledger | Enforcement agency determination; whistleblower framework | TBD |
| Workforce_Transition | 3–4 | 1 | ~2,719 | Rural deployment; Social domain cross-ref integration; pilot selection criteria | housing-workforce-stabilization-pilots, benefits-gradient-modernization | Pilot cohort selection; rural access spec | TBD |

---

## Cross-Domain Files in This Folder

| File | Declared Domain | Declared Subdomain | Notes |
|------|-----------------|--------------------|-------|
| credential-portability-and-competency-recognition.md | Economic_Prosperity | Labor_Mobility | Lives here; tracked under Economic_Prosperity/Labor_Mobility |

---

## Dependency Map

### Hard Dependencies (Blocking)
| This Domain Requires | From Domain | Status | Risk Level |
|---------------------|-------------|--------|------------|
| SSI credential infrastructure | Technology_and_Data | Phase 3 | Medium — pilots work without it; full capability requires it |
| UPI payment rail | Technology_and_Data | Phase 3 | Medium — HTA and real-time EITC need it for full operation |
| IRS modernization / income attestation | Economic_Prosperity/Budget_and_Fiscal | Phase 3–4 | Medium — real-time credit delivery and benefits gradient calibration depend on it |
| DoDA regional wage/cost heatmap | Institutional_Modernization | Phase 3 | Medium — wage pilot evaluation and benefits gradient calibration |

### Soft Dependencies (Coordination)
| This Domain Benefits From | From Domain | Status | Notes |
|--------------------------|-------------|--------|-------|
| Severe Event Coverage (SEC) architecture | Healthcare | Phase 3 | Benefits gradient Medicaid bridge destination |
| Housing supply stack | Housing | Phase 2–3 | Workforce stabilization exit pathways |
| Manufacturing credential pathways | Economic_Prosperity/Manufacturing | Phase 3 | IDP alliance credentialing uses same SSI infrastructure |

### Provides To (Downstream Impact)
| Other Domain | What We Provide | Criticality |
|--------------|-----------------|-------------|
| Economic_Prosperity | Wage floor stabilization, labor cost predictability, workforce mobility | High |
| Healthcare | Medicaid bridge design, portable HTA contributions, worker financial stability | High |
| Housing | Stable income = stable housing; STZ corridor workforce pipeline | High |
| Manufacturing / IDP | Credential portability for domestic and allied-nation workforce | Medium |

---

## Gap Analysis

### Tier 1: Critical Gaps (Missing Foundation)
- [x] **Wage restoration** — Regional Wage Modernization Pilot: evidence-gated, commuting-zone calibrated, PCA-backstopped ✅
- [x] **Benefits cliff elimination** — Benefits Gradient Modernization Act: 60-cent floor, regional calibration, Medicaid bridge ✅
- [x] **Worker classification** — Dependent contractor arbitrage closed; payroll contribution parity ✅
- [x] **Income smoothing** — Real-time EITC/CTC delivery: replaces annual lump-sum with continuous stabilization ✅
- [x] **Worker governance** — Codetermination: 1/3 board seats, scoped authority over automation/restructuring/productivity gains ✅

### Tier 2: Structural Gaps (Incomplete Coverage)
- [x] **Workforce stabilization pilots** — workforce-stabilization-pilot.md: transitional housing/workforce integration for people who've fallen out of the labor market; cross-domain with Social/Homelessness stack ✅
- [x] **Anti-regressive enforcement** — labor-stack-enforcement-framework-v0.2.md: penalty architecture, audit triggers, SSI/UPI/IGL enforcement infrastructure ✅ (enforcement agency home still TBD)
- [ ] **NLRA / union policy relationship** — How does codetermination interact with existing collective bargaining rights? Codetermination brief is silent on NLRA — Target: Phase 3
- [ ] **Enforcement agency home** — labor-stack-enforcement-framework-v0.2.md names DoDA as coordinator but doesn't determine primary enforcement home (FTC/NLRB/new entity) — Target: Phase 4

### Tier 3: Enhancement Gaps (Nice-to-Have)
- [ ] **Sectoral bargaining / regional wage councils** — Referenced in credential portability as a related initiative; no standalone brief — Target: Phase 3
- [ ] **Automation/AI transition fund** — Codetermination creates worker standing but no dedicated transition capital for AI displacement — Target: Phase 3
- [ ] **Gig worker organizing infrastructure** — Classification parity closes the cost arbitrage but doesn't address collective voice for independent workers — Target: Phase 3

---

## Phase Advancement Checklist

### Requirements for Phase 5 (External Validation) — Active Next Step
- [x] Full instrument stack documented and sequenced (overview v0.3 complete)
- [x] Employer-facing communication drafted (employer letter v0.3)
- [x] Workforce stabilization brief developed (workforce-stabilization-pilot.md v0.2) ✅
- [x] Enforcement architecture defined (labor-stack-enforcement-framework-v0.2.md) ✅
- [ ] Worker-facing communication / plain-language summaries
- [ ] Attack-line stress testing: union displacement objections; small business burden; codetermination legislative pathway challenges
- [ ] Rebuttal language drafted for: "this will kill jobs", "government interference in private firms", "this is socialism"
- [ ] NLRA relationship clarified in codetermination brief
- [ ] Enforcement agency home determined

---

## YAML Issues Log

| File | Issue | Priority |
|------|-------|----------|
| regional-wage-modernization-pilot.md | Old YAML format: domain `"Labor, Wages, and Economic Security"` (wrong); missing id, sidebar_position, subdomain, slug, author, tags in standard format | High |
| worker-classification-partity.md | Filename typo: "partity" should be "parity" | Low — functional, may affect slug/link |

---

## Recent Activity Log

| Date | Subdomain | Change | Phase Impact |
|------|-----------|--------|--------------|
| 2026-05-19 | Enforcement, Workforce_Transition | Tracker updated: 2 new files added (labor-stack-enforcement-framework-v0.2.md ~3,159 words; workforce-stabilization-pilot.md ~2,719 words); file count 10 → 12; both Tier 2 gaps closed; enforcement agency home still TBD | 2 Tier 2 gaps closed |
| 2026-04-27 | All | Full prose build-out completed: benefits-gradient-modernization v0.4, worker-classification-partity v0.4, portable-healthcare-contribution-floor v1.0, earned-income-and-child-tax-credit v0.4, codetermination v0.5, superannuation-employer-contribution-portability v0.3, employer-letter v0.3; domain-overview updated to v0.3 with full layered architecture and sequencing | Domain established at Phase 4–5 |

---

## Notes & Context

- New standalone domain — previously labor/welfare content was loosely tracked under Economic_Prosperity/Labor_and_Wellfare (4 files, ~3,500 words, Phase 2); that subdomain has now been superseded
- **12 files total** (~39,868 words); 11 declare Labor_and_Economic_Security domain; 1 cross-domain (credential portability — Economic_Prosperity/Labor_Mobility)
- **Two new subdomains added since April 27**: Enforcement (labor-stack-enforcement-framework-v0.2.md) closes the anti-regressive enforcement Tier 2 gap; Workforce_Transition (workforce-stabilization-pilot.md) closes the workforce stabilization gap with cross-domain bridge to Social/Homelessness
- Employer letter at Phase 5 — external stakeholder communication already drafted, which is ahead of most domains
- Full stack architecture explicitly designed with two-phase capability: pilots and policy reforms deployable now; full capability unlocked when SSI/UPI/IRS modernization/DoDA come online
- Codetermination is the capstone instrument — governance layer that none of the other instruments reach; scoped deliberately to avoid NLRA conflicts but that relationship needs explicit treatment
- Healthcare_Transition subdomain (portable healthcare contribution floor, v1.0) is the most mature individual instrument by version number
- Wage_Modernization subdomain (regional-wage-modernization-pilot.md) needs YAML standardization — currently uses old non-standard format
