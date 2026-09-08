---
description: "The authoritative NEXON economic model: two operational layers, two token roles, the 72/28 capital path, staking, vesting, redemption and risk boundaries."
icon: "coins"
---

# Token Economics

> One account, two operational layers, and one auditable economic flow.

This Part implements the economic model approved by the project party on 6 September 2026. Where an older NEXON document differs, this Part supersedes it.

NEX Main Exchange/CEX is the compliant spot layer. It supports EXON spot trading, IEO activity and release display. The Staking Platform is a separate staking-and-rewards layer for single-token staking, term weighting, dynamic rewards and reward redemption. The layers share an account system and capital backend; staking parameters do not become exchange spot rules.

Every principal amount `P` follows the same path:

```text
B = 0.28 × P  → buy EXON at the prevailing price → Treasury Liquidity
S = 0.72 × P  → staking principal and reward base
B + S = P
```

{% hint style="danger" %}
The figures in this Part are protocol parameters and conditional illustrations, not promises of yield, price, payback period or principal protection. APY, token prices, reward rates, execution parameters and outcomes may change or fluctuate. Participants may lose some or all principal.
{% endhint %}

## In this Part

- [Two Assets, Two Jobs](two-assets-two-jobs.md) defines XO and EXON without role overlap.
- [XO](xo.md) explains the staking-principal asset.
- [EXON](exon.md) explains the core value and spot asset.
- [Distribution & Release](distribution.md) records prices, early tiers and 1,095-day release.
- [Staking & Returns](staking-and-returns.md) contains the APY, term and reward formulas.
- [Worked Examples](worked-examples.md) reproduces the project paper's complete conditional math.
- [Value Flows](value-flows.md) joins buy, lock, redemption and burn into the value loop.

The numerical EXON total supply, complete allocation, initial float, future-round limits and complete dynamic reward table remain unpublished. They must not be inferred.

*Next: [Two Assets, Two Jobs](two-assets-two-jobs.md)*
