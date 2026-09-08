---
description: "The approved NEXON economy — dual-asset narrative roles mapped, without alteration, onto the 72/28 order, release, reward and redemption mechanism."
icon: coins
---

# Token Economics

> NEXON is the ecosystem. XO carries value. EXON drives circulation.

This Part implements the economic model the project approved on 6 September 2026, and maps the narrative positions — XO as **Value Anchor**, EXON as **Circulation Engine** — onto that model **without changing a single piece of its arithmetic**.

## Read each asset on three levels

| Level | XO | EXON |
|---|---|---|
| **Narrative** | Value Anchor: participation, staking, rights and long-term value accumulation | Circulation Engine: connecting digital finance, exchange, payments, fees and consumption |
| **Current mechanism** | U-priced Staking Principal Token, used inside the Staking Platform | Core Value Token; the public spot / release / buy / check / burn asset |
| **Long-term direction** | Broader ecosystem rights and governance, pending published rules | Payment, exchange, fee and consumption utility, pending published product terms |

The narrative says what each asset is **meant** to contribute. The mechanism says what it **does now**. Say both, in that order.

## One account, two operating layers

**NEX Main Exchange / CEX** is the spot layer for EXON trading, IEO activity and release display. The separate **Staking Platform** handles single-token staking, term weighting, dynamic rewards and redemption. They may share an account system and a capital backend; staking parameters do not become exchange spot rules, and the exchange does not distribute the staking rewards described here.

Every qualifying principal `P` follows the same 72/28 path:

```text
B = 0.28 × P   → buy EXON at the prevailing price → Treasury Liquidity
S = 0.72 × P   → XO staking principal and reward / PV base
B + S = P
F = 0.28 × P   → matching EXON balance check; stays with the user
```

{% hint style="info" %}
`B` and `F` have **the same U value and completely different ownership and function**. `B` is EXON bought into Treasury Liquidity. `F` is a balance checked in the user's own account — not transferred, charged or burned when the order opens. Conflating the two is the single most common misreading of this mechanism.
{% endhint %}

## The economic lifecycle

Early-round EXON enters the common **1,095-day linear release** from TGE, across 2,190 twelve-hour epochs. XO staking rewards use a **200% Base APY** parameter, a term weight from **1.00 to 1.50**, and two epochs per day. Early exit from the 30-day term deducts 10%–15% from the 72% staking base.

Reward redemption offers T+0, 30D and 60D lanes, releasing 70%, 85% and 100% and permanently burning an equivalent 30%, 15% or 0% of EXON. Dynamic rewards use an adjacent-level Differential Matching Bonus with a Reward Payout Ratio band of 150%–200%.

The Base APY and the payout band are adjustable protocol parameters and may change by issuance round and market conditions. Every figure derived from them is conditional on the parameter version and the price assumption in force at the time.

## What has not been published

The numerical EXON total supply, complete allocation, initial circulating amount, later-round quotas and discounts, final dates and the complete dynamic-reward level table are not given in the approved source. Those fields stay [Open](../open-parameters/README.md), and no other document fills them in.

## In this Part

<table data-view="cards"><thead><tr><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><strong>Two Assets, Two Jobs</strong></td><td>Why value accumulation and active circulation cannot be the same job.</td><td><a href="two-assets-two-jobs.md">two-assets-two-jobs.md</a></td></tr><tr><td><strong>Distribution &#x26; Release</strong></td><td>Early tiers, the TGE guide price, and the 1,095-day linear release.</td><td><a href="distribution.md">distribution.md</a></td></tr><tr><td><strong>Staking &#x26; Returns</strong></td><td>The 200% Base APY, term weights, the renewal ladder and early exit.</td><td><a href="staking-and-returns.md">staking-and-returns.md</a></td></tr><tr><td><strong>Worked Examples</strong></td><td>Three examples, each number shown next to the assumption it rests on.</td><td><a href="worked-examples.md">worked-examples.md</a></td></tr><tr><td><strong>Value Flows</strong></td><td>Six flows, booked separately, never collapsed into one story.</td><td><a href="value-flows.md">value-flows.md</a></td></tr><tr><td><strong>XO and EXON</strong></td><td>Each asset's name, role and current mechanism.</td><td><a href="xo.md">xo.md</a></td></tr></tbody></table>

*Next: [Two Assets, Two Jobs](two-assets-two-jobs.md)*
