---
description: "The 200% Base APY, 12-hour epochs, term weights, the renewal ladder, the early-exit rule and the dynamic-reward boundary."
icon: chart-line
---

# Staking & Returns

The interest base is `S`, the 72% principal component of the order. The Base APY parameter is **200%**, settled every 12 hours and multiplied by the selected term weight `w`.

```text
r_epoch = (S × APY × w) ÷ (365 × 2)     per epoch
r_day   = (S × APY × w) ÷ 365           per day
R_term  = S × APY × w × T ÷ 365         over the full term
```

All three are the same formula — **base × APY × weight** — sliced by time.

## Five terms

<figure><img src="../.gitbook/assets/chart-term-weights.svg" alt="Effective APY by term: 30 days 200%, 90 days 220%, 180 days 240%, 360 days 270%, 540 days 300%"><figcaption>Weights lift the 200% Base APY into a 200%–300% band</figcaption></figure>

| Term `T` | Weight `w` | Effective APY parameter | Liquidity condition |
|---:|---:|---:|---|
| 30 days | 1.00 | 200% | Flexible; early exit deducts 10%–15% of the principal base |
| 90 days | 1.10 | 220% | Unlocks at maturity |
| 180 days | 1.20 | 240% | Unlocks at maturity |
| 360 days | 1.35 | 270% | Unlocks at maturity |
| 540 days | 1.50 | 300% | The long term recommended in the approved paper |

## The renewal ladder

The renewal path is `30 → 90 → 180 → 360 → 540 days`. Renewed step by step, it accumulates roughly **1,200–1,400 locked days**.

A user can also take the other path: redeem at maturity and open a fresh 540-day order. **Both paths end at the same weight; the liquidity along the way is completely different.**

## Early exit

Only the 30-day term supports early exit:

```text
Refund = S × (1 − λ), where λ is 10%–15%
```

The exact value of λ inside that band has not been published. With `S = 21,600 USDT`, an early exit returns **18,360–19,440 USDT**.

## Dynamic rewards

The dynamic component establishes levels from **community contribution and team performance**, and applies a **Differential Matching Bonus** between adjacent levels, settled in the **same epoch** as static rewards.

**The Reward Payout Ratio band is 150%–200%**, adjustable by issuance round and market conditions.

Level names, qualification thresholds, per-level differential rates and team-performance boundaries have not been published, so **an individual dynamic reward cannot be calculated from this paper** ([Open Parameters](../open-parameters/README.md), OP-T04).

{% hint style="info" %}
**Both 200% and the 150%–200% band are adjustable protocol parameters, and both may change by issuance round and market conditions.** Every order and every epoch records the parameter version in force at the time, so a later change does not rewrite a historical accrual. An interface should be able to tell a user which version applied when their order executed.
{% endhint %}

*Previous: [Distribution & Release](distribution.md) · Next: [Worked Examples](worked-examples.md)*
