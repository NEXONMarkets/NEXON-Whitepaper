---
description: "The Wallet is the user's financial home inside the ecosystem — assets, permissions, staking access, decision support and eligible third-party experiences."
icon: wallet
---

# Wallet — Financial Home and Control

*Product stage · Roadmap*

The NEXON Wallet is designed as the user's **financial home**: the place to understand assets, positions, permissions, policies and pending actions before any route reaches execution. It is not a list of balances, and it does not manufacture a second source of yield.

## Unified state, without pretending the assets are unified

A unified view has to say where value **actually is**. XO staking principal, pending rewards, redeemable amounts and external assets each have their own executor, liquidity and risk. EXON spot balances and vesting releases are exchange-side records.

The wallet names the responsible venue, network, contract or custodian — rather than presenting every row as equivalent cash.

For the current Staking Platform mechanism, the wallet should show:

| Display | Note |
|---|---|
| Qualifying principal `P` | What went into this order |
| 28% EXON build | Bought and moved into Treasury Liquidity |
| 72% XO staking / PV base | The interest base |
| Matching EXON fuel check | Marked clearly as **still in the user's account** |
| Selected term and weight | 30 / 90 / 180 / 360 / 540 days, 1.00 – 1.50 |
| 12-hour epoch accruals and parameter version | Each accrual records the rule version in force |
| Early-exit condition | Applies to the 30-day term only |
| Pending reward and redemption choice | T+0 / 30D / 60D |
| Equivalent EXON burn and net release | Shown when a burn-bearing lane is selected |

**A display is not an executable quote.** Prices and withdrawal conditions have to be refreshed from the responsible system.

## Permission center

The wallet makes agent authority legible at a glance. A user can inspect which application may read account state, which asset it may act on, the maximum amount, destination restrictions, expiry, and how much unused authority remains.

Revocation stops **future use**. It does not reverse a completed transfer or market order. Those are two separate sentences in the interface.

Holding tokens does not widen any of this. XO's role as Value Anchor and EXON's as Circulation Engine are narrative positions, distinct from account authorization.

## Decision support

The wallet is where a user crosses from discovery to decision. It can organize watchlists, risk alerts, scenario comparisons, reserve policies and route history. AI can summarize and explain — and must flag uncertainty, sources, and **the difference between an observed balance, an estimated value and an executable quote**.

The ecosystem may also expose decentralized prediction-market experiences through third-party protocols. Those markets express a view about the future; they cannot guarantee it. NEXON provides infrastructure and an entry point, and is not the operator, counterparty or resolution authority for any of them.

Before such an entry point opens, the product terms have to state:

* the independent protocol and its custody model;
* eligibility and prohibited jurisdictions;
* market creator and resolution source;
* fees, liquidity and settlement asset;
* dispute and invalid-market rules;
* oracle and manipulation risk;
* that a prediction price is neither advice nor certainty.

Participation requires its own user approval. **Social popularity and an AI forecast do not open a position.**

## Staking access, not new economics

The wallet can provide an interface to the existing Staking Platform. That interface reproduces the confirmed mechanism at its current parameter version: it cannot change 72/28, invent dynamic-reward levels, or imply principal protection. Any calculated return states the price assumption it rests on.

## Its place in the loop

The Social App supplies context the user chose. The Wallet holds financial state and policy. PayFi builds the approved route. After execution, receipts return to the wallet so the user can reconcile what actually changed. Marketplace or card delivery stays visible as **a separate fulfillment state**.

That makes the wallet a control surface between discovery and action — not an autonomous trader.

## What has to ship before launch

A documented custody model, key recovery and incident procedures, permission and revocation specifications, supported networks and assets, independent security review, privacy and retention terms, third-party integration disclosures and jurisdictional controls.

*Previous: [AI-Native PayFi](payfi.md) · Next: [Marketplace](marketplace.md)*
