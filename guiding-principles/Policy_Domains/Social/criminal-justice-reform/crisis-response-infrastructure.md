---
id: crisis-response-infrastructure
title: Crisis Response Infrastructure — Fourth Dispatch Framework
sidebar_label: Crisis Response Infrastructure
sidebar_position: 1
slug: /criminal-justice/crisis-response-infrastructure
domain: Criminal_Justice
subdomain: Prevention_Layer
policy_type: Crisis Response Framework
status: Draft
version: 0.2
author: Futures Project
dependencies:
  - ssi-self-sovereign-identity-framework
  - upi-privacy-preserving-payment-rail
  - immutable-government-ledger
  - healthcare-enabled-housing-pilot-v2
  - housing_workforce_stabilization_pilots_v2
  - housing_arrival_transition_stack_v2
  - homelessness-prevention-automatic-stabilizer
  - department-of-data-and-accountability
related_initiatives:
  - community-stabilization-framework
  - non-violent-rehabilitation-framework
  - school-and-neighborhood-stabilization
non_goals:
  - replacement of police, fire, or EMS
  - mandatory dispatch overrides
  - federal control of local dispatch decisions
  - punitive framing for callers seeking help
  - surveillance of crisis callers beyond operational necessity
  - forced treatment without consent
tags:
  - criminal-justice
  - crisis-response
  - mental-health
  - substance-use
  - homelessness
  - dispatch
  - prevention
  - opt-in
  - denver-star
last_updated: 2026-03-29
---

# Crisis Response Infrastructure
## Fourth Dispatch Framework — National Opt-In Expansion

---

## Executive Summary

American emergency dispatch currently offers three response options: police, fire, and EMS. For a significant share of 911 calls — mental health crises, substance use emergencies, homelessness-related distress, non-violent domestic disturbances — none of the three is the appropriate primary response. Police are trained for law enforcement, not behavioral health. Fire and EMS are trained for medical emergencies, not psychiatric stabilization or substance use support.

The result is systematic over-policing of situations that do not require law enforcement and systematic under-serving of individuals who need clinical or social support. Unnecessary police involvement in mental health and substance use calls produces bad outcomes for individuals, erodes community trust, and consumes law enforcement resources that are needed elsewhere.

This framework establishes a **fourth dispatch option**: a trained crisis response team — comprising behavioral health clinicians, peer support specialists, and social workers — available as the primary or co-response unit for defined call types. Crisis response teams are not police. They do not carry weapons. They do not have arrest authority. They exist to provide appropriate care to people in crisis.

The framework is explicitly **opt-in for jurisdictions**. Federal support — funding, training standards, data infrastructure, and outcome measurement — is available to any jurisdiction that adopts the framework. No jurisdiction is required to participate. Jurisdictions that participate retain full control over local implementation within defined quality standards.

The framework is also explicitly **safe for callers**. Rather than creating a new number, this framework builds dispatch capability behind **988** — the national Suicide and Crisis Lifeline launched in 2022, which currently connects callers to mental health counselors but does not yet have standardized crisis team dispatch attached to it. This framework gives 988 teeth: an actual team that can show up, not just a phone counselor. The design principle is simple: if someone is scared to call because they fear the consequences of police involvement, they will not call. A number that already exists, is already being marketed as safe, and now has real dispatch capacity behind it is the right architecture — building on existing infrastructure rather than asking the public to learn a new number.

---

## The Denver STAR Evidence Base

The Denver Support Team Assisted Response (STAR) program is the primary evidence base for this framework. Launched in 2020, STAR deploys a mental health clinician and a paramedic in response to low-acuity behavioral health calls that would otherwise receive police response.

Key outcomes from Denver STAR:
- In the first six months, STAR responded to over 700 calls with zero instances requiring police backup
- No arrests were made during STAR responses in the program's first year
- Calls handled by STAR freed equivalent police time for calls requiring law enforcement response
- Participant surveys showed high rates of reported helpfulness and willingness to call again
- Cost per STAR response was significantly lower than cost per police response for equivalent call types

Similar programs in Eugene, Oregon (CAHOOTS, operating since 1989), Olympia, Washington, and several other cities show consistent results: behavioral health crisis calls handled by trained non-police responders produce better outcomes for individuals, lower costs, and no increase in safety incidents.

The evidence base is sufficient to justify national opt-in expansion. It is not sufficient to justify federal mandate — local implementation conditions vary, and the opt-in framework preserves the experimentation and adaptation that has made these programs successful.

---

## Core Design Principles

**Fourth option, not replacement:** Crisis response teams operate alongside police, fire, and EMS — not instead of them. Police remain available for law enforcement situations. Crisis response teams handle calls where law enforcement is not the appropriate primary response.

**Default to crisis response for ambiguous non-violent calls:** Dispatch logic defaults to crisis response for calls that present as non-violent, even when ambiguous. The failure mode of defaulting to police — the teenager who doesn't call because they fear arrest, the person in psychiatric crisis who escalates when confronted by armed officers — is worse than the failure mode of dispatching a crisis team to a call that turns out to need police backup. Backup is always available and always fast.

**Safe to call:** The routing architecture is designed to feel like calling for help, not calling to report yourself. No automatic police notification for crisis line calls. No record shared with law enforcement unless a safety threshold is crossed. The caller's decision to seek help is not used against them.

**Opt-in with quality standards:** Jurisdictions choose to participate. Participation requires meeting defined training, staffing, and data reporting standards. Federal support flows to participating jurisdictions. Non-participating jurisdictions retain their existing systems.

**Connected to the stabilization ecosystem:** Crisis response teams are not a standalone intervention. They are the front door to the broader stabilization ecosystem — connected to the arrival/transition stack, the workforce stabilization pilots, the healthcare-enabled housing pilot, and the homelessness prevention ERA system. A crisis response is not successful if it ends with the individual returned to the same conditions that produced the crisis.

---

## The Fourth Dispatch Option

### Call Types in Scope

Crisis response teams are the default primary dispatch for calls presenting as:

**Mental health crisis:** Suicidal ideation, psychiatric episode, emotional distress, erratic behavior without weapon involvement, welfare checks for individuals with known mental health history.

**Substance use crisis:** Active intoxication without violence, overdose (co-dispatched with EMS), substance use-related distress, requests for harm reduction support.

**Homelessness-related calls:** Individual in distress related to housing instability, encampment welfare checks, calls about individuals who appear unwell in public spaces.

**Non-violent domestic disturbance:** Verbal conflict without weapon involvement or physical violence, family crisis, calls where the reporting party explicitly requests non-police response.

**Discretion-weighted ambiguous calls:** Calls that could be any of the above but present ambiguously. Dispatch applies a non-violence presumption — if the call does not present active violence or weapon involvement, crisis response is the default primary unit. Police are notified and available but do not respond unless requested by the crisis team or unless the situation presents new safety information.

**Explicitly out of scope:**
- Active violence or weapon involvement — police primary, crisis team may co-respond if requested
- Medical emergency without behavioral health component — EMS primary
- Property crime — police primary
- Any call where the reporting party requests police specifically

### Dispatch Logic

```
911 CALL RECEIVED
      │
      ▼
Does call present active violence
or weapon involvement?
      │
   YES → Police primary dispatch
         Crisis team notified, available if requested
      │
   NO  ▼
Does call present medical emergency
without behavioral health component?
      │
   YES → EMS primary dispatch
         Crisis team notified, available if requested
      │
   NO  ▼
Default → Crisis Response Team primary dispatch
          Police notified, available if requested
          EMS notified, available if requested
          │
          ▼
Crisis team assessment on scene
          │
      ┌───┴───┐
      │       │
 Situation   Situation escalates
 resolved    or safety concern identified
      │             │
      ▼             ▼
 Stabilization   Police/EMS
 pathway         requested
 connection
```

### 988 — Crisis Routing and Dispatch Integration

988 launched in 2022 as the national Suicide and Crisis Lifeline — a three-digit number connecting callers to mental health counselors via call, text, or chat. It is relatively unknown but already exists, is already safe-framed, and already has infrastructure behind it. The gap is that 988 currently provides phone support without standardized crisis team dispatch capability. This framework closes that gap.

**988 as the dispatch layer for crisis response:**
- 988 becomes the front-door routing number for crisis team dispatch in participating jurisdictions
- Callers reach a trained crisis counselor first — the same model as today
- Counselors can dispatch a crisis response team with caller consent
- 911 remains available and crisis teams remain dispatchable from 911 — 988 is an additional safe pathway, not a replacement

**Design principles:**
- No automatic police notification for 988 calls
- Caller identity is not recorded or shared with law enforcement unless a defined safety threshold is crossed — imminent threat to life of caller or a specific third party
- ZKP consent model applies — callers may optionally verify identity and eligibility attributes without disclosing personal data (see SSI and ZKP section below)
- The line is marketed as a safe alternative — not a backdoor to police involvement
- 988 awareness is a federal public communication priority — the number is only useful if people know it exists

**Why 988 rather than a new number:**
Creating a new routing number requires public education from zero. 988 already exists, already has a safe-to-call brand, and is already being promoted by SAMHSA and state mental health agencies. Building dispatch capability behind 988 leverages existing infrastructure and existing awareness rather than splitting the public communication effort.

**The failure mode this prevents:** A teenager who has been drinking and is having a bad reaction does not call 911 because they fear arrest. A person in a mental health crisis does not call because they or a family member has had a bad police encounter. A person experiencing homelessness does not call because they expect to be moved on rather than helped. 988 exists because these populations need a number they will actually call — and this framework ensures that calling it actually sends someone who can help.

---

## Team Composition and Training

### Core Team Model

The crisis response team model draws from Denver STAR, CAHOOTS, and international evidence on effective co-response models. The core team for a standard deployment is a two-person unit:

**Behavioral Health Clinician:** Licensed mental health professional (LCSW, LPC, or equivalent) with specific training in crisis intervention, de-escalation, trauma-informed care, and substance use assessment. Not a peer support specialist — a licensed clinician with assessment authority.

**Peer Support Specialist:** Individual with lived experience of mental health or substance use challenges, certified as a peer support specialist. The peer role is evidence-backed — individuals in crisis are more likely to engage with someone who has shared experience. Peer specialists are not clinical staff; they work alongside the clinician.

**Optional co-response additions by call type:**
- Paramedic for calls with potential medical component
- Housing navigator for homelessness-related calls — with direct connection to the arrival/transition stack and stabilization pilots
- Substance use counselor for substance use calls in jurisdictions with this capacity

### Training Standards

Federal training standards are a condition of funding eligibility. Standards define minimum competencies, not curriculum — jurisdictions may develop their own training programs that meet the competency framework.

**Required competencies:**
- Crisis intervention and de-escalation
- Trauma-informed care
- Mental health first aid and psychiatric assessment
- Substance use recognition and harm reduction
- Motivational interviewing
- Warm handoff protocols to downstream stabilization services
- Physical safety awareness (recognizing when to request police backup)
- Documentation and outcome reporting consistent with DoDa standards

**Training hours:** Minimum 200 hours pre-deployment, including supervised field hours. Ongoing continuing education requirements consistent with clinical licensure standards.

---

## Routing to the Stabilization Ecosystem

Crisis response teams are the front door to the broader stabilization system. A crisis response that ends without a connection to downstream support has partially succeeded — the immediate crisis is resolved — but has not addressed the conditions that produced it.

**Warm handoff protocols:**

*Mental health crisis → Healthcare-Enabled Housing Pilot:* Individuals presenting with chronic mental health needs and housing instability are assessed for healthcare-enabled housing eligibility during or immediately following the crisis response. The crisis team carries direct referral access to the healthcare-enabled housing intake system.

*Substance use crisis → Treatment and harm reduction:* Individuals in substance use crisis are offered warm handoffs to treatment, harm reduction services, and where relevant, housing stabilization. The crisis team does not compel treatment — engagement is voluntary. The offer is made and the connection is facilitated.

*Homelessness-related calls → Arrival/Transition Stack and Stabilization Pilots:* Individuals experiencing homelessness are connected to the appropriate tier of the stabilization system based on triage. The crisis team carries a housing navigator on homelessness-related calls specifically for this handoff.

*ERA trigger flag:* Where a crisis call involves an individual who may be at risk of eviction or housing loss, the crisis team can flag the individual for ERA eligibility screening — with consent — connecting the crisis response to the homelessness prevention automatic stabilizer.

*Workforce stabilization → Transitional housing:* Individuals who are workforce-capable but in situational crisis are connected to the workforce stabilization track. The crisis team triage protocol mirrors the shared triage protocol used across the stabilization system.

All warm handoffs are recorded in the DoDa outcome tracking system — with appropriate privacy protections — to enable measurement of whether crisis responses result in stable downstream connections.

---

## Infrastructure Integration

### SSI Integration — Phased Approach

SSI is not a day-one dependency for crisis response. The framework operates without it in early phases and integrates SSI as enrollment scales. The phasing is explicit:

**Near term — Medicaid as primary sustainability mechanism:**
Clinical services delivered by licensed clinicians during crisis response are Medicaid-reimbursable in many states today. This is the primary funding sustainability mechanism available immediately — no SSI required. Participating jurisdictions identify Medicaid billing pathways for crisis response clinical services as part of Phase 0 infrastructure setup.

**Medium term — SSI as optional identity layer:**
As SSI enrollment scales nationally, crisis response interactions become connectable to verified identity — with consent. An individual who has an SSI credential and chooses to share it during a crisis contact enables the team to access prior warm handoff history, flag ERA eligibility, and connect to stabilization services without re-intake burden. Consent is always required. SSI verification is never compelled.

**Long term — SSI as seamless ecosystem connector:**
At sufficient SSI enrollment, a person in crisis who consents to SSI verification gets connected to their full stabilization pathway in one interaction — housing history, ERA eligibility, healthcare-enabled housing referral, workforce stabilization track — without proving identity again at each step. The crisis response becomes the single point of contact for the entire stabilization ecosystem.

### Zero-Knowledge Proof Consent — Trust by Design

The ZKP consent model is the mechanism that makes SSI integration trustworthy for exactly the populations most likely to be in crisis.

The people most likely to call a crisis line are also the people most likely to have experienced harm from data sharing across institutions — mental health records affecting employment, substance use history affecting custody, crisis contacts appearing in background checks. Every prior "let's share data across agencies to help people" initiative has foundered on this trust problem. ZKP resolves it structurally, not through policy promises.

**How ZKP consent works in a crisis interaction:**

The individual controls what gets proven, not what gets shared. Specific examples:

- *"I am eligible for housing stabilization services"* — proven, without revealing income level, address history, or prior crisis contacts
- *"I have an active ERA eligibility window"* — proven, without revealing why the window was triggered or what the triggering event was
- *"I am enrolled in Medicaid"* — proven, without revealing diagnosis, treatment history, or provider
- *"I am over 18"* — proven, without revealing date of birth or any other attribute

Nothing beyond the proven fact is disclosed. The crisis team receives confirmation of the relevant eligibility condition. They do not receive a file. They do not receive a history. They receive exactly what they need to connect the person to the right service.

**Why this builds trust specifically in this population:**

A person in a mental health crisis who understands that consenting to a ZKP means "they can connect me to housing support" — and not "they now have access to my psychiatric history, which will follow me" — is far more likely to consent. And far more likely to call in the first place.

The trust effect compounds. Each positive interaction where the ZKP model works as described — person consents, gets connected to services, experiences no downstream data leakage — becomes social proof that the system is safe to use. That social proof spreads through exactly the networks where crisis response trust is lowest and most needed.

**ZKP consent as a design principle for the criminal justice domain:**

This is not specific to crisis response. Every point in the criminal justice domain where an individual interacts with a system that could use their data against them is a point where ZKP consent can replace data disclosure. The crisis response framework is the first implementation of this principle — subsequent criminal justice briefs will reference it explicitly.

### IGL Integration

Every crisis response generates a ledger entry: pseudonymous credential reference (where SSI verification occurred with consent), call type category, response unit composition, outcome category (resolved, escalated, warm handoff completed), and timestamp. No personal data, no call content, no individual identifying information beyond the pseudonymous reference.

The IGL record enables:
- DoDa outcome tracking across the full crisis response system
- Fraud detection for any financial transactions associated with crisis response (coordination payments, ERA triggers)
- Permanent audit record of program performance

### DoDa Outcome Tracking

DoDa publishes quarterly aggregate outcome reports for participating jurisdictions:
- Total crisis responses by call type
- Escalation rate (calls requiring police or EMS backup)
- Warm handoff completion rate
- 30-day re-contact rate (indicator of stabilization success)
- Cost per crisis response vs. equivalent police response
- ERA trigger rate from crisis contacts

These metrics are the evidence base for program expansion and the accountability mechanism for federal funding.

---

## Capital and Funding Model

### Federal Support Structure

Federal funding flows to participating jurisdictions through a tiered grant structure:

**Tier 1 — Startup grant:** Covers team recruitment, training, vehicle and equipment, and first-year operations for new crisis response programs. Available to any jurisdiction meeting baseline eligibility (population threshold, dispatch infrastructure, data reporting commitment).

**Tier 2 — Sustaining grant:** Annual operating support for established programs meeting defined outcome standards. Outcome standards are published in advance and applied mechanically — not subject to discretionary review.

**Tier 3 — Excellence incentive:** Additional funding for programs demonstrating exceptional outcomes on defined metrics — high warm handoff completion rates, low escalation rates, measurable reductions in repeat crisis contacts.

Funding is disbursed through UPI to participating jurisdiction accounts and recorded on the IGL.

### Local Funding Sustainability

Federal startup grants are designed to demonstrate financial viability, not to create permanent federal dependency. Participating jurisdictions are expected to transition toward local funding sustainability within a defined window, supported by:

- Documented cost savings from reduced police response to behavioral health calls
- Medicaid reimbursement for clinical services delivered during crisis response (where legally eligible)
- Reduced emergency department utilization costs shared with hospital systems

The cost offset case is strong — the per-response cost of a crisis team is substantially lower than the per-response cost of police, and the downstream cost reductions (avoided hospitalization, avoided incarceration, avoided repeat crisis) are measurable through DoDa outcome tracking.

---

## Opt-In Framework and Local Authority

### Jurisdiction Eligibility

Any municipality, county, or state may opt into the framework. Eligibility requires:

- Commitment to defined training standards for crisis response staff
- Integration with existing 911 dispatch infrastructure
- Data reporting to DoDa outcome tracking system
- Public designation of the program with consistent branding standards (no stigma signaling)

### What Jurisdictions Control

Participating jurisdictions retain full control over:
- Team composition within the core model parameters
- Call type definitions within the defined scope (may be more restrictive, not more expansive than the federal framework)
- Local referral networks and stabilization pathway connections
- Staffing levels and deployment geography within their jurisdiction
- Local labor agreements and employment terms

### What Federal Standards Govern

Federal standards define the minimum quality floor:
- Training competency requirements
- Data reporting format and cadence
- Safe-to-call routing requirements for direct crisis line
- Escalation protocol minimums (when police/EMS must be notified)
- Privacy protections for crisis callers

### Expansion Pathway

Jurisdictions that demonstrate successful outcomes are eligible for expanded federal support and are designated as technical assistance providers for new programs in neighboring jurisdictions. The knowledge transfer function — experienced programs helping new programs implement — is a funded activity, not a volunteer expectation.

---

## Phased Implementation

### Phase 0 — Standards and Infrastructure
Federal training competency framework published. DoDa outcome tracking system built. IGL integration with crisis response dispatch systems designed. 988 dispatch integration architecture designed with SAMHSA. Medicaid billing pathway guidance published for participating jurisdictions. Federal grant structure established.

### Phase 1 — Pilot Expansion
Existing programs (Denver STAR, CAHOOTS, and equivalents) formally enrolled in the federal framework. Data reporting standards implemented. Outcome baseline established. 988 dispatch capability piloted in participating jurisdictions. Medicaid reimbursement for crisis clinical services activated where eligible. First new programs funded in jurisdictions with demonstrated readiness.

### Phase 2 — Broad Opt-In
Federal grant availability publicized nationally. Technical assistance from Phase 1 programs available to new jurisdictions. 988 dispatch integration operational across participating jurisdictions. Stabilization ecosystem connections (ERA trigger, warm handoff protocols) live. SSI optional consent layer available where SSI enrollment is sufficient — ZKP consent model piloted with willing participants.

### Phase 3 — Normalization
Crisis response teams are a standard feature of emergency dispatch in participating jurisdictions. 988 is broadly known as the safe crisis line with real dispatch capability behind it. SSI integration enables seamless stabilization pathway connections for consenting individuals. Outcome data is sufficient to demonstrate cost effectiveness and safety. Non-participating jurisdictions face documented evidence of what their residents are missing. Opt-in rate drives toward broad national coverage through demonstrated value rather than mandate.

---

## Performance Metrics

**Safety:**
- Escalation rate requiring police backup (target: below 5% of crisis responses)
- Injury rate during crisis responses (crisis team and individuals)
- Serious incident rate

**Effectiveness:**
- Warm handoff completion rate (target: above 70%)
- 30-day re-contact rate
- 90-day housing stability for individuals connected to stabilization pathways
- ERA trigger rate from crisis contacts

**Equity:**
- Response time by neighborhood and demographic composition
- Call type distribution by jurisdiction — ensuring crisis response is not de facto limited to specific neighborhoods
- Caller willingness to call again (survey-based)

**Cost:**
- Cost per crisis response vs. equivalent police response
- Avoided emergency department utilization cost
- Avoided incarceration cost per individual connected to stabilization pathway

---

## Failure Modes

System degrades if:

- Crisis teams are sent to calls with active violence without police backup available — safety incident damages program credibility and suppresses future adoption
- 988 becomes associated with police involvement — callers stop using it and the access benefit is lost; the safe-to-call framing is the most fragile asset in the system
- 988 awareness remains low — the number is only useful if people know it exists; public communication is a funded requirement, not an afterthought
- ZKP consent model is implemented in ways that feel like surveillance — if individuals believe that consenting to a ZKP creates a file that can be used against them, they will not consent and the trust benefit is lost
- Warm handoff protocols are not funded — crisis teams resolve immediate situations but individuals return to the same conditions
- Medicaid billing pathways are not established in Phase 0 — programs become financially unsustainable when federal startup grants expire
- Data reporting requirements are so burdensome that small jurisdictions cannot comply — participation skews toward well-resourced municipalities
- Federal funding creates dependency without local sustainability planning — programs collapse when grant cycles end
- Program is branded or operated in ways that stigmatize users — individuals avoid calling even when the line is safe

---

## Relationship to Broader Criminal Justice Domain

The crisis response framework is the **prevention layer** of the criminal justice domain — the intervention that happens before an individual enters the formal justice system.

Its downstream connections are explicit:

- Individuals stabilized through crisis response and connected to healthcare-enabled housing or workforce stabilization tracks are less likely to cycle back through crisis response, emergency departments, and jails
- The warm handoff data tracked through DoDa provides the evidence base for the community stabilization framework — identifying which neighborhoods have the highest crisis response density and therefore the greatest need for environmental and third-space investment
- The non-violent crime rehabilitation framework benefits from reduced entry into the formal justice system — individuals whose substance use and mental health crises are resolved through crisis response rather than arrest do not acquire the criminal record that makes rehabilitation harder

The crisis response team is not a substitute for the rest of the criminal justice reform agenda. It is the front door that determines how many people need to walk through the rest of it.

---

## Meta Insight

The question "why are there only three things you can call in an emergency?" has no good answer. It is a historical accident — the three services that existed were the three services that got numbers. The population of people who need help in a crisis is not neatly divided into "needs police," "needs fire," and "needs EMS."

The fourth option is not radical. It exists in Denver, Eugene, and dozens of other cities. It works. The evidence is not ambiguous.

What has been missing is the national infrastructure — funding, training standards, routing architecture, outcome measurement, and stabilization ecosystem connections — that allows successful local experiments to become normal practice everywhere.

This framework provides that infrastructure.

The goal is simple: when someone is in crisis and reaches for a phone, there is always a number that feels safe to call, and always a team equipped to help them.

That is achievable. The infrastructure to achieve it is defined here.
