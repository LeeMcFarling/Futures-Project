---
id: maternal-family-care-hta-integration
title: Maternal and Family Care — HTA Integration and Postpartum Support Framework
sidebar_label: Maternal & Family Care
sidebar_position: TBD
slug: /healthcare/care-delivery/maternal-family-care-hta-integration
domain: Healthcare
subdomain: Care_Delivery_and_Insurance
policy_type: Cross-Domain Integration Framework
status: Draft
phase: 2
version: 0.1
author: Futures Project
last_updated: 2026-05-03
dependencies:
  - care-delivery-market-design
  - insurance-architecture-sec
  - sec-administration-heta-steady-state
  - healthcare-infrastructure-layer
  - employer-sponsored-coverage-transition
  - permanent-health-security-accounts
  - benefits-gradient-modernization
  - portable-healthcare-contribution-floor
  - regional-health-center-network
  - cost-performance-backstop
  - department-of-data-and-accountability
  - ssi-self-sovereign-identity-framework
  - upi-privacy-preserving-payment-rail
related_initiatives:
  - maternal-health-access-standard
  - postpartum-recovery-center-certification
  - child-future-accounts
  - family-care-envelope
  - primary-care-market-design
  - labor-stack-enforcement-framework
tags:
  - healthcare
  - maternal-care
  - family-care
  - pregnancy
  - postpartum
  - hta
  - sec
  - price-transparency
  - family-formation
  - employer-contributions
  - app-routing
  - ssi
  - upi
---

## Purpose and Scope

This brief defines how maternal, prenatal, postpartum, newborn, and family-formation
care integrate with the Health Transition Account structure, Severe Event Coverage,
the healthcare app, and the employer healthcare contribution framework. The purpose
is to convert pregnancy and early family formation from a fragmented billing sequence
into a priced, routed, and risk-stratified care pathway.

Five rules govern the framework. Emergency, acute, medically necessary, and
hospital-based birth events are covered through SEC. Routine prenatal, postnatal,
newborn-support, lactation, pelvic-floor, doula, parent-education, and
postpartum-support services operate in the market layer where they are predictable,
schedulable, and price-comparable. These market-layer services are discoverable,
priced, and settled through the integrated healthcare app and HTA rails. Pregnancy,
birth, adoption, and early newborn care may activate a time-bounded Family Care
Envelope with higher contribution limits than ordinary individual HTA use. And
certified postpartum recovery centers may operate as hospital-adjacent, lower-acuity
support infrastructure, reducing unnecessary hospital-bed use while preserving rapid
escalation access if complications arise.

This brief does not create a separate maternal insurance program. It does not make
families save for emergency care. It does not move birth complications into HTA
accounts. It defines how predictable maternal and family-care services are financed,
displayed, settled, and measured while preserving SEC as the universal severe-event
floor.

---

## Problem Statement

Maternal care in the current U.S. healthcare system is structurally fragmented.
Pregnancy is predictable as a life event, but the system treats it as a sequence of
disconnected encounters: preconception advice, prenatal visits, labs, scans,
specialist referrals, hospital delivery, postpartum discharge, pediatric onboarding,
lactation support, mental-health screening, and newborn follow-up. Each step may
involve different providers, different portals, different bills, different coverage
rules, and different levels of price visibility. The result is uncertainty at exactly
the wrong moment.

A family planning for a child often cannot know in advance which services are
available, how much routine support will cost, what insurance will cover, what their
employer contribution is worth, whether postpartum help is accessible, or how
emergency complications will be handled financially. The family discovers the price
of becoming a family one bill at a time.

This is not merely a consumer inconvenience. It is a care-delivery failure.
Fragmented maternal care weakens early intervention, increases missed postpartum
risk, hides access gaps, obscures price variation, and makes it difficult to evaluate
which supports reduce severe-event escalation, readmissions, postpartum depression,
breastfeeding failure, emergency utilization, or newborn complications.

The reformed healthcare stack creates the tools to correct this. SEC protects against
emergency, acute, medically necessary, and high-cost events. HTA accounts provide
portable liquidity for routine market-layer care. The healthcare app provides
discovery, routing, price display, scheduling, eligibility verification, and
settlement. SSI and UPI provide privacy-preserving identity and payment rails. DoDA
provides independent measurement of access, cost, outcomes, and severe-event risk
attenuation. The missing piece is a maternal and family-care integration rule.

---

## Core Design Principle

Pregnancy is a predictable care pathway with catastrophic tail risk. The predictable
pathway should be priced, routed, and supported through transparent healthcare rails.
The catastrophic tail risk should be pooled through SEC. Families should never have
to save for emergency care. They should be able to save and plan for the kind of
pregnancy, recovery, and early-family support pathway they want.

---

## Domain Placement

SEC covers maternal, birth, and newborn events when the clinical situation is
emergency, acute, medically necessary, non-elective, high-cost, or hospital or
procedural in nature. This includes emergency pregnancy complications, emergency
department visits related to pregnancy or postpartum, labor and delivery hospital
episodes, medically necessary and emergency C-sections, hemorrhage, hypertensive
crisis, severe preeclampsia and eclampsia, sepsis and serious infection, pulmonary
embolism and other acute thrombotic events, acute cardiac events during pregnancy or
postpartum, medically necessary anesthesia, inpatient maternal stabilization,
neonatal intensive care, emergency newborn stabilization, medically necessary
readmissions, acute postpartum psychiatric crisis, and other maternal or newborn
episodes meeting SEC clinical trigger definitions. SEC applies at the episode level.
HTA balances are not drawn down for SEC-covered events. The governing test is
clinical urgency, medical necessity, and non-shoppability. Families do not
self-insure emergency pregnancy risk.

Market-layer maternal and family-care services include preconception consultation,
fertility-awareness counseling where non-procedural and routine, routine prenatal
visit packages, standard prenatal labs and screening where market-layer
classification applies, routine scan routing where not part of an SEC-covered
episode, childbirth education, birth planning, doula support, lactation consultation,
prenatal nutrition counseling, pelvic-floor physical therapy, routine postpartum
checkups, postpartum mental-health screening and outpatient therapy, sleep and
newborn-care education, parent education, home-visiting support where non-acute,
postpartum recovery-center stays, parent cohorts and family-support groups,
transportation support where authorized, routine newborn orientation and care
navigation, and non-acute pediatric onboarding services. These services may be paid
through HTA balances, family-care envelopes, income-graduated subsidies, employer
family contributions, individual contributions, or approved public credits. They are
not SEC-covered merely because they are important. SEC is preserved for severe,
acute, medically necessary, non-elective, and high-cost clinical events.

---

## Family-Formation Planning Pathway

When an individual tells a primary-care provider, OB/GYN, midwife, fertility
provider, or other certified clinician that they are planning a pregnancy, the
healthcare app activates a Family-Formation Planning Pathway.

The pathway produces a local, plain-language planning packet covering recommended
preconception steps, local prenatal-care options across OB, midwife, doula,
lactation, pelvic-floor, mental-health, and postpartum providers, the expected care
timeline from preconception through one year postpartum, SEC-covered services and
events, HTA-eligible services, estimated family exposure under available care
packages, available employer contributions and public subsidies, expected HTA
drawdown, postpartum recovery-center options, parent cohort options, transportation
and language-access supports, escalation instructions for urgent symptoms, and
risk-stratified routing where clinically indicated.

The packet is printable, shareable, and available in the app. A clinician can
generate it during a normal visit. The purpose is not to force a single pathway. The
purpose is to make the pathway visible before the family is inside the event.

---

## Maternal Care Package Display

The app displays standardized maternal and family-care packages that are comparable
enough to evaluate and flexible enough to preserve genuine choice.

The Baseline Maternal Pathway includes a preconception visit, routine prenatal visit
schedule, standard lab and screening schedule, routine scan routing, birth planning,
postpartum checkup, lactation consultation, postpartum mental-health screening,
newborn-care orientation, and parent cohort placement.

The Supported Recovery Pathway adds doula support, expanded lactation support,
pelvic-floor physical therapy, nutrition counseling, postpartum mental-health
check-ins, a home visit, a short postpartum recovery-center stay, and enhanced parent
cohort programming.

The High-Support Family Pathway extends further to include a longer postpartum
recovery-center stay, additional home visits, more intensive lactation and
newborn-care support, expanded mental-health support, caregiver coaching, and
transportation, language-access, and disability-access supports where needed.

Where clinical risk is elevated, the app does not present routine packages as
substitutes for medical care. A Risk-Stratified Clinical Pathway may include
maternal-fetal medicine referral, higher-frequency monitoring, specialist
coordination, hospital delivery planning, SEC episode-boundary explanation,
emergency escalation instructions, postpartum complication monitoring, and newborn
risk routing. Risk stratification guides clinical routing. It does not deny
market-layer support or shift emergency risk into HTA accounts.

---

## Price Transparency and App Display

Maternal and family-care services appear in the same public portal used for other
market-layer care. For each covered service or package, the app displays the provider
or facility name, credential and certification status, posted price, standard service
definition, package inclusions and exclusions, local median price, local percentile
range, patient net price after available credits, HTA drawdown estimate, Family Care
Envelope balance and contribution estimate, employer contribution availability, public
subsidy availability, available appointment windows, distance and transportation
options, language access, accessibility status, patient-reported experience metrics
where validated, outcome and safety indicators where validated, hospital escalation
affiliation where relevant, and whether the provider accepts UPI settlement.

No provider may pay for ranking placement. Ranking logic prioritizes fit,
availability, price, quality, access, and safety. Sponsored placement, hidden
steering, and vertically integrated self-preferencing are prohibited unless clearly
labeled and independently justified by validated outcome data.

---

## HTA Eligibility Rule

Market-layer maternal and family-care services are eligible for payment through HTA
accounts and authorized Family Care Envelopes. Eligible funding sources include
individual HTA balances, employer healthcare contribution deposits, elevated
family-care employer contributions, individual or household contributions,
income-graduated routine-care subsidies, public maternal-care credits, public child
health reserve contributions, and approved philanthropic or local access credits.

The rail combines these sources at settlement. The provider receives confirmed
payment, standardized service code, and settlement status. The provider does not see
the patient's account balance, employer contribution status, public subsidy amount,
family contribution level, income status, or payer mix. The patient sees the full
breakdown through the app.

---

## Medicaid Function — Automated Affordability Layer

This framework preserves Medicaid's affordability function while changing how
that function is administered for market-layer care.

Under this framework, Medicaid-derived support does not operate as a separate
bureaucratic coverage silo for market-layer maternal and family-care services.

For eligible households, Medicaid functions as an automated affordability layer
applied through the healthcare rail. Income eligibility is verified through
privacy-preserving attestation. Clinical-need adjustments, where authorized, are
verified through purpose-bound health attestations. The rail applies the relevant
discount, credit, or family-envelope enhancement at settlement.

The patient sees the net price before booking and at checkout. The provider receives
the confirmed settlement amount and standardized service code. The provider does not
see Medicaid status, income tier, subsidy amount, clinical-condition attestation, or
payer mix.

This design preserves the redistributive function of Medicaid while removing the
legacy administrative form: separate enrollment pathways, provider stigma, narrow
networks, reimbursement friction, cliff effects, and manual claims adjudication.

Medicaid becomes a rule in the rail, not a maze around the patient.

---

## Family Care Envelope

Pregnancy, birth, adoption, newborn care, and defined family-care events may activate
a time-bounded Family Care Envelope. The envelope is not a separate insurance
product. It is a temporary account structure that allows individual, employer, public,
and household funds to be used for certified family-care needs. It may be activated
for pregnancy, birth, adoption, foster placement where authorized, newborn care,
serious pediatric routine-care needs, disability-related dependent care where
market-layer services apply, and other certified caregiving events authorized by
statute. It allows higher contribution caps than ordinary individual HTA use during
the relevant life event. It does not replace SEC — emergency and medically necessary
acute care remains SEC-covered.

The envelope may draw from or coordinate among the pregnant individual's HTA, the
other parent's HTA where authorized, a child-linked health account after birth,
employer family-care contributions, public family-care credits, household
contributions, and approved local or philanthropic credits. Funds remain governed by
ownership and fiduciary rules. The envelope is a spending and planning interface, not
a transfer of ownership unless statute authorizes a specific transfer.

---

## Family Contribution Stratification

The HTA architecture distinguishes between individual routine-care contributions and
family-care contributions. Ordinary individual contributions support routine
individual healthcare needs. Family-care contributions support certified household
life events including pregnancy, birth, adoption, and early newborn care. This
distinction is necessary because family formation creates predictable, time-bounded,
household-level expenses that do not fit cleanly inside a single adult's ordinary
annual routine-care cap.

This mirrors the existing logic of family insurance. Employers already contribute
differently for individual, spouse, child, and family coverage. The reform does not
invent a new family-support obligation. It converts the family-insurance premium
function into transparent, portable, account-based purchasing power. Under the legacy
model, the employer pays opaque family premiums into a plan. Under the HTA model,
the employer contributes visible family-care dollars into a portable account
architecture while SEC covers emergency and medically necessary acute care.

---

## Transition-Period Elevated Caps

During the transition from employer-sponsored insurance to SEC plus HTA, family-care
contribution caps are temporarily elevated for certified family-care events. The
purpose is to avoid stranding families while legacy employer insurance obligations
decline and the new HTA market matures. Elevated caps may apply to pregnancy
planning, prenatal care, postpartum support, newborn onboarding, postpartum
recovery-center stays, lactation support, pelvic-floor therapy, parent cohorts,
home-visiting support, and other certified family-care services.

Elevated caps phase down as SEC coverage stabilizes, provider prices become legible,
routine maternal-care markets mature, and baseline family-care reserves become
adequate. They are not a permanent tax shelter. Guardrails include certification of
eligible family-care event, time-bounded activation, use restriction to authorized
care categories, income-sensitive public top-ups, prospective tapering above
sufficiency thresholds, provider-side blindness to balances, DoDA monitoring of
distributional effects, and automatic phase-down unless renewed by evidence.

---

## Postpartum Recovery Centers

Certified Postpartum Recovery Centers may operate as hospital-adjacent, lower-acuity
recovery and support facilities. Their purpose is to provide humane, structured
postpartum support without using high-cost hospital beds for patients who are
medically stable but not yet well-supported at home.

These centers may provide rest and recovery space, meals and basic recovery support,
lactation support, newborn-care education, postpartum mental-health screening,
blood-pressure monitoring, C-section wound observation within defined scope, bleeding
and infection symptom monitoring, sleep and feeding support, parent education, care
navigation, cohort formation, and escalation routing to hospital care. They are not
hospitals. They do not provide emergency care, surgery, intensive care, or acute
stabilization beyond their certified scope. Their value comes from adjacency — a
center located near or physically connected to a hospital can reduce unnecessary
inpatient stay length while preserving rapid escalation access if complications arise.

HETA, in coordination with state regulators and DoDA-certified measurement standards,
defines certification requirements covering staffing ratios, credential requirements,
scope-of-practice limits, maternal and newborn monitoring protocols, lactation and
mental-health screening standards, emergency escalation triggers, transfer protocols,
hospital affiliation or adjacency requirements, price transparency, package
disclosure, infection-control standards, patient rights, and data reporting.
Postpartum centers must not become liability arbitrage vehicles. Hospitals may not
use them to discharge clinical responsibility prematurely.

Centers may offer tiered accommodations, but the clinical baseline must be protected.
A certified baseline stay includes the core recovery, monitoring, education,
lactation, mental-health screening, and escalation functions. Optional upgrades may
include larger rooms, additional amenities, or premium hospitality features. SEC,
HTA, public credits, and family-care envelopes support the certified baseline.
Families may purchase optional upgrades with private funds. The public architecture
does not recreate postpartum support as a luxury product.

---

## Parent Cohorts and Family Support Groups

Postpartum Recovery Centers and participating community providers organize parent
cohorts. Cohorts convert postpartum care from isolated consumer navigation into
structured social support. They may include birth-month parent groups, mother support
groups, father or non-birthing parent groups, lactation groups, newborn-care groups,
postpartum mental-health support groups, language-specific cohorts,
disability-accessible cohorts, rural tele-cohorts, and high-risk postpartum
follow-up cohorts. Participation is voluntary. The app allows families to opt into
local, virtual, or hybrid cohorts. Cohort information is privacy-protected and may
not be disclosed to employers. The purpose is to reduce social isolation, increase
continuity, normalize escalation, and create durable support networks during the
first year postpartum.

---

## Risk-Stratified Affordability Protection

High-risk pregnancies may require substantially more routine monitoring than standard
pathways — additional ultrasounds, more frequent prenatal visits, specialist
consultations, expanded labs, and closer postpartum follow-up. Much of this
additional monitoring is predictable and schedulable, which keeps it in the
market layer by design. But it is not optional in any meaningful clinical sense.
A high-risk mother facing elevated routine-layer exposure because her clinically
indicated monitoring exceeds standard package assumptions is bearing a cost the
system did not intend to impose.

The design intent is that risk-stratified routine services remain price-transparent
and HTA-settled, but that enhanced public credits or family-envelope allowances
activate automatically where DoDA and HETA taxonomy classifies the pathway as
medically indicated. The subsidy and envelope calibration should adjust to the
pathway, not require the patient to absorb the gap between standard assumptions
and clinical reality.

The precise mechanism for this adjustment is an open calibration question that
cannot be fully resolved before pilot data is available. Two approaches are under
consideration. The first is validated income- and clinical-need discounting through the Medicaid-derived affordability layer using zero-knowledge
proof attestation of a clinical condition — the patient's SSI health wallet
confirms that a risk-stratifying condition is present without disclosing the
underlying diagnosis to the provider or the system, and the subsidy adjusts
accordingly. This preserves privacy while allowing income-graduated support to
reflect clinical need. The second is routing certain categories of high-risk
monitoring directly through SEC as medically necessary rather than treating them
as market-layer care, even where they are technically schedulable.

Both approaches have tradeoffs. ZKP-based Medicaid discounting preserves the
market-layer architecture and price transparency, but depends on SSI attestation
infrastructure reaching sufficient maturity and on DoDA certifying which conditions
qualify. SEC routing for high-risk monitoring simplifies the patient experience but
compresses the market-layer boundary and creates classification disputes at the
margin.

DoDA should monitor high-risk pregnancy cohort exposure — the gap between expected
HTA drawdown under standard assumptions and actual drawdown under risk-stratified
pathways — from the beginning of pilot deployment. Where that gap is systematically
large, HETA is authorized to adjust enhanced credit activation thresholds without
waiting for the next legislative cycle. The resolution between ZKP discounting and
SEC routing will be informed by that data, by SSI infrastructure readiness, and
by Congressional guidance on the boundary between market-layer and SEC-covered
medically necessary monitoring.

During pilot phases, the default should be upside protection rather than patient
exposure: where classification is uncertain, temporary enhanced credits should apply
subject to later DoDA reconciliation rather than leaving high-risk patients to absorb
clinically indicated monitoring costs.

---

## Regional Health Center Integration

Regional Health Centers include maternal and family-care capacity where DoDA
identifies documented gaps. At minimum, regional integration covers preconception
counseling, prenatal routing, routine maternal-care navigation, postpartum checkups,
lactation support, newborn-care onboarding, behavioral-health screening, telehealth
maternal support, transfer coordination, postpartum cohort facilitation, and referral
to certified postpartum recovery centers where available.

In rural and frontier regions, the federal obligation may shift toward transport,
telehealth, mobile maternal-care units, and regional postpartum-support hubs where
fixed postpartum centers are not viable. Maternal-care deserts are treated as
infrastructure gaps, not merely provider-market failures.

---

## Settlement Flow

The standard maternal and family-care settlement flow is straightforward. The patient
activates a Family-Formation Planning Pathway through a participating provider or
directly through the healthcare app. The app generates local care package options,
SEC boundary explanations, HTA eligibility, employer contribution estimates, public
subsidy eligibility, and expected out-of-pocket exposure. The patient selects a
provider, package, postpartum center, or support service. The provider submits the
standardized service code and posted price through the unified payment rail. The rail
checks available HTA balance, Family Care Envelope status, employer contributions,
public subsidies, and approved credits, then calculates the patient's net
responsibility and displays the settlement breakdown. Payment settles to the provider
through UPI. Qualifying services update the patient's maternal-care pathway record
with consent-bound privacy protections. DoDA receives aggregate, de-identified data
for access, cost, outcome, and severe-event risk analysis.

The patient does not file a claim. The arithmetic is done by the rail.

---

## Privacy and Anti-Surveillance Guardrails

Maternal and family-care data is among the most sensitive in the system. This
framework must not become a reproductive surveillance system, employer monitoring
channel, or family-status discrimination tool.

Employers may not access pregnancy planning status, pregnancy status, fertility
status, provider selection, maternal diagnosis, postpartum mental-health status,
child health data, account balance, family-care utilization, subsidy eligibility,
cohort participation, or actuarial classification. Providers may not access account
balances, employer contribution status, income subsidy status, or payer mix. Public
reporting must be aggregate, de-identified, and privacy-protected. Any
reproductive-health data sharing must be purpose-bound, time-limited, revocable
where legally possible, and logged through the SSI health wallet.

---

## Fraud, Gaming, and Abuse Controls

Maternal and family-care account architecture creates predictable gaming risks
including providers inflating package prices after subsidy activation, postpartum
centers marketing luxury amenities as medically necessary care, unnecessary service
bundling, steering families into vertically integrated providers, employers
undercontributing to family-care envelopes, account overfunding for tax preference
rather than care need, platforms using pregnancy-related engagement to target or
discriminate, and hospitals using postpartum centers for premature discharge without
proper clinical stability.

Controls include standardized maternal service taxonomy, package definition rules,
posted-price requirements, regional price telemetry, provider-side blindness to
account balances, employer privacy firewall, clinical stability discharge criteria,
postpartum center certification, hospital escalation protocols, patient confirmation
of completed service, randomized audit sampling, anomaly detection on service mix and
price movement, DoDA monitoring of subsidy capture, labor-stack enforcement for
contribution evasion, and PCA access suspension for firms or providers engaged in
systematic abuse. Enforcement targets provider, employer, and platform gaming.
Patients are not forced into paperwork-heavy reimbursement systems because
institutions may abuse the rail.

---

## Access Safeguards

Family-care support must not become a two-tier system. Before full activation of
price-based choice models, DoDA certifies regional access adequacy using metrics
including OB and midwife availability, preconception and prenatal appointment wait
times, postpartum appointment completion rates, lactation and pelvic-floor PT
availability, maternal mental-health availability, postpartum recovery-center
capacity, parent cohort availability, transportation and language access, rural and
frontier access, maternal severe-event rates, postpartum readmission rates, emergency
transfer times, price dispersion for maternal packages, and provider participation
rates.

Where access is inadequate, HETA and PCA may prioritize capacity expansion through
Regional Health Centers, postpartum recovery-center buildout, mobile maternal-care
units, telehealth infrastructure, provider onboarding support, midwife and doula
certification pathways, and workforce pipeline investments. Public credits may
increase access in inadequate regions, but non-utilization may not be interpreted as
patient choice where provider supply is insufficient.

---

## DoDA Maternal-Care Telemetry

DoDA tracks maternal and family-care metrics as a defined healthcare telemetry
category. Key indicators include preconception pathway activation, prenatal and
postpartum visit completion, postpartum mental-health screening completion, lactation
and pelvic-floor therapy utilization, postpartum recovery-center and parent cohort
utilization, maternal emergency utilization, severe maternal morbidity, maternal and
newborn readmissions, NICU utilization, emergency transfer times, postpartum
complication follow-up rates, patient-reported escalation failure and price surprise,
average expected versus actual family exposure, HTA and Family Care Envelope
drawdown, employer family-care contribution compliance, provider price movement after
subsidy activation, and access by region, income, language, disability, household
structure, and employment type where legally permitted and privacy-protected.

The key measurement question is whether transparent maternal-care pathways,
family-care envelopes, postpartum centers, and parent cohorts reduce preventable
complications, financial uncertainty, postpartum isolation, missed follow-up, and
severe-event escalation. If DoDA certifies durable risk reduction, the SEC
contribution sufficiency framework may recognize that reduction through reserve
calibration, contribution step-downs, or other authorized fiscal mechanisms.

---

## Relationship to SEC

This framework preserves SEC actuarial integrity. SEC remains responsible for
emergency, acute, medically necessary, hospital and procedural, and severe maternal
or newborn events. HTA accounts and Family Care Envelopes finance predictable,
market-layer maternal and family-care services. The two layers interact actuarially
— better prenatal routing, postpartum monitoring, lactation support, pelvic-floor
therapy, mental-health support, and parent cohorts may reduce future severe-event
exposure. HTA balances do not replace SEC reserves. SEC reserves do not pay for
ordinary family support. The bridge between the layers is measured, DoDA-certified
risk reduction.

---

## Relationship to Employer Contributions

Employer family-care contributions replace the family-insurance premium function.
Under the legacy system, employers often pay more for family coverage than individual
coverage, but that support disappears into opaque premiums, networks, deductibles,
and claims administration. Under this framework, employer family-care contributions
are routed into transparent, portable account architecture while SEC covers
severe-event risk. Employers may satisfy their family-care contribution obligations
through authorized payroll deposits into worker-owned HTA accounts or certified
Family Care Envelopes. Employers may not condition contributions on provider choice,
pregnancy status disclosure, marital status beyond lawful household eligibility, or
health status. The obligation is contribution-based, not surveillance-based.

---

## Relationship to Child Accounts

After birth, a child-linked health account may be created through the child's SSI
health wallet. The child account may receive authorized public child health reserve
contributions, parental transfers within capped limits, employer family-care
contributions where authorized, public newborn-care credits, and philanthropic or
local child-health credits. Guardians control spending while the child is a minor
under fiduciary rules. Spending authority transfers at adulthood, subject to
disability or guardianship exceptions. Child accounts may be used for authorized
pediatric market-layer care including primary care, urgent care, dental, vision,
therapy, diagnostics, and other routine child-health needs. Child accounts may not
be used as unlimited tax-preferred family savings vehicles.

---

## Relationship to Labor Enforcement

Employer family-care contribution obligations are enforceable through the labor
stack. Contribution failures, underreporting of hours, dependent-contractor evasion,
payroll manipulation, or worker misclassification designed to avoid family-care
obligations trigger labor enforcement. Consequences include automatic reporting flags,
formula-based civil penalties, required make-whole deposits, enhanced audit status,
PCA access suspension, and debarment where warranted. The system fails if firms can
convert family-support obligations into labor-structure games.

---

## What This Is Not

This is not a new maternal insurance program. Not an HSA expansion. Not a
high-deductible birth model. Not a requirement that families save for emergencies.
Not a replacement for SEC. Not a luxury postpartum hotel subsidy. Not
employer-sponsored insurance under a new name. Not a provider network. Not
reproductive surveillance. Not a mechanism for employers to monitor pregnancy,
fertility, postpartum status, or child health.

It is a maternal and family-care integration framework that makes predictable care
visible, priced, routable, and supportable while keeping emergency and medically
necessary acute care inside SEC.

---

## Bottom Line

A mother should not have to discover the price of becoming a mother one bill at a
time.

Pregnancy and early family formation should be a visible care pathway. Routine
maternal and family-support services should be discoverable, priced, and supported
through HTA architecture. Emergency and medically necessary acute care should be
covered through SEC. Postpartum recovery should be built as hospital-adjacent support
infrastructure, not as a luxury product or an afterthought. Employer family
contributions should convert the familiar logic of family insurance into transparent,
portable, account-based purchasing power.

The system gives families planning power without asking them to self-insure
catastrophe. That is the design. That is the whole point.
