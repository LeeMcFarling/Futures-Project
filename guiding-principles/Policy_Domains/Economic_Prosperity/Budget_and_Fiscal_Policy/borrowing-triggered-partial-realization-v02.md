---
id: borrowing-triggered-partial-realization
title: Borrowing-Triggered Partial Realization
sidebar_label: Borrowing-Triggered Realization
sidebar_position: 4
slug: /economic-prosperity/budget-fiscal/borrowing-triggered-partial-realization
domain: Economic_Prosperity
subdomain: Budget_and_Fiscal_Policy
policy_type: Mechanism
status: Draft
version: 0.2
author: Futures Project
dependencies:
  - tax-code-as-revenue-system
  - wealth-mobility-and-anti-aristocracy-principle
  - superannuation-and-large-fortune-framework
  - dynasty-tax-and-generational-transfer-framework
  - pca-capital-recycling-architecture
tags:
  - tax
  - unrealized-gains
  - capital-formation
  - borrowing
  - realization
  - anti-aristocracy
  - realization-parity
last_updated: 2026-04-21
---

## Purpose

The capital gains system taxes wealth when it is realized — when an asset
is sold and a gain is recognized. That design was built for an economy in
which accessing wealth required selling assets. It was not built for an
economy in which the wealthiest individuals can access the full economic
benefit of appreciated assets — indefinitely, at scale — without ever
selling them.

The mechanism that makes this possible is well understood. An individual
holds $1 billion in appreciated stock, most of it unrealized gain. Rather
than sell — which would trigger immediate tax — they borrow against the
position at low interest rates. The loan provides cash. The asset continues
to compound. The interest payments are trivial relative to the deferred
liability and the ongoing appreciation. At death, the basis steps up and
the heirs inherit the position free of the embedded gain. The accumulated
tax liability disappears entirely.

This is not a loophole in the narrow sense. It is a structural consequence
of a realization system that treats borrowing and selling as categorically
different events, even when they produce economically equivalent outcomes
for the borrower. This framework recognizes that monetization — accessing
the economic value of appreciated assets through borrowing or equivalent
instruments — is economically equivalent to realization at sufficient scale,
and treats it accordingly.

This brief is the primary mechanism document for Doc 4 of the fiscal
architecture: how you stop people from accessing huge appreciated fortunes
without ever realizing gains. It establishes what the instrument does, how
it works, what it explicitly does not do, and how it interacts with the
broader anti-aristocracy framework of which it is one part. The enforcement
architecture that makes it operational is established in the companion
implementation brief.

---

## The Structural Problem

The conventional description of buy-borrow-die focuses on the interest rate
arithmetic — borrowing at 3% is cheaper than paying capital gains at 23.8%.
That framing is accurate but incomplete. The deeper problem is not that
borrowing is cheap. It is that borrowing against appreciated assets is
currently costless in tax terms, regardless of scale or intent.

Consider the math directly. An individual holds $1 billion in appreciated
stock. Assume $900 million of that is unrealized gain. The capital gains
rate is 23.8%. A sale would generate $214 million in immediate tax
liability. A $50 million loan at 3% costs $1.5 million per year in
interest. The full $1 billion continues to compound. No realization occurs.
No tax is due.

At that interest rate, the borrower can sustain $50 million in annual
liquidity for approximately 143 years before the cumulative interest
payments reach what a single sale would have cost in taxes — and the
underlying asset will have compounded far beyond its current value long
before then. The strategy is not merely advantageous. It is categorically
dominant over selling, for anyone with a large enough position and a long
enough horizon.

The consequence is not simply deferred revenue. It is structural lock-in
of unrealized appreciation at the top of the wealth distribution, combined
with permanent insulation of that appreciation from the tax system that
applies to everyone who cannot access it. Capital that would otherwise
circulate — through reinvestment, diversification, and the ordinary process
of economic churn — stays locked in concentrated positions because the tax
system creates a powerful incentive to hold indefinitely and borrow
indefinitely rather than sell.

This lock-in has a second-order distortion that is less discussed but
equally real. Founders and major shareholders who cannot sell without
triggering realization have a structural incentive to support share buybacks
and other price-stabilization mechanisms because their borrowing capacity
and cost depends on a sustained stock price. The personal liquidity strategy
and the firm's capital allocation decisions become entangled in a way that
serves the shareholder's balance sheet rather than the firm's long-term
productive interests. Removing the structural advantage of indefinite
borrowing removes that entanglement, allowing capital allocation decisions
to be made on economic rather than tax-optimization grounds.

---

## The Mechanism

Borrowing-triggered partial realization treats any transaction that
monetizes appreciated assets above the threshold as a partial recognition
event proportional to the share of total asset value accessed.

The operative rule is as follows. When an individual or a covered entity
borrows against or otherwise monetizes appreciated assets, and the total
value of assets covered by this framework exceeds $50 million, a fraction
of the embedded unrealized gain is deemed realized equal to the fraction
of total covered asset value that the borrowed or accessed amount
represents.

The arithmetic is straightforward. An individual with $1 billion in covered
assets borrows $50 million. That loan represents 5% of total covered asset
value. Five percent of the embedded unrealized gain — in this case, 5% of
$900 million, or $45 million — is deemed realized in the year of the
borrowing. Capital gains tax applies to that deemed realization at the
applicable rate. On $45 million at 23.8%, the tax owed is approximately
$10.7 million.

The total cost of the $50 million borrowing — tax plus interest — is
approximately $12.2 million in the first year alone. That is a 24% effective
cost on the borrowed amount before accounting for ongoing interest drag and
any future realization events on unreleased gain. At that cost, selling a
comparable position is genuinely competitive: a direct sale of $50 million
in stock generates approximately $11.9 million in capital gains tax, clears
the debt from the balance sheet, eliminates ongoing interest payments, and
removes the unrealized gain on that portion from the future tax base
entirely.

The structural advantage of buy-borrow-die does not survive this calculus.
Borrowing can continue — it is not prohibited — but it is no longer a
dominant strategy. Individuals will make decisions based on liquidity needs,
concentration risk, and genuine economic judgment rather than optimizing
purely around tax deferral. That is the intended effect.

**Irreversibility.** Deemed realization triggered under this provision is
final. It is not reversed by subsequent repayment, refinancing, or unwinding
of the underlying transaction. Without this rule, the mechanism's most
obvious attack surface is a structured loop: borrow to trigger realization,
repay to reset the basis clock, borrow again. The irreversibility clause
closes that loop entirely. A borrowing event triggers realization; what
happens to the loan afterward is irrelevant to the tax consequence already
recognized.

**De minimis threshold and aggregation.** A borrowing event below $1 million
or below 1% of total covered asset value — whichever is greater — does not
trigger realization. This prevents administrative churn from incidental
transactions and small liquidity draws. To prevent fragmentation as an
avoidance strategy, all covered borrowing and monetization events within a
rolling 12-month window are aggregated for purposes of applying the trigger
and calculating proportional realization. Borrowings structured as sequential
small tranches to stay below the de minimis floor are treated as a single
event for this purpose.

**Unified portfolio treatment.** Covered assets are treated as a unified
portfolio for purposes of determining proportional realization and basis
adjustment. The proportionality calculation uses total covered asset value
and total embedded unrealized gain across the portfolio — not the value or
basis of any specific asset pledged or referenced in a particular
transaction. Without this rule, individuals would selectively pledge
high-basis assets to minimize the realized gain per dollar borrowed,
defeating the proportional logic of the mechanism. Portfolio-level treatment
eliminates that optimization entirely.

---

## Scope: What Triggers Realization

The trigger is defined by economic substance, not legal form. Any
transaction that results in cash or cash-equivalent proceeds derived from
or collateralized by appreciated assets above the $50 million threshold
triggers proportional realization on the accessed portion of embedded
gain, regardless of how the transaction is structured.

This scope is intentionally broad because the narrow alternative —
limiting the trigger to conventional secured loans — is systematically
gameable. The population of individuals to whom this provision applies
has consistent access to sophisticated financial engineering, and any
enumerated list of covered instruments will generate pressure to develop
instruments that achieve identical economic outcomes through uncovered
structures.

The instruments that would otherwise circumvent a loans-only trigger
include total return swaps, in which a counterparty pays cash flows
economically equivalent to a sale without a transfer of ownership;
prepaid variable forwards, in which future appreciation is exchanged
for present cash without a current recognition event; and monetization
collars, in which a position is economically locked at a known value
through a combination of puts and calls while leaving the borrowing
technically uncollateralized. Each of these is a functional equivalent
of borrowing against an appreciated position. Each would escape a
narrow loans-only trigger and preserve the structural advantage this
provision is designed to eliminate.

To ensure that future instrument design does not outpace statutory
enumeration, the provision includes a synthetic exposure clause: any
transaction with a primary purpose or material effect of replicating
the economic outcome of collateralized borrowing against appreciated
assets shall be treated as a covered monetization event, regardless
of its formal structure. This gives regulators authority to move
against novel instruments without waiting for statutory updates, and
places the burden of demonstrating non-equivalence on the transacting
party rather than on the government to identify each new structure as
it appears.

The substance test asks a single question: has the individual accessed
the economic value of appreciated assets above the threshold without
a recognition event? If yes, proportional realization applies.

---

## Scope: The Operating Company Exemption

Genuine operating companies are exempt from the borrowing trigger. A
business borrowing against its assets for operational purposes —
capital expenditure, working capital, acquisition of productive
capacity — is not monetizing personal accumulated appreciation. It is
doing what businesses do. Treating that activity as a realization event
would distort business financing and create perverse incentives against
legitimate capital deployment.

The exemption attaches to the asset's function rather than the entity's
legal form. The relevant question is not whether a borrowing occurs
through a corporate entity but whether the specific assets against
which borrowing occurs are actively and demonstrably employed in a
genuine trade or business. Legal form is irrelevant. Economic function
is determinative.

An operating company that manufactures goods, employs workers, and
borrows against productive assets to finance expansion is clearly
exempt. A family office that holds appreciated securities inside an LLC
and has that LLC borrow against the portfolio is not exempt — the
LLC's legal existence does not transform the underlying transaction
into business financing. A holding entity whose primary purpose is
wealth management is treated as the household it functionally is,
regardless of its corporate structure.

The more difficult cases involve entities that are genuinely operational
but also hold significant appreciated assets that serve no operating
function. A large private company that operates actively in its core
business but also holds a substantial real estate or securities
portfolio on its balance sheet presents a mixed picture. The resolution
is asset-level rather than entity-level: operating assets remain
exempt, non-operating appreciated holdings do not, and borrowing is
allocated proportionally between the two pools based on the balance
sheet composition at the time of the transaction. This approach is
administrable through standard accounting distinctions between
operating and non-operating assets, which already exist in financial
reporting.

The test for exemption has three elements. The asset must be held by
an entity with active business operations, meaning revenue from the
sale of goods or services rather than investment returns or
appreciation. The asset must be used in the conduct of those
operations rather than merely owned by the entity as a financial
holding. And the entity must be subject to genuine business risk —
employees, liabilities, and operational exposure beyond the asset
itself. Stock in a publicly traded company held inside a family
partnership fails all three. A founder's equity in an actively
operating private company they lead and manage passes all three.

One guardrail applies regardless of entity structure: assets primarily
held for investment, liquidity management, or passive appreciation do
not qualify as operating assets. A genuine operating company that also
maintains a substantial securities portfolio, cash reserve in excess
of operational needs, or real estate held for appreciation rather than
use does not thereby exempt those holdings from the trigger. The
exemption follows the asset's function. Assets doing economic work in
a business are exempt. Assets sitting on a balance sheet compounding
are not, even if they sit inside an entity that is otherwise
legitimate.

---

## What This Mechanism Does Not Do

It does not prohibit borrowing against appreciated assets. The
transaction remains available. The structural tax advantage of using
it in lieu of realization does not.

It does not require forced liquidation. Tax liability triggered by
borrowing is payable in cash — from the proceeds of the loan, from
other liquid resources, or through a deferred payment arrangement where
liquidity is genuinely constrained. No asset sale is compelled by the
mechanism itself.

It does not apply to assets below the $50 million total threshold.
Below that level, ordinary wealth-building incentives remain intact.
The mechanism is calibrated to extreme accumulated scale — the
population for whom buy-borrow-die is a planning strategy, not an
academic concept — and does not reach ordinary high-net-worth
individuals, family businesses, or professional earnings accumulated
over a career.

It does not apply to ordinary business financing. The operating company
exemption reflects the genuine structural distinction between business
borrowing and personal monetization of accumulated appreciation, and
it is drawn broadly enough to protect legitimate commercial activity
while closing the personal planning strategy the provision is designed
to address.

It does not create ongoing state management of private assets or
investment decisions. The obligation arises at the moment of
monetization and is settled at that moment. The state is not involved
in how assets are held, managed, or deployed in the intervals between
transactions.

---

## The Offshore Routing Problem

A substance-based trigger applied only to domestic lenders would push
borrowing to foreign institutions. The fix is to make the trigger
follow the asset, not the lender. Any borrowing against covered assets
— whether those assets are U.S.-sited or held by U.S. persons, and
regardless of where the loan originates or where the lender is
domiciled — triggers proportional realization. A U.S. person who
pledges appreciated U.S. securities to a Swiss bank as collateral for
a cash loan has monetized those securities in the relevant sense.

Enforcement against offshore structures relies on existing disclosure
requirements for foreign financial accounts and the reporting
obligations applicable to U.S. persons with foreign financial
interests, supplemented where necessary by enhanced reporting
requirements for transactions involving covered assets above the
threshold. The full offshore enforcement architecture — including
FATCA coordination and the covered asset exit notification requirement
— is established in the implementation brief.

---

## Interaction with the Anti-Aristocracy Framework

This mechanism is one of two complementary instruments that together
close the primary structural paths through which extreme accumulated
appreciation has remained permanently outside the tax system. It
operates alongside the dynasty tax and generational transfer framework,
which closes the generational transfer path by treating death — or
the 100-year holding mark for structures designed to avoid a death
event — as a realization event rather than a basis-reset opportunity.

This instrument addresses active monetization — accessing appreciated
value through debt or equivalent structures rather than sale. The
dynasty tax framework addresses the generational transfer —
eliminating the step-up mechanism that currently resets the embedded
gain at death and closing the holding-forever path by making the
generational transfer a recognition event rather than a permanent
escape.

The two instruments are internally consistent and do not create
double taxation on the same gain. The borrowing trigger adjusts
cost basis upward for each proportional realization event during
the holder's lifetime. At death, the dynasty tax framework applies
to the remaining embedded gain — the gain that was never recognized
during the holder's lifetime. Every dollar of gain is recognized
exactly once, either during the holder's lifetime when it is accessed
or at the generational transfer when it is transferred.

Together, the two instruments make permanent, frictionless insulation
of extreme wealth from the public system that enabled it structurally
unavailable. There is no exit through borrowing. There is no exit
through transfer. The $50 million threshold is consistent across both
instruments and is not a cap on wealth accumulation. It is the point
at which the system introduces structured obligations designed to keep
extreme accumulated appreciation connected to the public and economic
environment that made it possible.

---

## Why This Is Not a Wealth Tax

A wealth tax imposes an annual obligation on the value of assets held,
regardless of whether those assets have been monetized, appreciated,
or accessed in any form. It applies to static holdings and requires
either liquidation or other arrangements to generate cash to pay a
liability that arises from ownership alone.

This mechanism does not apply to static holdings. It applies to
transactions — specific, voluntary decisions to access the economic
value of appreciated assets above the threshold. The obligation arises
when the individual monetizes, not merely when they hold. An
individual who holds $5 billion in appreciated stock and neither sells
nor borrows against it incurs no obligation under this mechanism.

The distinction is not merely semantic. It reflects a genuine
difference in what the mechanism is designed to do. The goal is not
to tax wealth for existing. It is to prevent the indefinite,
frictionless extraction of value from appreciated assets without any
interaction with the tax system that applies to ordinary income and
capital gains. Monetization is the event that makes that extraction
concrete. The trigger follows the event.

The code taxes income, profit, transfers, and monetization events.
It does not tax passive ownership merely for existing. This mechanism
is consistent with that principle in a way that a wealth tax is not.
