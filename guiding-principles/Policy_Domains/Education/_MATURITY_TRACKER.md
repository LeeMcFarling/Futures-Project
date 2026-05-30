# Domain Maturity Tracker: Education

**Last Updated:** 2026-05-30
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
Rebuild education as a system that produces capable, adaptable people — not a credentialing bureaucracy that produces compliant test-takers. K-12 redesign centers on competency-based progression, personalized learning, principal-led school autonomy, and a national competency framework that replaces the current standards morass. Higher education refocus centers on pre-seeding (research infrastructure), labor-market alignment, and converting universities from gatekeepers to genuine preparation pipelines.

**Key Questions:**
- How do we shift K-12 from age-based progression to competency-based progression without creating chaos at the school level?
- What does principal budget autonomy with accountability look like at implementation scale?
- How do we align university admissions and programs with actual labor market and national capacity needs?
- How do we connect education investment to the child future accounts (pre-seed) and manufacturing corridor workforce pipelines?

**Success Criteria:**
- National Competency Framework (NCF) deployed and DoDA-integrated
- Department of Education Standards (DES) trigger thresholds operational
- Principal budget autonomy pilot expanded to Phase 4 implementation
- Book rating + recommendation system deployed as personalization infrastructure
- Higher education pre-seeding architecture specified
- Student-based funding + campus colocation deployed in pilot jurisdictions

---

## Subdomain Status Matrix

| Subdomain | Phase | File Count | Word Count | Key Gaps | Dependencies | Next Action | Target Date |
|-----------|-------|------------|------------|----------|--------------|-------------|-------------|
| K12_Strategy | 3 | 2 | ~6,365 | Regional differentiation; rural access design | Housing_and_Public_Infrastructure | Rural access overlay; regional deployment design | TBD |
| Competency_Framework | 3 | 1 | ~2,595 | Domain-specific competency definitions; cross-state adoption pathway | department-of-data-and-accountability | Domain competency spec; adoption pathway | TBD |
| DES_and_Accountability | 3 | 2 | ~5,854 | Trigger calibration data; DoDA integration spec | department-of-data-and-accountability | DoDA integration API spec; trigger calibration | TBD |
| Personalized_Learning | 3 | 1 | ~2,886 | Teacher transition support design; pilot selection criteria | teacher-reskilling-and-role-transformation | Teacher transition spec; pilot cohort design | TBD |
| Principal_Budget_Autonomy | 3–4 | 3 | ~8,469 | Autonomy grant governance; accountability firewall design | department-of-data-and-accountability | Governance spec; accountability firewall | TBD |
| Book_Program | 3 | 3 | ~9,169 | Platform implementation; student walkthrough scale | Technology_and_Data | Platform deployment spec; scaling design | TBD |
| Teacher_Reskilling | 3 | 1 | ~4,044 | Role transition timeline; retraining certification pathway | execution-corps-spec | Transition timeline; certification pathway | TBD |
| Student_Funding_and_Colocation | 3 | 1 | ~3,308 | Per-pupil funding formula; colocation facility standards | public-capital-authority | Funding formula spec; facility standards | TBD |
| Youth_Challenge_Media | 3 | 1 | ~4,028 | Media production spec; distribution platform | Budget_and_Fiscal_Policy (child-future-accounts) | Production design; distribution spec | TBD |
| University_Admissions | 2–3 | 2 | ~5,635 | Competency-based admissions rollout; national credentialing bridge | Competency_Framework | Rollout pathway; credentialing bridge design | TBD |
| Higher_Ed_Overview | 2–3 | 2 | ~6,427 | Cross-domain interface deployment sequencing; university selection criteria | Budget_and_Fiscal_Policy (pre-seeding), IDP, national-problem-portfolio | Interface deployment spec; NPP → university linkage | TBD |
| Pre_Seeding_Research | 3 | 1 | ~3,077 | Capitalization structure; university selection criteria | public-capital-authority | Capitalization spec; selection criteria | TBD |
| Capability_Apprenticeship | 2–3 | 1 | ~4,756 | Employer compact governance; WCA demand-signal integration; community college credentialing bridge; TRAC spec | workforce-coordination-authority, community-college-network | TRAC certification design; employer compact pilot design | TBD |

---

## Dependency Map

### Hard Dependencies (Blocking)
| This Domain Requires | From Domain | Status | Risk Level |
|---------------------|-------------|--------|------------|
| Measurement backbone for DES triggers | Institutional-Modernization (DoDA) | Phase 3 | Low — DoDA spec exists |
| Child future accounts integration (youth challenge media) | Budget_and_Fiscal_Policy | Phase 3 | Low |

### Soft Dependencies (Coordination)
| This Domain Benefits From | From Domain | Status | Notes |
|--------------------------|-------------|--------|-------|
| Manufacturing workforce pipeline | Manufacturing (WCA, ISA) | Phase 3 | Education feeds manufacturing corridor workforce |
| Student health services | Healthcare | Phase 4 | School-based health integration |
| Immigration talent retention | Immigration | Phase 2–3 | University → industry pipeline |
| NCT → Execution Corps pipeline | Institutional-Modernization (Civic_Formation) | Phase 3 | Education is the early stage of the civic competence pipeline |

### Provides To (Downstream Impact)
| Other Domain | What We Provide | Criticality |
|--------------|-----------------|-------------|
| Manufacturing | Workforce pipeline — competency-credentialed workers ready for corridors | High |
| Labor_and_Economic_Security | Worker quality baseline; ISA integration | High |
| Immigration | Student-to-industry pathway | Medium |
| Institutional-Modernization | Early civic formation stage (education → NCT → Execution Corps) | High |

---

## Gap Analysis

### Tier 1: Critical Gaps (Missing Foundation)
- [x] **National Competency Framework** — national-competency-framework.md: competency domains, progression architecture, DoDA integration ✅
- [x] **DES trigger thresholds** — des-trigger-thresholds-and-intervention-protocol.md: accountability trigger architecture, intervention escalation ✅
- [x] **Principal budget autonomy** — principal-budget-autonomy-pilot.md + principal-budget-autonomy-counterfactual.md: pilot design, counterfactual methodology ✅
- [x] **Personalized learning reform** — personalized-education-reform.md: competency-based progression, adaptive learning architecture ✅
- [x] **Book rating + recommendation** — book-rating-system.md + book-recommendation-pilot.md + book-recommendation-student-walkthroughs.md: information diet infrastructure, discovery platform ✅
- [x] **Teacher reskilling** — teacher-reskilling-and-role-transformation.md: role transformation (teacher → learning architect), retraining pathway ✅
- [x] **Student-based funding + colocation** — student-based-funding-and-campus-colocation.md: per-pupil portability, campus colocation model ✅
- [x] **Youth challenge media** — youth-challenge-media-child-future-accounts.md: media production connecting child future accounts to youth aspiration ✅

### Tier 2: Structural Gaps (Incomplete Coverage)
- [x] **University admissions alignment** — university-admissions-competency-alignment.md: competency-based admissions, NCF bridge ✅ (2 versions; k-12/ version is more complete)
- [ ] **Higher education pre-seeding capitalization** — pre-seeding.md has architecture (~3,077 words); capitalization structure and university selection criteria not specified — Target: Phase 4
- [ ] **Rural and frontier education access** — no brief on applying competency/personalized learning architecture to rural/frontier contexts — Target: Phase 3
- [ ] **Special education and disability access** — no brief on how NCF + personalized learning applies to students with disabilities — Target: Phase 3

### Tier 3: Enhancement Gaps (Nice-to-Have)
- [~] **Vocational and trade pathway** – capability-apprenticeship-compact-v0.1.md (v0.1, ~4,756 words): WCA-coordinated, employer-anchored, community-college-credentialed pathway from high school senior year through Associate; TRAC certification; employer compact governance still TBD — Target: Phase 3
- [ ] **Early childhood** – Pre-K and childcare integration with NCF and child future accounts – Target: Phase 4

---

## Phase Advancement Checklist

### Requirements for Phase 4 (Sequencing & Execution)
- [x] K-12 reform architecture complete (NCF, DES, principal autonomy, personalized learning, teacher reskilling, student funding/colocation, book program, youth media) ✅
- [ ] Principal budget autonomy pilot cohort selected
- [ ] DES trigger calibration data and DoDA integration spec
- [ ] Pre-seeding capitalization structure and university selection criteria
- [ ] Rural access overlay
- [ ] Stress-testing against attack lines ("federal curriculum control," "replacing teachers with computers," "destroying public schools")

---

## Recent Activity Log

| Date | Subdomain | Change | Phase Impact |
|------|-----------|--------|--------------|
| 2026-05-30 | Higher_Ed | university-cross-domain-interfaces-v0.2.md (v0.2, ~3,970 words): maps what universities become in AI era — institutional anchor for public/private/university capital on hard long-horizon problems; interfaces to defense (DARPA-style discovery units), energy, agriculture, NPP open competitive architecture; crowding-in model; v0.2 restructured to lead with structural challenges universities face today | Higher_Ed_Overview: 1 → 2 files |
| 2026-05-30 | Higher_Ed | capability-apprenticeship-compact-v0.1.md (v0.1, ~4,756 words): WCA-coordinated employer-anchored community-college-credentialed pathway from HS senior year through Associate degree; braids paid work with credentialed instruction; TRAC certification; closes vocational/trade pathway Tier 3 gap | New subdomain: Capability_Apprenticeship |
| 2026-05-16 | All | Tracker updated: file count updated to 18 active; phase 2 → 3; k-12 stack recognized as complete Phase 3; word counts updated | N/A |
| 2026-03-15 | K12 | youth-challenge-media-child-future-accounts.md added; teacher-reskilling-and-role-transformation.md (~4,044 words); student-based-funding-and-campus-colocation.md (~3,308); book-recommendation-student-walkthroughs.md; department-of-education-standards.md (~2,539); principal-budget-autonomy-counterfactual.md | New |
| 2026-03-12 | K12 | national-competency-framework.md added (~2,595); education-reform-distillate.md | New |
| 2026-01-28 | All | YAML standardized, k-12/ and university/ subfolder structure created | N/A |
| 2025-01-25 | All | Domain created, initial files added | N/A |

---

## Notes & Context

- Domain has **15 active k-12 files** (~46,994 words) + **5 university files** (~15,485 words) = **20 active files** in subdirectories (~62,479 words); root also has 8 older/duplicate files (~7,204 words) that are pre-subfolder versions
- **K-12 stack is the most complete education subdomain** — NCF, DES triggers, principal autonomy, personalized learning, teacher reskilling, student funding/colocation, book program, youth media all specified; this is a comprehensive Phase 3 K-12 redesign
- **Book program (3 files, ~9,169 words) is the largest subdomain** — the personalized reading discovery infrastructure addresses information diet and is one of the platform's most operationally concrete instruments (it has student walkthrough examples)
- **Youth challenge media + child future accounts** is the Budget ↔ Education connection — pre-seed activation is partly an education intervention (showing young people the compound math and what it means for their futures)
- **Teacher reskilling is the most politically sensitive K-12 file** — honest about role transformation (teacher as learning architect, not content deliverer); union reaction will be hostile; needs political strategy before Phase 5
- **University stack is underdeveloped relative to K-12** — pre-seeding and admissions alignment are defined but thin; the AI outline draft in university/ folder explicitly notes this
- **Root-level files are mostly older versions** of k-12 files — not the canonical versions; those live in k-12/ subfolder; root versions can be archived
- **Education → Manufacturing pipeline** is the platform's workforce answer: NCF competencies → ISA/WCA demand matching → corridor jobs; this loop runs through Education, Manufacturing, and Immigration simultaneously
