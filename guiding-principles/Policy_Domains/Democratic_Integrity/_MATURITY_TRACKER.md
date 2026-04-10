# Domain Maturity Tracker: Democratic_Integrity

**Last Updated:** 2026-04-10
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
Strengthen democratic institutions against corruption, ensure fair representation, and modernize governance mechanisms for accountability and responsiveness.

**Key Questions:**
- How do we eliminate structural corruption without partisan weaponization?
- What term/age limits balance experience with institutional renewal?
- How do we ensure fair electoral maps and campaign finance?

**Success Criteria:**
- Elimination of congressional stock trading conflicts
- Independent redistricting mechanisms adopted
- Campaign finance transparency and limits in place

---

## Subdomain Status Matrix

| Subdomain | Phase | File Count | Word Count | Key Gaps | Dependencies | Next Action | Target Date |
|-----------|-------|------------|------------|----------|--------------|-------------|-------------|
| Anti_Corruption | 2 | 5 | ~5,500 | Enforcement mechanisms | None | Add implementation details | TBD |
| Campaign_Finance_Reform | 2 | 1 | ~800 | Public financing details | Budget.Campaign_Funding | Expand financing model | TBD |
| Term_and_Age_Limits | 2 | 1 | ~700 | Constitutional pathway | None | Add constitutional amendment strategy | TBD |
| Electoral_Reform | 3 | 3 | ~7,200 | Third-party ballot access implementation timeline; automatic registration tech integration | ssi-self-sovereign-identity-framework, department-of-data-and-accountability | Expand implementation sequencing | TBD |
| Digital_Democracy | 3 | 1 | ~5,500 | Phase 0 infrastructure dependencies; SSI deployment prerequisite — no timeline yet | unified-law-regulation-repository, ssi-self-sovereign-identity-framework, department-of-data-and-accountability | Define Phase 0 pilot jurisdiction plan | TBD |
| Representation_and_Self_Government | 2 | 1 | ~3,500 | Statehood pathway depth; USVI/Guam specific strategies | democratic-integrity, foreign-policy-guiding-principles | Add implementation pathway | TBD |
| Judicial_Reform | 0 | 0 | 0 | **Not started** | None | Create initial file | TBD |

---

## Dependency Map

### Hard Dependencies (Blocking)
| This Domain Requires | From Domain | Status | Risk Level |
|---------------------|-------------|--------|------------|
| Campaign funding mechanism | Budget | Not started | Medium |

### Soft Dependencies (Coordination)
| This Domain Benefits From | From Domain | Status | Notes |
|--------------------------|-------------|--------|-------|
| Institutional modernization | Technology_and_Data | Phase 2 | Digital democracy tools |

### Provides To (Downstream Impact)
| Other Domain | What We Provide | Criticality |
|--------------|-----------------|-------------|
| All domains | Clean governance foundation | High |

---

## Gap Analysis

### Tier 1: Critical Gaps (Missing Foundation)
- [x] **Voting Rights & Access** – Election Day holiday, voter ID reform, and voter registration reform all added at Phase 3 ✅
- [ ] **Judicial Reform** – Supreme Court structure, term limits – Target: Phase 2

### Tier 2: Structural Gaps (Incomplete Coverage)
- [ ] **Enforcement mechanisms** – How corruption rules are enforced – Target: Phase 3
- [ ] **Constitutional amendment strategy** – Pathway for term limits – Target: Phase 3

### Tier 3: Enhancement Gaps (Nice-to-Have)
- [ ] **State legislature reform** – Extend principles to state level – Target: Phase 4
- [ ] **Lobbying reform** – Revolving door restrictions – Target: Phase 3

---

## Phase Advancement Checklist

### Requirements for Phase 3 (Outcomes & Decision Rules)
- [ ] Clear success metrics defined
- [ ] Decision criteria established
- [ ] Risk mitigation strategies documented
- [ ] Monitoring framework designed

---

## Recent Activity Log

| Date | Subdomain | Change | Phase Impact |
|------|-----------|--------|--------------|
| 2026-04-10 | Representation_and_Self_Government | Added territorial-self-determination-and-representation-normalization.md (DC statehood + territory representation normalization; domain: Democratic_Integrity, physically in National_Security/foreign-policy/ folder — structural cross-placement) | 0 → 1 file |
| 2026-04-10 | Cross-domain note | coordinated-deceptive-practices-enforcement-framework-v0.5.md lives in Democratic_Integrity folder but declares domain: Institutional_Modernization (market integrity / CDE framework) — tracked under Institutional-Modernization | N/A |
| 2026-03-29 | Anti_Corruption | Added impeachment-reform-enumerated-triggers-v0.4.md (enumerated triggers, democratic override, enforcement doctrine — 12 triggers, supermajority override) and impeachment-reform-oversight-commission-v0.1.md (oversight commission architecture, special counsel framework, suspension mechanism governance); YAML standardized with sidebar fields | 3 → 5 files |
| 2026-03-26 | Electoral_Reform | Added election-day-and-primary-reform.md (federal holiday + unified national Primary Day, 1-year deliberative window, ballot access standardization), voter-id-registration-reform.md (3-phase framework: universal free ID, numeric matching, SSI cryptographic identity), national-referendum-mechanism.md (NRM: circuit breaker for institutional capture — 7-part anti-capture architecture with red-team analysis) | 0 → 3 |
| 2026-03-26 | Digital_Democracy | Added digital-democracy-platform.md (5-phase platform: SSI identity layer, ULRR jurisdictional routing, signal capture, DoDA processing, lawmaker dashboards, semi-annual townhalls, 10-year mandate formation, referendum infrastructure) — domain declared as Institutional_Modernization but lives in Democratic_Integrity folder | 0 → 3 |
| 2026-03-26 | All (YAML) | Added full YAML front matter to all 7 files missing domain/subdomain/policy_type/status/version/author/last_updated; corrected dependency slugs in national-referendum-mechanism.md and digital-democracy-platform.md | N/A |
| 2026-03-12 | Execution_Corps | Subdomain removed from this domain — moved to Institutional-Modernization | N/A |
| 2025-01-25 | All | YAML standardized, Docusaurus format | N/A |

---

## Notes & Context

- Domain has **12 files** totaling ~22,200 words
- Voting rights gap closed: election day, voter ID, national referendum mechanism all at Phase 3
- Digital Democracy Platform added (massive doc, ~5,500 words) — declares domain: Institutional_Modernization but lives in Democratic_Integrity folder; structural note for future reconciliation
- Anti-corruption stack still needs enforcement mechanism detail; constitutional amendment strategy for term limits unwritten
- Execution_Corps subdomain moved to Institutional-Modernization domain
- New: Representation_and_Self_Government subdomain — territorial-self-determination added (lives in NS/foreign-policy folder, cross-domain placement)
- CDE enforcement framework lives in DI folder but declares domain: Institutional_Modernization
