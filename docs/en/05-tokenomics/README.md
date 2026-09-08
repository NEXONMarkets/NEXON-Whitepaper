---
description: "The project-approved NEXON economy: narrative asset roles mapped without alteration to the 72/28 order, release, reward and redemption mechanism."
icon: "coins"
---

# Token Economics

> NEXON is the ecosystem. XO carries value. EXON drives circulation.

This Part implements the economic model approved by the project party on 6 September 2026. It also maps the later approved narrative—XO as **Value Anchor**, EXON as **Circulation Engine**—to that model without changing its arithmetic. Where an older NEXON document differs on mechanics, the approved Tokenomics paper and the authority registry supersede it.

## Read every asset on three levels

| Level | XO | EXON |
|---|---|---|
| Narrative | Value Anchor: participation, staking, rights and long-term value accumulation | Circulation Engine: connection among digital finance, exchange, payments, fees and consumption |
| Current approved mechanism | U-priced Staking Principal Token used inside the Staking Platform | Core Value Token and public spot/release/buy/check/burn asset |
| Roadmap | Broader ecosystem rights and governance require published rules | Payment, exchange, fee and consumption utilities require published product terms |

The narrative explains what each asset is intended to contribute to the ecosystem. The mechanism defines what it does now. A Roadmap role cannot be represented as current utility merely because it fits the narrative.

## One account, two operating layers

NEX Main Exchange/CEX is the spot layer for EXON trading, IEO activity and release display. The separate Staking Platform handles single-token staking, term weighting, dynamic rewards and redemption. They may share an account system and capital backend; staking parameters do not become exchange spot rules, and the exchange does not distribute the staking rewards described here.

Every qualifying principal amount `P` follows the approved 72/28 path:

```text
B = 0.28 × P  → buy EXON at the prevailing price → Treasury Liquidity
S = 0.72 × P  → XO staking principal and reward/PV base
B + S = P
F = 0.28 × P  → matching EXON balance check; remains with the user
```

`B` and `F` have the same U-value but different ownership and function. `B` purchases EXON into Treasury Liquidity. `F` is checked in the user's account and is not transferred, charged or burned when the order opens.

## Economic lifecycle

Early-round EXON enters the same 1,095-day linear release beginning at TGE. Releases occur over 2,190 twelve-hour epochs. XO staking rewards use a 200% Base APY parameter, a term weight from 1.00 to 1.50 and two epochs per day. Early exit from the 30-day term deducts 10%–15% of the 72% staking base.

Reward redemption offers T+0, 30D and 60D lanes. They release 70%, 85% and 100% respectively and permanently burn an equivalent 30%, 15% or 0% amount of EXON. The dynamic reward system uses adjacent-level Differential Matching Bonus logic and a 150–200% adjustable payout range; the complete levels and rates remain unpublished.

## What is not supplied

The numerical EXON total supply, complete allocation, initial circulating amount, later-round quotas, final dates and complete dynamic-reward table are not published in the approved source. No estimate in another document can fill those fields. Governance thresholds, PayFi fees, supported payment assets, card economics and marketplace terms also require separate future decisions.

{% hint style="danger" %}
Every figure in this Part is a protocol parameter or conditional illustration, not a promise of yield, price, payback or principal protection. EXON price, liquidity, execution, fees, taxes, custody, technical failure, rule changes and legal restrictions can materially change outcomes. Participants may lose some or all principal.
{% endhint %}

## In this Part

- [Two Assets, Two Jobs](two-assets-two-jobs.md) separates narrative, current mechanism and Roadmap.
- [XO](xo.md) explains the Value Anchor and current staking-principal role.
- [EXON](exon.md) explains the Circulation Engine and current market/burn role.
- [Distribution & Release](distribution.md) records prices, early tiers and linear release.
- [Staking & Returns](staking-and-returns.md) states the APY, term and reward formulas.
- [Worked Examples](worked-examples.md) reproduces the project's conditional calculations.
- [Value Flows](value-flows.md) traces capital, asset and receipt movement without implying a price floor.

*Next: [Two Assets, Two Jobs](two-assets-two-jobs.md)*
