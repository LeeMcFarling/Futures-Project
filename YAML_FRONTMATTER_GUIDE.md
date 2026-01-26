# YAML Front Matter Standard - Quick Reference

## Template

Copy this to the top of every new policy markdown file:

```yaml
---
domain: [Domain_Name]
subdomain: [Subdomain_Name]
phase: [0-6]
dependencies:
  - type: [hard|soft|optional]
    target: [Domain.Subdomain]
    reason: [Brief explanation]
status: [draft|in_progress|review|complete]
last_updated: [YYYY-MM-DD]
---
```

## Field Definitions

### domain (required)
The top-level policy domain. Should match the directory name exactly.

**Examples:**
- `Climate_and_Energy`
- `Healthcare`
- `National_Security`
- `Immigration`

### subdomain (required)
The specific policy area within the domain.

**Examples:**
- For Climate_and_Energy: `Decarbonization`, `Grid_Modernization`, `Renewable_Energy`
- For Healthcare: `Universal_Coverage`, `Drug_Pricing`, `Rural_Access`

### phase (required)
Current development phase (0-6) following the Phase Model:

- **0** = Problem Framing
- **1** = Strategic Constraints  
- **2** = Structured Exploration
- **3** = Outcomes & Decision Rules
- **4** = Sequencing & Execution Design
- **5** = External Validation
- **6** = Messaging & Rebuttal

**Rules:**
- Be conservative - don't claim a phase until requirements are met
- Files cannot exceed the phase of their dependencies
- See Phase Advancement Checklist in domain tracker

### dependencies (optional but recommended)
List of other policy areas this file depends on.

**Dependency Types:**
- **hard** - Blocking dependency; this policy cannot advance without it
- **soft** - Coordination needed; beneficial but not blocking
- **optional** - Nice to have; can proceed independently

**Format:**
```yaml
dependencies:
  - type: hard
    target: Budget.Carbon_Revenue
    reason: Need revenue mechanism for carbon pricing
  - type: soft
    target: Public_Infrastructure.Grid
    reason: Coordination on grid upgrades
```

**Target Format:** `Domain.Subdomain` (use underscores, match exact names)

### status (required)
Current working status of the file:

- **draft** - Initial outline or rough draft
- **in_progress** - Actively being written/developed
- **review** - Complete enough for review/feedback
- **complete** - Finished for current phase

### last_updated (required)
Date of last significant update in `YYYY-MM-DD` format.

**Examples:** `2025-01-25`, `2024-12-15`

Update this when:
- Content changes substantially
- Phase advances
- Dependencies change

---

## Complete Examples

### Example 1: Early Phase File

```yaml
---
domain: Climate_and_Energy
subdomain: Decarbonization
phase: 1
dependencies:
  - type: hard
    target: Budget.Carbon_Revenue
    reason: Need revenue mechanism for carbon pricing policy
  - type: soft
    target: Economic_Prosperity.Manufacturing
    reason: Coordination on green manufacturing incentives
status: in_progress
last_updated: 2025-01-25
---

# Decarbonization Strategy

[Content here...]
```

### Example 2: Advanced Phase File

```yaml
---
domain: Healthcare
subdomain: Universal_Coverage
phase: 4
dependencies:
  - type: hard
    target: Budget.Healthcare_Financing
    reason: Requires comprehensive funding model
  - type: hard
    target: Economic_Prosperity.Labor_Market
    reason: Impacts employer-based coverage transitions
  - type: soft
    target: Technology_and_Data.Health_IT
    reason: Electronic health records integration
status: review
last_updated: 2025-01-20
---

# Universal Healthcare Coverage

[Content here...]
```

### Example 3: No Dependencies

```yaml
---
domain: Democratic_Integrity
subdomain: Voting_Rights
phase: 2
dependencies: []
status: in_progress
last_updated: 2025-01-22
---

# Voting Rights and Access

[Content here...]
```

---

## Best Practices

### ✅ DO:
- Keep domain/subdomain names consistent with directory structure
- Use underscores in names (not spaces or hyphens)
- Be conservative with phase assignments
- Document all meaningful dependencies
- Update `last_updated` when making significant changes
- List hard dependencies first, then soft, then optional

### ❌ DON'T:
- Claim a phase without meeting requirements
- Create circular dependencies
- Use spaces in domain/subdomain names
- Forget to update `last_updated`
- Add dependencies without explaining why

---

## Dependency Checklist

Before adding a dependency, ask:

1. **Is it truly required?** (hard) or just beneficial? (soft)
2. **Is the target specific enough?** (use Domain.Subdomain format)
3. **Is the reason clear?** (helps others understand the connection)
4. **Have I checked for circular dependencies?** (A depends on B, B depends on A)

---

## Phase Discipline Reminders

- A file at **Phase 2** cannot depend on something at **Phase 0**
- If dependencies advance, dependent files can potentially advance
- The automation script flags phase violations
- When in doubt, stay at lower phase until requirements are clearly met

---

## Validation

The automation script will:
- ✅ Extract this front matter automatically
- ✅ Count files per subdomain
- ✅ Calculate domain phase (minimum across subdomains)
- ✅ Flag missing dependencies
- ⚠️ Warn about phase violations (future feature)

---

## Questions?

If you're unsure about:
- **Domain/subdomain naming**: Check existing trackers in `docs/*/`
- **Phase assignment**: See Phase Advancement Checklist in domain tracker
- **Dependency type**: If it blocks progress → hard, if it's just coordination → soft
- **Status**: When in doubt, use `in_progress`
