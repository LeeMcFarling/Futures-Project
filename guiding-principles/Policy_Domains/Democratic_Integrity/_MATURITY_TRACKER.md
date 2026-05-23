# Domain Maturity Tracker: Democratic_Integrity

**Last Updated:** 2026-05-21
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
Break structural corruption and anti-democratic capture across all institutions — electoral system, judiciary, campaign finance, anti-corruption enforcement, and digital information environments. The democratic integrity stack is genuinely non-partisan in effect: it breaks machines on both sides, returns control to voters, and creates the institutional conditions for every other policy domain to function without capture.

**Key Questions:**
- How do we eliminate money-as-speech distortions without triggering First Amendment litigation that kills the reform?
- What electoral architecture produces genuine multi-party competition and candidate quality rather than primary extremism?
- How do we modernize the judiciary and impeachment architecture without creating partisan weaponization?
- What digital democracy infrastructure supports informed consent at scale?

**Success Criteria:**
- Campaign finance architecture operational: anti-bundling enforcement, Citizens United workaround, transparency infrastructure
- Electoral reform stack passed: party formation, primary reform, presidential selection, national referendum mechanism
- Judicial reform enacted: SCOTUS term limits, Article III modernization
- Enumerated impeachment triggers codified
- Anti-corruption floor: stock trading ban, age/term limits, voter ID + registration reform
- Digital democracy platform architecture specified

---

## Subdomain Status Matrix

| Subdomain | Phase | File Count | Word Count | Key Gaps | Dependencies | Next Action | Target Date |
|-----------|-------|------------|------------|----------|--------------|-------------|-------------|
| Campaign_Finance | 3 | 1 | ~5,955 | 3 remaining spec choices: enforcement home agency, constitutional convention bundling architecture, union/labor asymmetry resolution | department-of-data-and-accountability | Resolve 3 spec choices; finalize enforcement agency | TBD |
| Electoral_Reform | 3 | 8 | ~25,431 | Implementation sequencing across 8 instruments; congressional authorization pathway | Institutional-Modernization (Legislative_Design) | Implementation sequencing spec; statutory language templates | TBD |
| Judicial_Reform | 3 | 1 | ~2,108 | SCOTUS term limit constitutional pathway; circuit court reform | None | Constitutional amendment vs. statute analysis | TBD |
| Anti_Corruption | 3 | 3 | ~5,657 | Enforcement agency design; whistleblower protection architecture | Institutional-Modernization (Democratic_Execution_Interface) | Enforcement agency spec; whistleblower framework | TBD |
| Digital_Democracy | 2–3 | 1 | ~5,459 | Platform specification incomplete (DRAFT); UPI/SSI integration for secure digital civic participation | Technology_and_Data | Prose completion; SSI voting registration integration | TBD |
| Sequencing_and_Architecture | 3 | 1 | ~6,430 | Cross-subdomain activation sequence; congressional coalition design | All subdomains | Activation calendar; coalition pathway | TBD |

---

## Dependency Map

### Hard Dependencies (Blocking)
| This Domain Requires | From Domain | Status | Risk Level |
|---------------------|-------------|--------|------------|
| Enforcement infrastructure for campaign finance | Institutional-Modernization (DoDA + Democratic_Execution_Interface) | Phase 3 | Low |

### Soft Dependencies (Coordination)
| This Domain Benefits From | From Domain | Status | Notes |
|--------------------------|-------------|--------|-------|
| SSI/UPI identity layer | Technology_and_Data | Phase 2 | Voter registration, secure digital participation |
| Legislative design templates | Institutional-Modernization | Phase 2 | Statutory language for electoral reform |

### Provides To (Downstream Impact)
| Other Domain | What We Provide | Criticality |
|--------------|-----------------|-------------|
| All domains | Clean governance foundation — prevents capture of every other reform | Critical |
| Institutional-Modernization | Democratic legitimacy framework for execution instruments | High |
| All domains | Judicial reform — removes activist bench risk for litigation-targeted reforms | High |

---

## Gap Analysis

### Tier 1: Critical Gaps (Missing Foundation)
- [x] **Campaign Finance / Citizens United architecture** — campaign-finance-anti-capture-v1.md (v1): anti-bundling architecture, PAC transparency, constitutional workaround strategy, enforcement framework ✅; [~] 3 remaining spec choices: enforcement home agency, constitutional convention bundling, union/labor asymmetry
- [x] **Electoral Reform stack** — 8-file v2 series: party formation, presidential selection, representation fairness, system standardization, national referendum mechanism, candidate nutrition label, election day reform, UN advisory letter ✅
- [x] **Judicial Reform** — draft-scotus-judicial-reform-v2.md: Article III term limits, SCOTUS expansion risk analysis, constitutional pathway ✅
- [x] **Enumerated Impeachment Triggers** — impeachment-reform-enumerated-triggers-v0.4.md (v0.4): statutory enumeration of impeachable offenses, removal mechanics, Senate trial reform ✅
- [x] **Anti-Corruption Floor** — voter-id-registration-reform.md, federal-employee-age-and-term-limits.md, ban-stock-trading (multiple versions) ✅
- [x] **Sequencing Architecture** — democratic-integrity-sequencing-v3.md: cross-subdomain activation sequence, congressional pathway analysis ✅

### Tier 2: Structural Gaps (Incomplete Coverage)
- [~] **Campaign Finance (3 spec choices)** — enforcement home agency (FEC vs. new entity vs. DoJ), constitutional convention bundling architecture (how to handle bundled contributions at conventions), union/labor asymmetry (whether union political activity gets symmetric treatment) — Target: Phase 4
- [ ] **Digital Democracy Platform** — DRAFT-digital-democracy-platform.md is incomplete; SSI/UPI integration for secure civic participation not yet specified — Target: Phase 4
- [ ] **Lobbying Reform** — revolving door restrictions, disclosure requirements — Target: Phase 3
- [ ] **Congressional delegation and presidential powers sunset** — BRIEF NEEDED (canonical home for this cross-domain brief): instrument is a single statute with two operative provisions: (1) **retroactive sunset** — enumerates all existing open-ended congressional authority grants (AUMFs 2001/2002, IEEPA tariff invocations, Section 232/301 determinations, National Emergency Act declarations) and sets a scheduled expiration for each unless Congress affirmatively reauthorizes; this retires the accumulated stock of unchecked authority in one vote rather than requiring Congress to relitigate each authority individually; (2) **mandatory prospective sunset** — establishes that any future congressional delegation of executive authority must include defined scope, duration limit, and automatic expiration; no open-ended grants permitted; brief should also specify: reauthorization threshold (simple majority vs. supermajority), reporting requirements during grant period, and connection to impeachment reform enumerated triggers (acting under lapsed authority as enumerated offense); connects to treaty lock-in architecture (treaties as high-durability instrument for commitments you want to keep; delegated emergency powers as time-bounded instrument requiring periodic democratic reauthorization — currently inverted); cross-references National_Security (AUMF/emergency declarations) and Trade_Policy (IEEPA/TPA/Section 232) — Target: Phase 3

### Tier 3: Enhancement Gaps (Nice-to-Have)
- [ ] **State legislature extension** – Apply electoral architecture to state level – Target: Phase 4
- [ ] **DACA/immigration crossover** – Country-based restriction linkage to Democratic Integrity principles – Target: Phase 4

---

## Phase Advancement Checklist

### Requirements for Phase 4 (Sequencing & Execution)
- [x] Electoral reform instruments specified (8-file stack) ✅
- [x] Campaign finance architecture defined ✅
- [x] Judicial reform pathway articulated ✅
- [x] Impeachment triggers codified ✅
- [ ] Campaign finance 3 spec choices resolved
- [ ] Digital democracy platform prose completed
- [ ] Implementation sequencing calendar (which instrument first, in what political sequence)
- [ ] Stress-testing against known attack lines ("government censorship," "incumbent protection," "anti-free-speech")

---

## Recent Activity Log

| Date | Subdomain | Change | Phase Impact |
|------|-----------|--------|--------------|
| 2026-05-21 | Separation_of_Powers | TODO logged: congressional delegation and presidential powers sunset brief — catalog open-ended authority grants (AUMFs, IEEPA, TPA, Section 232, NEA), systematic sunset/reauthorization framework, constitutional template for future delegations, treaty/impeachment cross-reference; canonical home for cross-domain brief (NS + Trade cross-ref) | Tier 2 gap added |
| 2026-05-16 | All | Tracker updated to reflect actual domain state; phase corrected 2 → 3; file count corrected 7 → 15 active; word count corrected ~5K → ~51K | N/A |
| 2026-04-27 | Campaign_Finance | campaign-finance-anti-capture-v1.md: Citizens United architecture complete; 3 spec choices remain (enforcement home, convention bundling, union/labor asymmetry) — marked [~] not [x] | Phase 3 |
| 2026-04-27 | Electoral_Reform | Electoral reform v2 series complete: party formation, presidential selection, representation fairness, system standardization, national referendum, candidate nutrition label, UN advisory letter | Phase 3 |
| 2026-04-27 | Judicial_Reform | draft-scotus-judicial-reform-v2.md: Article III modernization, term limits, constitutional pathway | New |
| 2026-04-27 | Anti_Corruption | impeachment-reform-enumerated-triggers-v0.4.md, voter-id-registration-reform.md, election-day-and-primary-reform.md added | Enhanced |
| 2026-04-27 | Digital_Democracy | DRAFT-digital-democracy-platform.md: platform spec draft (incomplete) | New |
| 2026-04-27 | Sequencing | democratic-integrity-sequencing-v3.md: master sequencing and architecture document | New |
| 2025-01-25 | All | YAML standardized, Docusaurus format | N/A |

---

## Notes & Context

- Domain has **15 active files** at root level totaling ~50,280 words (plus 3 files in `Anti Corruption/` subdirectory as older versions, deprecated folder)
- **Domain doubled this platform** from original 7 files (~4,986 words) — entire electoral reform stack was written after January 2025
- **This is the most politically dangerous domain in the stack** — campaign finance, judicial reform, and electoral architecture together attack the core infrastructure of political power in both parties; it will be attacked as self-serving by incumbents of all stripes
- **The correct answer to "is this a power grab?"** is no — if it works, it breaks the Democrats too. The architecture is anti-machine, not anti-party.
- **Citizens United workaround** is the hardest legal problem in the domain — the architecture is complete but the 3 remaining spec choices are genuinely hard constitutional questions, not just style choices
- **Electoral reform UN advisory letter** is a distinctive credential — seeking UN electoral observation endorsement as a legitimacy anchor; unusual for a domestic reform proposal and potentially powerful
- **Candidate nutrition label** is one of the highest-leverage low-cost instruments in the platform: standardized disclosure format for candidate positions; forces comparison shopping; destroys the ambiguity incumbents rely on
- **Sequencing document (v3)** is the meta-coordination spec for this domain — should be read first before any subdomain file
- Old duplicate files (Campaign_Finance.md, Ban_stock_trading.md) are at root level and predate the v1/v2 series; they can be archived
