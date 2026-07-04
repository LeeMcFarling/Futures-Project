---
id: credential-portability-and-competency-recognition
title: Credential Portability & Competency Recognition Framework
sidebar_label: Credential Portability
sidebar_position: 1
slug: /labor-and-economic-security/credential-portability
domain: Labor_and_Economic_Security
subdomain: Labor_Mobility
policy_type: Recognition Framework
status: Draft
phase: 3
version: 0.5
author: Futures Project
dependencies:
  - national-competency-framework
  - university-admissions-competency-alignment
  - workforce-immigration-skill-mobility-system
  - immigration-services-and-administration
  - ssi-self-sovereign-identity-framework
  - upi-privacy-preserving-payment-rail
  - irs-modernization-automated-income-attestation
  - idp-industrial-capacity-defense-production
  - idp-shipyard-modernization-continuity
  - idp-continuous-competitive-production
  - idp-american-outbound-mobility-scaffold
  - housing-arrival-transition-stack
related_initiatives:
  - doda-regional-wage-heatmap
  - teacher-reskilling-and-role-transformation
  - student-to-industry-retention-pathways
  - regional-wage-modernization-pilot
  - benefits-gradient-modernization
  - real-time-tax-credit-delivery
  - codetermination-worker-board-representation
tags:
  - labor
  - credentials
  - licensing
  - mobility
  - competency
  - immigration
  - education
  - ssi
  - idp
  - alliance
last_updated: 2026-04-25
---

# Credential Portability & Competency Recognition Framework

## Executive Summary

The United States has a labor mobility problem disguised as a credentialing problem. Workers who are already competent are routinely blocked from practicing across state lines, moving between institutions, or re-entering regulated occupations without duplicative relicensing, opaque equivalency review, or prolonged periods of underemployment. This affects native-born workers moving between states, workers shifting between military, apprenticeship, community-college, and university pathways, and lawful immigrants whose real skills often disappear into a bureaucratic black box rather than being translated into usable economic participation.

This framework treats credential portability as a competency-recognition problem rather than a paperwork problem. In the short run, it creates reciprocity, bridge certification, provisional practice, and equivalency mechanisms that reduce bureaucratic scarcity while preserving legitimate public-safety standards. In the long run, it shifts occupational recognition away from fragmented institutional pedigree and toward validated capability itself — carried by the worker, verifiable in near-real-time, and portable across state lines, employment transitions, and international boundaries.

The brief sits at the intersection of three stacks. It is a domestic labor mobility instrument, connecting to the wage modernization pilot, labor-market transparency architecture, benefits and tax credit delivery reforms, and codetermination. It is a technology infrastructure instrument, built on the Self-Sovereign Identity framework and the IRS modernization data layer. And it is an alliance industrial instrument, providing the workforce credentialing layer that the Integrated Defense Partnership industrial architecture requires to function at scale. These three functions run through the same technical infrastructure. The same credential a nurse carries across state lines is the same credential architecture that certifies an allied nation's manufacturing workforce for IDP production programs.

Licenses are the bridge. Competency is the destination.

## Problem Statement

The American credentialing system is fragmented across states, boards, institutions, and legacy professional pathways that often treat prior proof of competence as if it does not exist. A licensed worker moving from one state to another may be forced to repeat training, exams, waiting periods, or documentation processes even when the underlying competency requirements are substantially similar. A worker with military or apprenticeship training may find that their demonstrated skills are not recognized cleanly outside the institution that produced them. A lawful immigrant with real occupational competence may spend years in low-wage work because foreign training, supervised experience, or prior licensure cannot be translated into a recognized U.S. pathway quickly or transparently.

These failures reduce labor-market throughput, raise prices, exacerbate regional shortages, and create artificial scarcity in occupations where the country already has the human capability it needs. This is not merely inefficiency. It is a structural mismatch between a modern economy that needs labor to move and a credentialing system that still assumes competence is local, static, and institution-bound.

The failure is compounded by an information architecture problem. Verification currently depends on institutions communicating with each other — a state licensing board calling another state licensing board, a hospital requesting paper records from a medical school, an employer waiting for a foreign credentialing body to respond. Each of these verification chains is slow, gameable, and opaque. The worker has no portable, authoritative representation of their own professional identity. Their credentials live in other people's filing systems.

## Policy Objective

The objective of this framework is to make verified competence portable across jurisdictions, institutions, and lawful labor pathways while preserving legitimate public-safety standards. Success is defined by lower relicensing delay, higher interstate labor mobility, faster time-to-practice in shortage occupations, reduced immigrant deskilling, and growing use of competency-based recognition pathways over legacy administrative repetition. The goal is not to abolish professional standards. The goal is to distinguish real standards from bureaucratic duplication, and to give workers sovereign control over the proof of their own competence.

## Core Design Principle

Recognition should attach to demonstrated competence unless a clearly defined, role-specific reason requires additional training. That principle produces a two-horizon system. In the transition horizon, where states, boards, and legacy credentials still dominate, the default should be reciprocity, bridge certification, equivalency review, and provisional practice rather than full relicensing from scratch. In the destination horizon, occupational access increasingly rests on validated competency itself: modular capability records held by the worker, practical demonstration where warranted, periodic re-certification tied to actual scope-of-practice relevance, and machine-verifiable portability across jurisdictions.

## The Transitional Recognition Architecture

The transitional layer operates inside the current world of state licensing, institutional credentials, and board authority. Its function is to reduce friction without waiting for the destination horizon to arrive.

Where two jurisdictions regulate the same occupation and their core competency requirements are substantially equivalent, recognition should default to reciprocity. Reciprocity does not require perfect administrative uniformity. It requires that the worker has already demonstrated the underlying occupational capability and remains in good standing. States may retain narrow, jurisdiction-specific supplemental requirements where justified by local law, environment, or safety conditions, but those requirements must be explicit, published in advance, limited in scope, and tied to a real local difference rather than general protectionism. A state may require a short jurisprudence module or local code supplement. It may not require full retraining absent a demonstrated competency gap.

Where competencies are mostly but not fully equivalent, the worker enters a bridge pathway rather than a restart pathway. Bridge certification is appropriate when a worker has already demonstrated the occupational core but lacks one or more bounded requirements — a state-specific code module, a local procedural variation, a narrow supervised-hours category not covered in prior training. Bridge pathways must be modular rather than program-length, time-bounded, transparently priced, and available on a rolling basis rather than tied to rare cohort schedules. The system should not impose a two-year barrier to close a two-month gap.

For occupations where immediate full recognition would be inappropriate but existing competence is strong, states may issue provisional practice authority, allowing the worker to practice under defined supervision while completing bridge requirements. Provisional authority prevents deskilling during administrative transition and allows workers to earn, practice, and integrate while completing local requirements. It is especially valuable in nursing and allied health, skilled trades, teaching and educational support, and shortage occupations in regional labor markets.

Every participating jurisdiction must maintain a standardized equivalency review process with published criteria covering competency domains, training hours where relevant, supervised practice records, exam performance, recent practice history, and disciplinary status. The review must distinguish between core occupational competence, jurisdiction-specific supplementation, and documentation uncertainty. Documentation uncertainty alone should not collapse into non-recognition if alternative evidence of competence exists.

## The Competency-Native Recognition Architecture and SSI Infrastructure Layer

The long-term direction of the system is away from fragmented credential sovereignty and toward competency sovereignty — occupational recognition that rests on whether a person can actually demonstrate the required capability safely and consistently, not on whether they first acquired that capability inside the right bureaucratic container. Competency sovereignty requires more than a policy commitment. It requires an infrastructure layer that makes verified competence portable, machine-readable, and worker-controlled across jurisdictions, institutions, and lawful labor pathways. The Self-Sovereign Identity framework is that infrastructure layer.

Under the SSI framework, the credential lives with the worker rather than the issuer. Issuing institutions — state licensing boards, universities, apprenticeship programs, hospitals, employers — retain full authority to assess and certify occupational competence. What changes is where the credential lives after it is issued. A verifiable occupational credential is a cryptographically signed claim stored in the worker's own SSI wallet on their own device. The worker presents a zero-knowledge proof derived from the credential — confirming that they hold a valid, unexpired occupational competency record without disclosing raw underlying data. The receiving institution verifies the proof against the issuer's published cryptographic signature without contacting the issuer and without storing the worker's personal data.

Consider a doctor licensed in New York who moves to Wyoming. Wyoming's licensing board does not call New York. It requests a cryptographic proof from the wallet. The wallet returns a confirmation: valid NY medical license, unexpired, no disciplinary flags, MD from an accredited institution, verified employment history, relevant specialty competencies attested. Wyoming checks the proof against a published competency domain map and identifies any narrow gap. The recognition event that currently takes weeks or months collapses into a near-real-time verification. Is this person licensed as a physician in New York? Do they have the degree? Do they have the employment history? The answers are cryptographically confirmed in seconds.

The portability consequences of this architecture are direct. Portability becomes a property of the credential itself rather than a product of bilateral negotiation. A worker's professional identity is genuinely theirs — no institution holds a master copy that can be revoked, withheld, or lost when a board changes systems or fails to respond to a verification request. And because zero-knowledge proofs disclose only what is necessary, a licensing board learns that the credential is valid and covers the relevant competency domains without learning the worker's home address, date of birth, or any attribute not directly relevant to the verification purpose.

DoDA's role in this architecture is standards body, not issuer. DoDA publishes the credential schemas, the signing standards, the competency domain map, and the interoperability rules. It does not issue credentials to workers. A state nursing board that issues a verifiable credential under the DoDA schema is participating in a shared infrastructure. A registered apprenticeship program that issues a completion credential under the same schema is doing the same. The credentials look different — different issuers, different competency domains, different scope-of-practice specifications — but they are verifiable against the same schema standard, which means they are readable by the same verification infrastructure across every participating jurisdiction. The federal role is to publish the protocol, not to issue the certificates.

The worker's SSI wallet accumulates credentials across their career. A licensed electrician moving from Colorado to Washington carries a wallet containing: a Colorado electrical license credential signed by the Colorado licensing board, a journeyman completion credential signed by their apprenticeship program, an employment history credential signed by each employer, and any specialized certification credentials from relevant training programs. Washington's licensing board requests a proof, the wallet responds, and the verification infrastructure compares the competency domains against Washington's published scope-of-practice map. The gap, if any, is identified precisely and automatically rather than through an administrator's judgment call.

The SSI occupational credential layer also integrates with the broader labor market data infrastructure. The IRS Modernization and Automated Income Attestation program produces near-real-time earnings data by sector, occupation, and geography. A worker's SSI wallet may contain income attestation credentials issued by the IRS modernization system — verifiable claims that earnings fall within a defined band in a defined sector and region, without disclosing the precise figure. This income attestation credential enables real-time EITC and CTC advance delivery under the Real-Time Tax Credit Delivery reform, gradient-based benefits under the Benefits Gradient Modernization Act, and healthcare transition account accrual under the Employer Benefits Floor reform — all without the worker having to re-prove income eligibility at each program boundary. The credential a worker carries to cross a state line is part of the same wallet architecture that handles their tax credit delivery and benefits eligibility. These are not separate systems. They are one stack.

The wage transparency architecture connects to the same infrastructure. A worker in the restaurant sector in the Denver labor-market area who holds a verifiable occupational credential attesting to their sector, occupation, income band, and region carries, in that credential, the authorization artifact for participation in regional labor consultations, wage transparency processes, worker associations, codetermination-relevant labor analysis, or other authorized labor-market governance processes. The same credential infrastructure that enables interstate mobility can authenticate participation in those processes without requiring firm-by-firm certification as the sole organizing surface. That is a meaningful reduction in participation friction for workers in high-churn, low-wage labor markets.

## Alliance Industrial Certification — The IDP Dual-Use Layer

The SSI-based occupational credential infrastructure serves a second function that is architecturally distinct from the domestic labor mobility use case but runs through the same technical layer. It is the workforce credentialing mechanism for the Integrated Defense Partnership industrial architecture.

The IDP framework requires verified workforce competence at scale across multiple partner nations. The Continuous Competitive Production framework requires certified manufacturers across IDP partner states to compete for production share of designated stockpile systems. Certification requires manufacturing capacity verification and workforce qualification confirmation. The Shipyard Modernization brief requires cross-certification of workforce qualifications across allied yards — currently a manual, bilaterally negotiated process. The Critical Materials framework requires certified supply chain workers across multiple jurisdictions. In every case, the IDP architecture specifies a workforce competence verification requirement without naming the infrastructure that makes verification executable at alliance scale. The SSI occupational credential layer is that infrastructure.

An IDP-certified manufacturer in Japan whose welders hold verifiable occupational credentials issued under a DoDA-recognized partner credential framework can demonstrate workforce competence to an IDP Production Board certification process through the same cryptographic verification event that a domestic worker uses to demonstrate competence to a state licensing board. The verification is fast, auditable, and does not require bilateral negotiation of a paper-based equivalency review for each worker at each facility.

The mechanism for extending this infrastructure to partner nations is the Recognized Partner Nation Credential Framework. Partner nations seeking IDP manufacturing certification eligibility submit their occupational credentialing systems for equivalency assessment against the DoDA competency domain map. The assessment evaluates whether the partner nation's credentialing system produces verifiable claims about the same competency domains, whether its issuance standards meet SSI interoperability requirements, and whether its quality assurance and disciplinary processes are sufficient to make its credentials trustworthy inputs to IDP certification. Partner nations that meet the standard are designated Recognized Partner Nations. Their credentialing bodies are authorized to issue verifiable occupational credentials readable by DoDA's verification infrastructure. Workers and manufacturers in recognized partner nations can present their credentials to IDP certification processes through the same cryptographic verification mechanism used domestically.

This is not automatic acceptance of foreign credentials. It is a structured equivalency assessment of the credentialing system itself — conducted once, at the system level — that then makes individual credential verification fast and transparent rather than slow and opaque. A German aerospace manufacturing technician presents a credential issued under Germany's recognized credentialing framework. The IDP Production Board verifies the cryptographic proof, checks the competency domains against the IDP certification requirements, and identifies any narrow bridge requirement. The review cycle that currently takes months collapses into a structured verification event.

The recognized partner nation designation process is also an IDP governance mechanism. Partner nations that want to participate in IDP-standard production have an independent reason to bring their credentialing systems into alignment with the DoDA framework — not because the United States is imposing a standard, but because alignment is the condition for access to the pooled demand, surge capacity, and certification reciprocity that IDP membership provides. The adoption incentive structure is correct by design.

The American Outbound Mobility Scaffold introduces an IDP Mobility Credential as the specific implementation of this architecture for workers participating in international placements. An American electrician completing a trades rotation in Scotland accumulates verifiable competency records during her placement — records issued by her host employer or training institution under Scotland's recognized partner credential framework, stored in her SSI wallet alongside her existing domestic credentials. When she returns to the United States, her international experience is not professionally inert. It is a verifiable competency record that the domestic recognition architecture reads against the DoDA competency domain map and translates into explicit recognition or a defined bridge requirement. This is the mechanism that converts international occupational experience from an anecdote on a resume into a legible credential in the domestic labor market, and it is what makes the outbound mobility scaffold's career capital argument credible to working-class and early-career audiences.

There is a longer-run possibility worth naming briefly. If SSI-based occupational credentialing spreads across IDP partner nations as native domestic infrastructure rather than merely a U.S.-facing recognition standard, the framework transitions from a bilateral recognition mechanism toward an alliance-wide human capital layer with compounding implications for labor market integration and industrial coordination that exceed the sum of individual bilateral benefits. That is a horizon outcome rather than a design target, and its full implications belong in the IDP doctrine layer. What belongs here is the note that the architecture is pointed in that direction by design.

Finally, the cross-border professional relationships formed through outbound mobility placements and IDP sector rotations are not soft social benefits. They are operational assets. An American welder who spent a year in a Japanese shipyard and maintained professional relationships with Japanese counterparts is a node in the distributed industrial resilience network. That familiarity reduces coordination friction in exactly the scenarios — disruption, surge, partial node failure — where time-to-coordination is most consequential. The credential portability framework, the outbound mobility scaffold, and the IDP social layer together constitute the human infrastructure layer of alliance industrial resilience. The SSI credential architecture is what makes that human infrastructure legible, portable, and durable across career transitions and geographies.

## Domestic Skill Mobility

The system should treat credential portability as a national workforce issue, not an immigration-only issue. A welder, teacher, nurse, electrician, or technician moving from one state to another should not face labor-market exclusion because states refuse to recognize substantially equivalent competence. A worker completing an apprenticeship should not be forced into a lower-status recognition track than a university graduate if the demonstrated competency standard is met. A military veteran should not discover that years of highly structured training and supervised technical practice do not map cleanly into civilian occupational recognition.

The domestic skill translation principle is simple: when workers have already demonstrated the relevant capability through credible pathways, the burden is on the recognition system to explain what narrow gap remains — not on the worker to restart from zero. The labor market should not lose throughput because institutions refuse to speak a common recognition language.

## Wage Transparency and Credential Value

Credential portability is not only a recognition system. It is also a labor-market transparency system.

Once occupational credentials and competencies are standardized through SSI verification, workers can compare their verified skill profile against regional and national wage distributions published through the DoDA Regional Wage and Cost Heatmap. A restaurant worker in Denver should be able to see how workers with similar credentials, tenure, role responsibilities, and competency levels are paid in Denver, in comparable Colorado labor markets, and nationwide.

This allows workers to answer practical labor-market questions: whether their current wage is above or below the regional benchmark, which credentials are associated with wage progression, which bridge certifications open higher-paying roles, and where demand for their skill profile is strongest.

The purpose is not to force a national wage scale. It is to make labor-market information legible. Employers already possess far more wage and market information than individual workers. The credential-and-heatmap system narrows that asymmetry by giving workers a verified understanding of what their labor is worth across roles, sectors, and regions.

This transparency function is the mechanism the domain overview promised when it removed standing regional wage councils from the architecture. Workers don't need a formal council to identify wage gaps or advocate for better conditions — they need the information infrastructure that makes their labor market position visible and verifiable. A restaurant worker in Denver whose SSI wallet contains their occupational credential can see, through the public DoDA heatmap, exactly what comparable workers earn locally and nationally. That is the data foundation for individual negotiation, collective organizing, and wage-floor advocacy that is grounded in facts rather than competing claims — and it requires no employer-mediated records, no formal bargaining unit, and no standing council to function.

Credentialing makes competence visible. The DoDA heatmap makes compensation visible. Together they let workers navigate the labor market with information that is currently fragmented, employer-controlled, or unavailable.

## Lawful Immigrant Skill Recognition

Immigrant skill recognition belongs inside this framework, but under strict labor-standard and wage-protection conditions. The issue is not merely inclusion. It is lawful, standards-preserving deployment of real skill. A lawful immigrant with verified medical, technical, teaching, or skilled-trade competence should not be trapped indefinitely in non-corresponding low-wage work because foreign qualifications disappear into an unstructured recognition void. At the same time, skill recognition cannot become a backdoor for lowering standards or depressing compensation.

Foreign credential bridge pathways operate under four principles. First, verified competence rather than blind acceptance — foreign credentials are assessed against competency equivalence, supervised practice, and demonstrable skill, and recognition is never automatic merely because a credential exists. Second, bridge before exclusion — where the worker is near-equivalent, the default is bridge certification or provisional practice rather than categorical exclusion. Third, labor standards remain binding — all immigrant recognition pathways remain subject to prevailing wage protections, employer accountability requirements, sectoral labor standards where applicable, and anti-exploitation safeguards, because recognition is for lawful integration into shortage roles, not for creating a lower-cost parallel labor tier. Fourth, translation must be timed to actual mobility pathways — credential recognition should occur upstream or in parallel with lawful workforce entry wherever possible, so the worker knows what the recognition gap is before or upon entry, not after years of limbo.

Under the Recognized Partner Nation Credential Framework, lawful immigrants arriving through IDP-aligned workforce pathways present verifiable credentials from their home country's recognized credentialing system. The recognition event is a cryptographic verification rather than a multi-year bureaucratic review. This does not eliminate the bridge pathway for near-equivalent credentials — it makes the gap identification fast, precise, and transparent rather than slow and opaque.

## Role of States, Compacts, and the Federal Layer

This framework is not a blanket federal takeover of occupational licensing. States retain authority over genuinely local practice conditions, public-safety rules that are truly state-specific, and administration of boards and professional oversight within federal guardrails. Interstate compacts and regional recognition bodies enable reciprocity agreements, shared competency maps, common bridge modules, mutual recognition protocols, and pooled review infrastructure for occupations with high interstate mobility. The federal role is to fund and standardize the competency recognition infrastructure, define baseline anti-fragmentation rules for federally supported pathways, condition certain federal funding on recognition discipline, support model equivalency frameworks and open standards, and integrate recognition with lawful workforce and higher-education systems. The federal government should not replace all licensing. It should prevent states from using licensing fragmentation as de facto economic closure where competence is already real.

## Integration with Education and Higher Education

This framework is a bridge into the larger education architecture. The K-12 and higher-education system is already moving toward a competency-based model in which validated capability becomes the primary signal and the transcript becomes portable, longitudinal, and independently verifiable. This framework extends that logic into occupational practice. A student's demonstrated capability flows into university placement and advanced standing, modular workforce credentials, re-skilling pathways, occupational recognition, and cross-jurisdiction mobility. The country stops rebuilding a person's proof of competence every time they move between institutions. The SSI wallet is the longitudinal record that makes this continuity technically real — a credential issued by a community college at age nineteen is still in the wallet and still verifiable when the same worker applies for a state license at age thirty-four.

## Integration with Workforce Coordination and Immigration Administration

This framework plugs into the workforce-immigration architecture as the recognition layer that converts measured labor demand into actual workforce deployment. DoDA measures real labor demand and identifies where shortages are genuine rather than rhetorical. The Workforce Coordination Authority activates domestic workforce pathways first, then certifies where labor need persists and what competencies are actually required. The Immigration Services Administration administers lawful labor mobility and verifies identity, contract alignment, and credentials where required. The Credential Portability Framework determines how demonstrated competence is recognized across jurisdictions and pathways, so measured labor need can be met by real workers without unnecessary bureaucratic loss. The system can answer, in sequence: Is there real labor need? Can domestic workers meet it? If not, what competencies are required? Which workers already have those competencies? What narrow bridge, if any, is needed for lawful and safe practice? That is a much cleaner architecture than using blunt degree, state, or nationality proxies as substitutes for skill.

## Governance, Transparency, and Appeals

Recognition systems lose legitimacy when they are opaque. Every participating jurisdiction must publish recognition criteria, equivalency rules, bridge pathway requirements, average decision times, approval and denial rates, appeal procedures, and occupational shortage overlays where expedited recognition is active. Workers must be able to see whether they qualify for reciprocity, what precise gap prevents full recognition, what bridge pathway closes that gap, how long the process should take, and how to challenge a denial. An opaque board is not a quality-control mechanism. It is a labor bottleneck.

## Implementation Logic

The framework phases in across four stages. The first stage pilots a limited set of occupations with high verified shortage pressure and clear portability failure — nurses and allied health workers, electricians, plumbers, and skilled construction trades, teaching and educational support roles, advanced manufacturing technicians — and builds model reciprocity maps, bridge pathways, and provisional practice rules alongside the SSI credential issuance infrastructure. The second stage scales reciprocity and bridge modules through regional compacts and federal support, and extends the SSI credential schema to additional occupational categories and initial recognized partner nation certifications. The third stage integrates portable competency records fully with occupational recognition in sectors where the competency architecture is mature, and connects the IDP Mobility Credential to the outbound mobility scaffold's credential recognition infrastructure. The fourth stage shifts more occupations from pedigree-heavy recognition to competency-first recognition as validated capability records achieve sufficient coverage and institutional trust.

The bridge is phased. The destination is explicit.

## Strategic Framing

This framework should be framed as a pro-worker, pro-competence, anti-bureaucratic scarcity reform. It helps native-born workers move where opportunity exists, veterans translate real training into real civilian practice, students convert validated capability into actual economic mobility, lawful immigrants use real skills without being trapped below their capacity, employers access labor where shortages are genuine, and states preserve safety without weaponizing administrative fragmentation. At the alliance level, it helps IDP partner nations certify manufacturing workforces without bilateral paper review, helps international placement participants carry their experience home as legible credentials, and builds the human substrate of industrial resilience that makes distributed alliance production function under stress.

The strongest frame is not deregulatory. It is civilizational. A modern labor market cannot be regional in demand and medieval in credential portability. An alliance cannot be integrated in hardware and fragmented in human capital. The infrastructure that connects those two failures is the same infrastructure, and it is already being built.

## End State

In the near term, a worker moving between states or lawful pathways encounters reciprocity where competencies are equivalent, bridge certification where gaps are narrow, provisional practice where supervision is warranted, and a transparent explanation where further training is truly required. A partner nation manufacturer seeking IDP certification encounters a verification event rather than a bilateral negotiation. An American returning from an international placement encounters a domestic labor market that can read her international credentials.

In the long term, the country moves toward a simpler rule: occupational recognition rests on validated capability, held by the worker, verifiable in near-real-time, portable across every boundary the modern economy requires workers to cross. The result is a labor market that is more mobile, more honest, less bureaucratically extractive, and better aligned with the education, workforce, immigration, and alliance architecture of the project.

Licenses are the bridge. Competency is the destination.