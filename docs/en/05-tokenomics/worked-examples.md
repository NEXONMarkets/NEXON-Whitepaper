---
description: "Complete conditional examples from the approved model, including monthly ROI, static payback math, term rewards and redemption outcomes."
icon: "calculator"
---

# Worked Examples

{% hint style="danger" %}
The following figures are protocol parameters and conditional illustrations provided only to explain the calculation method. They are not promises of yield, price, payback period or principal protection. APY, token prices, reward rates, execution parameters and outcomes may change or fluctuate, and participants may lose some or all principal.
{% endhint %}

## Example A — early EXON release value

An input of `30,000 U` at the early price of `0.1 U` acquires `300,000 EXON`.

```text
D = 300,000 / 1,095 = 273.97 EXON/day
R_epoch = 273.97 / 2 = 136.99 EXON/epoch
ROI_month = (D × P_market × 30) / P_in × 100%
```

| Assumed market price | Monthly released value | Monthly ROI illustration |
|---:|---:|---:|
| 1.0 U | 8,219.18 U | 27.40% |
| 2.0 U | 16,438.36 U | 54.79% |

Only if the `2.0 U` price and all other simplifying assumptions held, the static payback arithmetic would be `30,000 / 16,438.36 ≈ 1.83 months`. This is a mathematical scenario, not a price forecast or payback promise. It omits liquidity, slippage, fees, taxes and execution constraints.

## Example B — 30,000 U staking order

For `P = 30,000 U`, the build is `B = 8,400 U` and the staking base is `S = 21,600 U`. At a conditional `0.1 U` build price, `B` buys `84,000 EXON`.

| Term | Weight | Daily | Per epoch | Term total |
|---:|---:|---:|---:|---:|
| 30 days | 1.00 | 118.36 U | 59.18 U | 3,550.68 U |
| 90 days | 1.10 | 130.19 U | 65.10 U | 11,717.26 U |
| 180 days | 1.20 | 142.03 U | 71.01 U | 25,564.93 U |
| 360 days | 1.35 | 159.78 U | 79.89 U | 57,521.10 U |
| 540 days | 1.50 | 177.53 U | 88.77 U | 95,868.49 U |

The 540-day weight produces an effective 300% APY parameter. Early exit from the 30-day term returns `18,360–19,440 U` of the `21,600 U` principal base after the 15%–10% deduction.

## Example C — redeeming 1,000 U of rewards

| Choice | Equivalent EXON permanently burned | Net received |
|---|---:|---:|
| T+0 | 300 U | 700 U |
| 30-day linear | 150 U | 850 U |
| 60-day linear | 0 U | 1,000 U |

*Previous: [Staking & Returns](staking-and-returns.md) · Next: [Value Flows](value-flows.md)*
