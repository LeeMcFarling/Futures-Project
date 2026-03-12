---
id: civilizational-cost-function-model
title: Model Definitions — Continuity Portfolio & Civilizational Cost Function
sidebar_label: Model Definitions
sidebar_position: 2
slug: /framework-foundations/model-definitions
domain: Framework_Foundations
subdomain: Theoretical_Foundations
policy_type: Research Framework
status: Active
version: 0.1
author: Futures Project
last_updated: 2026-03-12
dependencies:
  - central-axioms-civilizational-stability
  - existential-stability-axiom
related_initiatives:
  - adaptive-governance-evidence-protocol
tags:
  - formal-model
  - continuity-portfolio
  - cost-function
  - civilizational-stability
---

# Defining the Model

To formalize, let each individual \(i\) have a **continuity portfolio** composed of anchors \(j=1,\dots,J\). Each anchor has a base value \(x_{ij}\) (positive meaning or utility the person derives) and is subject to threats. Let \(t_j^{(m)}\) be the *mortality*-threat to anchor \(j\) and \(t_j^{(e)}\) the *existential*-threat to that anchor (both per-unit costs). Each individual assigns a weight \(b_{ij}\) to anchor \(j\) (reflecting how central that anchor is to their identity). One simple linear model of individual stability \(F_i\) (a “continuity score”) is:  

\[
F_i \;=\; \sum_{j=1}^J b_{ij} \Bigl( x_{ij} \;-\; \bigl[t_j^{(m)} + t_j^{(e)}\bigr]\Bigr)\,. 
\]

Equivalently, \(F_i = \sum_j b_{ij} x_{ij} - \sum_j b_{ij}(t_j^{(m)}+t_j^{(e)})\).  In words, each anchor’s contribution is its intrinsic value \(x_{ij}\) minus the composite threat cost; the weights \(b_{ij}\) linearly scale both. If economic status (income, savings) is itself an anchor, then economic threats feed into \(t_j\). In particular, financial insecurity has been shown to **erode meaning in life** above and beyond actual income【45†L1-L4】【46†L1079-L1087】, so a shock to an economic anchor counts as both mortality (survival) and existential (meaning) threat.  

On the **population level**, we aggregate fragility. A **civilizational cost function** \(C\) can penalize unsafe states. A plausible form is:  

\[
C \;=\; \alpha\,\mathbb{E}[F_i] \;+\; \beta\,\mathrm{Var}(F_i) \;+\; \gamma\,\sum_{j<k} b_{\bullet j} b_{\bullet k}\,\mathrm{Antagonism}_{jk}.
\]

- **Mean fragility (\(\mathbb{E}[F_i]\))**: Higher average shortfall (low \(F\)) means overall instability.  
- **Variance (\(\mathrm{Var}(F_i)\))**: Large dispersion of fragility (social gaps) raises systemic risk.  
- **Anchor Antagonism**:  \(\mathrm{Antagonism}_{jk}\) captures conflict between anchors \(j,k\) (e.g. if anchor \(j\) for some groups undermines anchor \(k\) for others). We penalize strong cross-correlations of high-risk anchors, weighted by how many people rely on them (\(b_{\bullet j}b_{\bullet k}\)).  

Thus \(C\) grows if (a) average continuity falls, (b) some subgroups are much more fragile than others, or (c) anchors are mutually destructive.  This reflects that a healthy society has **high average confidence in survival and meaning, low inequality of confidence, and low antagonism** across anchor groups.  

**Example (two-anchor case):** Suppose anchors 1 and 2. Write each person’s score \(F_i = b_{i1}(x_{i1}-t_1) + b_{i2}(x_{i2}-t_2)\).  Then one could define, for instance,  
\[
C \;=\; \alpha\big(\overline{t} - \overline{x}\big) + \beta\,\mathrm{Var}_i(F_i) + \gamma\,|\rho_{12}|,
\] 
where \(\overline{x},\overline{t}\) are population means of anchor values and threats, and \(\rho_{12}\) is the correlation of exposure to threats 1 and 2 across groups. Each term penalizes a different risk: first-term penalizes *average loss of future-oriented utility*, second penalizes *unequal shock distribution*, third penalizes *conflicting identities*.  

## Civilizational Cost Function Terms  

1. **Baseline fragility (\(\mathbb{E}[F_i]\))**:  If mortality or existential salience grows (e.g. war, pandemic, economic collapse), all anchors tied to that threat lose value, dropping average \(F\). This term ensures we treat outright danger as costly.  

2. **Variance term (\(\mathrm{Var}(F_i)\))**:  Societies with uneven portfolios (some highly anchored, others unanchored) can face worse outcomes. High variance means some people are much more threatened. This term makes the cost sensitive to **inequality** of stability.  

3. **Antagonism term (\(\sum_{j<k} \dots\))**:  If large subpopulations rely on anchor \(j\) and other groups on anchor \(k\), and these anchors clash (e.g. national vs religious identity), instability is magnified. We model this via a matrix of antagonism or correlation between anchors. Eroding one anchor might then polarize against another. Penalizing the magnitude of these cross-terms captures that fragmentation **amplifies** risk.  

These terms align with real-world observations: crises often hit hardest where social cohesion is weak or identities compete【13†L237-L245】【46†L1079-L1087】. For example, during an economic shock, wealth‐based anchor destruction (unemployment, financial loss) triggers both concrete insecurity *and* a sense of lost purpose【46†L1120-L1128】【45†L1-L4】.  The cost function formalizes these forces so that interventions can be evaluated by their net effect on \(C\).

