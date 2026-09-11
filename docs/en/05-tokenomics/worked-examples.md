---
description: "Three complete worked examples from the approved model — release value, term rewards and redemption outcomes — each number next to its assumption."
icon: calculator
---

# Worked Examples

These three examples come from the approved economic model. Every result carries its price assumption inside the sentence.

## Example A — the release value of early-round EXON

An input of `30,000 USDT` at the early price of `0.1 USDT` acquires `300,000 EXON`.

```text
D = 300,000 ÷ 1,095 = 273.97 EXON/day
R_epoch = 273.97 ÷ 2 = 136.99 EXON/epoch
ROI_month = (D × P_market × 30) ÷ P_in × 100%
```

The release rate is fixed: **273.97 tokens a day, 136.99 every 12 hours.** That part rests on no assumption at all.

What it is worth does:

| Assumed market price | Monthly released value | Monthly ROI calculation |
|---:|---:|---:|
| 1.0 USDT | 8,219.18 USDT | 27.40% |
| 2.0 USDT | 16,438.36 USDT | 54.79% |

Under the `2.0 USDT` assumption, the static payback arithmetic is `30,000 ÷ 16,438.36 ≈ 1.83 months`.

{% hint style="info" %}
**Both rows read the same release curve, multiplied by two different assumed prices.** The calculation itself excludes liquidity, slippage, fees, taxes and execution constraints, and it forecasts no price.
{% endhint %}

## Example B — a 30,000 USDT staking order

For `P = 30,000 USDT`: the build is `B = 8,400 USDT` and the staking base is `S = 21,600 USDT`. At a build price of `0.1 USDT`, `B` buys `84,000 EXON`.

<figure><img src="../.gitbook/assets/chart-term-rewards.svg" alt="Term totals for a 21,600 USDT staking base: 3,550.68 USDT at 30 days, 11,717.26 USDT at 90, 25,564.93 USDT at 180, 57,521.10 USDT at 360, 95,868.49 USDT at 540"><figcaption>One 21,600 USDT base; across the five terms, the term-total parameter spans a factor of 27</figcaption></figure>

| Term | Weight | Per day | Per epoch | Term total |
|---:|---:|---:|---:|---:|
| 30 days | 1.00 | 118.36 USDT | 59.18 USDT | 3,550.68 USDT |
| 90 days | 1.10 | 130.19 USDT | 65.10 USDT | 11,717.26 USDT |
| 180 days | 1.20 | 142.03 USDT | 71.01 USDT | 25,564.93 USDT |
| 360 days | 1.35 | 159.78 USDT | 79.89 USDT | 57,521.10 USDT |
| 540 days | 1.50 | 177.53 USDT | 88.77 USDT | 95,868.49 USDT |

**Look at the per-day column**: from 118.36 to 177.53, a factor of 1.5 — exactly the spread of the weights. The 27× spread in the term totals comes mostly from time, not from weight.

The 540-day weight corresponds to a **300% effective APY parameter**. An early exit from the 30-day term returns **18,360–19,440 USDT** of the `21,600 USDT` principal base after the 15%–10% deduction.

## Example C — redeeming 1,000 USDT of rewards

<figure><img src="../.gitbook/assets/chart-redemption-lanes.svg" alt="Redemption lanes: T+0 nets 700 USDT and burns 300 USDT; 30-day linear nets 850 USDT and burns 150 USDT; 60-day linear nets 1,000 USDT and burns nothing"><figcaption>Only one variable separates the three lanes: how long you are willing to wait</figcaption></figure>

| Choice | Equivalent EXON permanently burned | Net received |
|---|---:|---:|
| T+0 | 300 USDT | 700 USDT |
| 30-day linear | 150 USDT | 850 USDT |
| 60-day linear | 0 USDT | 1,000 USDT |

The only variable that changes across the three lanes is **waiting time**. `Net = W × (1 − b)`, `Burn = W × b`.

*Previous: [Staking & Returns](staking-and-returns.md) · Next: [Value Flows](value-flows.md)*
