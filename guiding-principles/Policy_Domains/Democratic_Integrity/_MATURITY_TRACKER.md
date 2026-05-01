# Domain Maturity Tracker: Democratic_Integrity

**Last Updated:** 2026-05-01
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
Strengthen democratic institutions against corruption, ensure fair representation, and modernize governance mechanisms for accountability and responsiveness.

**Key Questions:**
- How do we eliminate structural corruption without partisan weaponization?
- What term/age limits balance experience with institutional renewal?
- How do we ensure fair electoral maps and campaign finance?

**Success Criteria:**
- Elimination of congressional stock trading conflicts
- Independent redistricting mechanisms adopted
- Campaign finance transparency and small-donor amplification in place
- FPTP sunset and cardinal voting piloted in willing states
- New party formation pathway operational
- Voter ID universally enrolled before any matching requirement activates
- Presidential selection architecture statutory foundation established

---

## Subdomain Status Matrix

| Subdomain | Phase | File Count | Word Count (est.) | Key Gaps | Dependencies | Next Action | Target Date |
|-----------|-------|------------|------------|----------|--------------|-------------|-------------|
| Anti_Corruption | 3 | 5 | ~8,000 | Enforcement mechanisms; constitutional amendment pathway for term limits | None | Add enforcement mechanism detail | TBD |
| Campaign_Finance_Reform | 4–5 | 2 | ~10,500 | Enforcement home ambiguity (FEIC vs FEC successor vs new CFIC — open question in brief); FEIC/DFP institutional relationship needs final spec; convention bundling decision (CU amendment standalone vs. bundled with term limits) | ssi-self-sovereign-identity-framework, national-referendum-mechanism | Resolve enforcement home; spec FEIC/DFP relationship; finalize NRM title framing | 2026 |
| Term_and_Age_Limits | 2 | 1 | ~700 | Constitutional pathway; enforcement mechanisms | None | Add constitutional amendment strategy | TBD |
| Electoral_Reform | 4 | 9 | ~50,000 | Presidential sequencing explicit 4-year communication; Citizens United pathway in campaign finance; constitutional convention scope spec; sidebar_position conflict: representation-fairness at pos 1, system-standardization at pos 1 — needs resolution | ssi-self-sovereign-identity-framework, department-of-data-and-accountability, campaign-finance-reform, federal-electoral-integrity-commission | Prose build-out (Phase 5–6 messaging); resolve sidebar conflict | 2028 target |
| Digital_Democracy | 3 | 1 | ~5,500 | Phase 0 infrastructure dependencies; SSI deployment prerequisite — no timeline yet | unified-law-regulation-repository, ssi-self-sovereign-identity-framework, department-of-data-and-accountability | Define Phase 0 pilot jurisdiction plan | TBD |
| Representation_and_Self_Government | 2 | 1 | ~3,500 | Statehood pathway depth; USVI/Guam specific strategies | democratic-integrity, foreign-policy-guiding-principles | Add implementation pathway | TBD |
| Judicial_Reform | 2 | 1 | ~3,500 | Appointment enforcement mechanisms; confirmation threshold recommendation (currently open question); constitutional amendment pathway; SCOTUS brief updated to v2 | federal-age-and-term-limits | Expand with ethics enforcement + court size doctrine; make confirmation threshold recommendation | TBD |
| Implementation | 4–5 | 1 | ~9,500 | Article V convention delegate selection design; Electoral College Compact coordination; Master Platform Sequencing Document (cross-domain; not yet started) | national-referendum-mechanism, federal-electoral-integrity-commission, representation-fairness-electoral-method-choice | Cross-domain Master Sequencing Document | TBD |

---

## Electoral Reform and Implementation Sidebar Order (updated 2026-05-01)

**Implementation subdomain:**
| Position | File |
|----------|------|
| 0 | democratic-integrity-sequencing-v3 (domain implementation architecture — Layer 0-7 game plan) |

Within Electoral_Reform subdomain:
| Position | File |
|----------|------|
| 0 | electoral-reform-un-advisory-letter (context/framing) |
| 1 | electoral-reform-system-standardization (federal integrity floor) — ⚠️ CONFLICT: representation-fairness also at pos 1; needs resolution |
| 1* | electoral-reform-representation-fairness-v1 (certified method menu, anti-entrenchment, heatmap) — supersedes Anti-Gerrymandering brief |
| 2 | electoral-reform-party-formation-v2 (party market layer) |
| 3 | electoral-reform-presidential-selection-v2 (three-round architecture) |
| 4 | electoral-reform-candidate-nutrition-label-v2 (accountability loop) |
| 5 | election-day-and-primary-reform (scheduling infrastructure) |
| 6 | voter-id-registration-reform (access infrastructure) |
| 7 | DRAFT-national-referendum-mechanism (direct democratic authorization) |

**⚠️ Sidebar conflict to resolve:** `representation-fairness-electoral-method-choice` has `sidebar_position: 1` — same as `electoral-reform-system-standardization`. Representation fairness depends on system-standardization, so system-standardization should remain at 1 and representation-fairness should shift to 2, with subsequent files incrementing. Recommend: representation-fairness → 2, party-formation → 3, presidential-selection → 4, candidate-nutrition-label → 5, election-day → 6, voter-id → 7, national-referendum → 8.

---

## Dependency Map

### Hard Dependencies (Blocking)
| This Domain Requires | From Domain | Status | Risk Level |
|---------------------|-------------|--------|------------|
| SSI identity infrastructure | Technology_and_Data | Phase 3 | Medium |
| DoDA outcome measurement | Institutional_Modernization | Phase 3 | Low |

### Soft Dependencies (Coordination)
| This Domain Benefits From | From Domain | Status | Notes |
|--------------------------|-------------|--------|-------|
| Institutional modernization | Technology_and_Data | Phase 2 | Digital democracy tools |
| IRS modernization | Economic_Prosperity/Budget_and_Fiscal_Policy | Phase 2 | Voter ID SSI pathway shared infrastructure |

### Provides To (Downstream Impact)
| Other Domain | What We Provide | Criticality |
|--------------|-----------------|-------------|
| All domains | Clean governance foundation | High |
| Economic_Prosperity | PCA accountability, mandate contribution measurement | High |
| Institutional_Modernization | FEIC, DoDA mandate confirmation, congressional operating system | High |

---

## Gap Analysis

### Tier 1: Critical Gaps (Missing Foundation)
- [x] **Voting Rights & Access** — Election Day holiday, voter ID reform, and voter registration reform all at Phase 3–4 ✅
- [x] **Campaign Finance** — Individual-only donations, National Democracy Fund, 5:1 small-donor matching framework present ✅; needs Citizens United constitutional pathway and Phase 4 enforcement depth
- [x] **Electoral System Architecture** — Full v2 suite + representation fairness + implementation sequencing at Phase 4 ✅
- [x] **Anti-Gerrymandering / Representation Fairness** — Superseded by Representation Fairness and Electoral Method Choice (v1.0) — certified method menu (MMP, open-list PR, PR-STV, independent districting, small-delegation cardinal primary), federal integrity floor, anti-entrenchment architecture, constituency-service assignment + heatmap ✅
- [x] **Implementation Sequencing** — Democratic Integrity Stack v3.0 sequencing document: Layer 0-7 architecture, 2026–2036+ game plan, filibuster mechanics, NRM deployment sequence, legal pressure escalation doctrine ✅
- [~] **Judicial Reform** — SCOTUS brief updated to v2 (Article III modernization, fixed nonrenewable terms, appointment cadence, bounded authority); confirmation threshold and ethics enforcement still open

### Tier 2: Structural Gaps (Incomplete Coverage)
- [~] **Citizens United pathway** — Three-track strategy now present: statutory (regulated pathways doctrine, coordination redefinition, beneficial-owner disclosure, natural-person requirement); NRM (5 severable titles including Title V constitutional amendment instruction with 60% Tier 3 threshold); constitutional amendment (draft language restoring authority to regulate artificial-entity spending, viewpoint-neutral, press and individual speech safe harbor explicit); red-team attack section addresses all major attack lines; remaining open questions: enforcement home (FEIC vs FEC successor vs CFIC), convention bundling decision, union/labor asymmetry
- [ ] **Presidential sequencing communication** — Explicit 4-year timeline signal for what one presidential term delivers vs. what requires the next cycle — Target: Phase 5–6 prose
- [ ] **Enforcement mechanisms** — How corruption rules (stock trading ban, gerrymandering, campaign finance) are enforced operationally — Target: Phase 3
- [ ] **Article V convention delegate selection** — Sequencing brief identifies this as a critical dependency not yet resolved — Target: Phase 3
- [ ] **Master Platform Sequencing Document** — Cross-domain; sequencing brief explicitly scopes itself as domain-only — Target: Phase 4

### Tier 3: Enhancement Gaps (Nice-to-Have)
- [ ] **State legislature reform** — Extend principles to state level — Target: Phase 4
- [ ] **Lobbying reform** — Revolving door restrictions — Target: Phase 3
- [ ] **Shadow docket regulation** — Referenced as open question in judicial reform brief — Target: Phase 3

---

## Phase Advancement Checklist

### Electoral_Reform + Implementation — Requirements for Phase 4 (Sequencing & Execution) — Substantially Met
- [x] Full system architecture documented (v2 suite + representation fairness + sequencing) ✅
- [x] Implementation phasing sequenced (Layer 0-7 with specific 2026–2036+ timeline) ✅
- [x] Constitutional pathways identified (NRM, Article V, Electoral College Compact) ✅
- [x] International precedents cited (NZ, Germany, Ireland, Nordic PR systems) ✅
- [x] Pre-office preparation architecture (Layer 0 legal hardening, international technical advisory, NRM vessel testing) ✅
- [x] Failure mode sequencing documented (per-layer fallback paths) ✅
- [x] Legal pressure escalation doctrine defined ✅
- [ ] sidebar_position conflict resolved (representation-fairness vs. system-standardization both at pos 1)

### Electoral_Reform + Implementation — Requirements for Phase 5 (External Validation)
- [ ] 4-year presidential term communication explicit
- [ ] Stress-test against known attack lines (cartel protection, UN involvement, first-iteration imperfection)
- [ ] Rebuttal language drafted for FPTP sunset objections
- [ ] International technical review conducted (Layer 0 objective — not yet done)
- [ ] Public demonstration products built (representation distortion heatmaps, simulated delegations, NRM ballot prototypes)

### Campaign_Finance_Reform — Requirements for Phase 5 (External Validation) — Active Next Step
- [x] Core architecture defined (individual-only, NDF, tiers) ✅
- [~] Citizens United pathway — three-track strategy (statutory/NRM/amendment) defined; draft amendment language present; NRM titles designed; red-team section drafted; remaining open questions are solvable design choices ✅
- [~] Enforcement architecture — civil/administrative penalties, Democracy Fund Portal real-time disclosure, FEIC anti-capture mandate, sectoral caps, lobbying credit system; enforcement home (FEIC vs. FEC successor vs. new CFIC) still an open question
- [ ] FEIC/DFP final institutional relationship spec
- [ ] NRM title framing finalized and reviewed
- [ ] Convention bundling decision (CU amendment standalone vs. bundled with term limits/SCOTUS reform)

---

## Recent Activity Log

| Date | Subdomain | Change | Phase Impact |
|------|-----------|--------|--------------|
| 2026-05-01 | Campaign_Finance_Reform | Added campaign-finance-anti-capture-v1.md (v1.0): three-track Citizens United closure strategy (statutory + NRM + constitutional amendment); regulated pathways doctrine; coordination redefinition (rebuttable presumption); real-time beneficial-owner disclosure; natural-person requirement; dark-money pass-through ban; lobbying access credit system; 5 severable NRM titles including Title V constitutional amendment instruction; draft amendment language; red-team attack surface section; sequencing integration with Layer 0-7 | Phase 3 → 4–5; Citizens United pathway substantially addressed |
| 2026-05-01 | Electoral_Reform | Added electoral-reform-representation-fairness-v1.md (v1.0): federal democratic integrity floor, certified method menu (MMP, open-list PR, PR-STV, independent nonpartisan districting, small-delegation cardinal primary), anti-entrenchment architecture, constituency-service assignment + representation heatmap, voluntary adoption + National Political Market Opening Act pathway; supersedes deprecated Anti-Gerrymandering brief; sidebar_position: 1 conflicts with system-standardization — needs resolution | 8 → 9 files; gaps closed |
| 2026-05-01 | Implementation | Added democratic-integrity-sequencing-v3.md (v3.0): Layer 0-7 full legislative game plan for DI Stack, 2026–2036+ timeline, filibuster reform mechanics, legal pressure escalation doctrine, NRM deployment sequence, failure mode sequencing, cross-domain interface documentation; new subdomain Implementation | New subdomain; domain Phase 3–4 → 4 |
| 2026-05-01 | Judicial_Reform | SCOTUS reform updated from v1 to v2 (draft-scotus-judicial-reform-v2.md); v1 moved to deprecated/ | N/A |
| 2026-04-25 | Electoral_Reform | Added 4 core v2 briefs: electoral-reform-system-standardization.md (federal integrity floor, FEIC, FPTP sunset, cardinal voting menu), electoral-reform-party-formation-v2.md (party market layer, anti-cartel enforcement, congressional caucus rights), electoral-reform-presidential-selection-v2.md (three-round architecture, regional credentialing, execution record pathway), electoral-reform-candidate-nutrition-label-v2.md (four-tier schema, mandate accountability loop, coalition discovery infrastructure) | Phase 3 → 4 |
| 2026-04-25 | Electoral_Reform | Resolved sidebar_position conflicts: election-day 4→5, voter-id 5→6, national-referendum 6→7, candidate-nutrition-label at 4 (new anchor) | N/A |
| 2026-04-25 | Anti_Corruption | Resolved sidebar_position conflict: impeachment-triggers 2→3 | N/A |
| 2026-04-10 | Judicial_Reform | Added draft-scotus-judicial-reform.md (Article III modernization — fixed nonrenewable 18-year terms, structured appointment cadence, constrained nomination process, bounded authority doctrine) | 0 → 1 file |
| 2026-04-10 | Representation_and_Self_Government | Added territorial-self-determination-and-representation-normalization.md (DC statehood + territory representation normalization; domain: Democratic_Integrity, physically in National_Security/foreign-policy/ folder — structural cross-placement) | 0 → 1 file |
| 2026-04-10 | Cross-domain note | coordinated-deceptive-practices-enforcement-framework-v0.5.md lives in Democratic_Integrity folder but declares domain: Institutional_Modernization — tracked under Institutional-Modernization | N/A |
| 2026-03-29 | Anti_Corruption | Added impeachment-reform-enumerated-triggers-v0.4.md (enumerated triggers, democratic override, enforcement doctrine — 12 triggers across 5 categories, supermajority override) | 3 → 5 files |
| 2026-03-26 | Electoral_Reform | Added election-day-and-primary-reform.md, voter-id-registration-reform.md, national-referendum-mechanism.md | 0 → 3 files |
| 2026-03-26 | Digital_Democracy | Added digital-democracy-platform.md (domain: Institutional_Modernization, lives in DI folder) | 0 → 1 file |
| 2026-03-26 | All (YAML) | Full YAML front matter standardized across all files | N/A |

---

## Notes & Context

- Domain now has **19 files** totaling ~67,000 words (up from 16 / ~47,000)
- Electoral_Reform is the most developed subdomain: 9 files, ~50,000 words, Phase 4; includes representation fairness (v1.0) which supersedes Anti-Gerrymandering
- **Campaign Finance** substantially advanced — anti-capture brief (v1.0) provides the Citizens United closure strategy the original brief lacked; three-track architecture (statutory/NRM/amendment) with draft amendment language, red-team attack surface, and sequencing integration; now Phase 4–5
- **Implementation subdomain** is new — sequencing v3.0 is the domain's legislative game plan (Layer 0-7, 2026–2036+ timeline); classified as Phase 4–5 because it contains attack-line handling (legal pressure escalation doctrine) and cross-domain coordination architecture
- **Representation Fairness** (v1.0): the most architecturally complete single brief in the domain — certified method menu with five options, FEIC anti-entrenchment enforcement, constituency-service assignment + heatmap resolves the "who represents me under PR?" objection; supersedes deprecated Anti-Gerrymandering brief
- **Lobbying Access Credit system** inside the anti-capture brief is the affirmative replacement for shadow channels — not just restriction but redirection; public, priced, nonexclusive, auditable; revenue funds public-interest counterweight capacity
- **Sidebar conflict to resolve**: representation-fairness and system-standardization both at sidebar_position 1; representation-fairness should shift to 2
- Digital Democracy Platform (domain: Institutional_Modernization, lives in DI folder) — structural cross-placement, future reconciliation needed
- CDE enforcement framework (domain: Institutional_Modernization, lives in DI folder) — tracked under Institutional-Modernization
- Representation_and_Self_Government subdomain (lives in NS/foreign-policy folder) — cross-domain placement
- Electoral reform Phase 5–6 messaging and rebuttal (attack-line stress testing, 4-year presidential sequencing communication) remain as active next step
