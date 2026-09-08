---
description: "The 200% Base APY, 12-hour epochs, term weights, renewal ladder, early-exit rule and dynamic reward boundary."
icon: "chart-line"
---

# Staking & Returns

The staking base is the 72% principal component `S`. The approved Base APY is 200%, settled every 12 hours and multiplied by the selected term weight `w`.

```text
r_epoch = (S × APY × w) / (365 × 2)
r_day   = (S × APY × w) / 365
R_term  = S × APY × w × T / 365
```

| Term `T` | Weight `w` | Liquidity condition |
|---:|---:|---|
| 30 days | 1.00 | Flexible; early exit deducts 10%–15% of principal |
| 90 days | 1.10 | Unlocks at maturity |
| 180 days | 1.20 | Unlocks at maturity |
| 360 days | 1.35 | Unlocks at maturity |
| 540 days | 1.50 | Recommended long term in the project paper |

The renewal ladder is `30 → 90 → 180 → 360 → 540 days`, producing approximately 1,200–1,400 cumulative locked days when renewed step by step. A user may instead redeem at maturity and open a new 540-day order.

For early exit from the flexible term:

```text
Refund = S × (1 − λ), where λ is 10%–15%
```

Dynamic rewards use community contribution and team performance to establish levels. Adjacent levels receive a Differential Matching Bonus in the same epoch as static rewards. The Reward Payout Ratio is 150%–200% and is adjustable by round and market conditions. Level names, thresholds and differential rates are not yet published, so an individual dynamic reward cannot be calculated from this paper.

{% hint style="danger" %}
The 200% Base APY and 150%–200% payout ratio are adjustable protocol parameters, not guaranteed realized returns. They do not account for token-price movement, liquidity, slippage, fees, taxes, custody, rule changes or loss of principal.
{% endhint %}

*Previous: [Distribution & Release](distribution.md) · Next: [Worked Examples](worked-examples.md)*
