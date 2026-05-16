# Futures Project - Maturity Tracking Automation

This system automates policy domain tracking and gap analysis for the Futures Project.

## Overview

The automation consists of:
1. **Maturity Tracker Template** - Standardized tracking document for each domain
2. **Automation Script** - Python script to scan repo and update trackers
3. **YAML Front Matter** - Metadata standard for all policy files

## File Structure

```
repo/
├── docs/
│   ├── Climate_and_Energy/
│   │   ├── _MATURITY_TRACKER.md          # Auto-generated tracker
│   │   ├── Decarbonization.md             # Policy file
│   │   └── Grid_Modernization.md          # Policy file
│   ├── Healthcare/
│   │   ├── _MATURITY_TRACKER.md
│   │   └── [policy files...]
│   └── [other domains...]
├── PROJECT_STATUS.md                       # Overall project status (auto-generated)
├── maturity_scan.py                        # Automation script
└── MATURITY_TRACKER_TEMPLATE.md           # Template for new domains
```

## YAML Front Matter Standard

Every policy markdown file should include this front matter:

```yaml
---
domain: Climate_and_Energy
subdomain: Decarbonization
phase: 2
dependencies:
  - type: hard
    target: Budget.Carbon_Revenue
    reason: Need revenue mechanism for carbon pricing
  - type: soft
    target: Public_Infrastructure.Grid
    reason: Coordination on grid upgrades
status: in_progress
last_updated: 2025-01-25
author: [optional]
---
```

### Front Matter Fields

- **domain**: Top-level policy domain (matches directory name)
- **subdomain**: Specific area within domain
- **phase**: Current phase (0-6) following the Phase Model
- **dependencies**: Array of dependencies with type (hard/soft/optional), target, and reason
- **status**: `draft`, `in_progress`, `review`, `complete`
- **last_updated**: Date of last significant update
- **author**: (Optional) Who's working on this

## Commands for Claude Code

### 1. Scan All Domains and Update Trackers

```bash
python maturity_scan.py scan
```

This will:
- Scan all domain directories
- Count files and words per subdomain
- Extract phase information from front matter
- Update `_MATURITY_TRACKER.md` in each domain
- Generate `PROJECT_STATUS.md` with overall status

### 2. Generate Project Status Report

```bash
python maturity_scan.py report
```

Creates a comprehensive status report showing:
- Total domains, files, and words
- Phase distribution
- Links to all domain trackers

### 3. Analyze Gaps

```bash
python maturity_scan.py gaps
```

Outputs gap analysis in three tiers:
- **Tier 1**: Missing domains (no files)
- **Tier 2**: Skeletal domains (1-2 files or <1000 words)
- **Tier 3**: Domains that could expand (<5000 words)

### 4. Validate Phase Discipline

```bash
python maturity_scan.py validate
```

(Coming soon) - Will check for:
- Phase violations (files claiming higher phase than dependencies)
- Missing required elements for phase advancement
- Dependency conflicts

## Typical Claude Code Workflow

When asked to "scan the repo for gaps":

1. Run: `python maturity_scan.py scan`
2. Read the generated `PROJECT_STATUS.md`
3. Run: `python maturity_scan.py gaps`
4. Summarize findings in tier format
5. Recommend priority domains based on analysis

When asked to "update maturity trackers":

1. Run: `python maturity_scan.py scan`
2. Confirm updates were successful
3. Report any new gaps or phase changes

When creating a new domain:

1. Create domain directory: `mkdir docs/New_Domain`
2. Copy template: `cp MATURITY_TRACKER_TEMPLATE.md docs/New_Domain/_MATURITY_TRACKER.md`
3. Edit template to fill in domain-specific information
4. Create first policy file with proper front matter
5. Run: `python maturity_scan.py scan`

## Automation Capabilities

The script automatically:

- ✅ Counts files per subdomain
- ✅ Counts total words (excluding front matter)
- ✅ Extracts phase from front matter
- ✅ Identifies dependencies
- ✅ Calculates overall domain phase (minimum across subdomains)
- ✅ Flags gaps (no files, minimal content)
- ✅ Preserves manual notes in trackers
- ✅ Generates project-wide status report

## What Claude Code Should Do

**When scanning:**
- Run the automation script
- Read generated reports
- Summarize findings in user-friendly format
- Highlight priority gaps

**When asked about a specific domain:**
- Navigate to domain directory
- Read `_MATURITY_TRACKER.md`
- Check actual policy files for detail
- Report status and recommend next actions

**When creating new content:**
- Ensure proper YAML front matter
- Run scan after creation to update trackers
- Check for phase violations

## Integration with User Workflow

1. **User works** to research and draft policy content
2. **User commits new markdown files** to repo with proper front matter
3. **User asks Claude Code** to "scan for updates"
4. **Claude Code runs** `maturity_scan.py scan`
5. **Claude Code reports** new status and any gaps
6. **User returns** for next research/writing task

## Configuration

Edit these variables in `maturity_scan.py` to match your repo structure:

```python
REPO_ROOT = Path(".")  # Adjust to your repo root
DOMAINS_DIR = REPO_ROOT / "docs"  # Adjust to where your policy domains are
TRACKER_FILENAME = "_MATURITY_TRACKER.md"
PROJECT_STATUS_FILE = REPO_ROOT / "PROJECT_STATUS.md"
```

## Requirements

```bash
pip install pyyaml
```

## Notes

- The automation **preserves manual notes** added to trackers below the auto-generated sections
- Domain phase is calculated as **minimum phase across all subdomains** (conservative approach)
- Empty directories are flagged as Phase 0
- The script is **idempotent** - safe to run multiple times
