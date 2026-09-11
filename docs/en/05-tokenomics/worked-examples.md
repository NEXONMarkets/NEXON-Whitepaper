---
description: "Four worked examples — release value, staking income, withdrawal burn, team rewards — every number reproducible from the current parameters."
icon: calculator
---

# Worked Examples

Four cases, all computed from the current parameters; wherever a price assumption is used, it is written into the sentence.

## Example A — the release value of a 30,000 USDT subscription <a href="#example-a-the-release-value-of-a-30-000-usdt-subscription" id="example-a-the-release-value-of-a-30-000-usdt-subscription"></a>

Subscribe `30,000 USDT` in the private sale at `0.1 USDT` and receive `300,000 EXON`.

```text
D = 300,000 ÷ 1,095 = 273.97 EXON / day
R_epoch = 273.97 ÷ 2 = 136.99 EXON / payout
ROI_month = (D × P_market × 30) ÷ P_in × 100%
```

The release speed is fixed: **273.97 EXON a day, 136.99 every 12 hours.** Every day pays, and every payout can be sold on NEX.

| Market price | Monthly release value | Monthly ROI | Subscription recovered in |
|---:|---:|---:|---:|
| 1.0 USDT (listing price) | 8,219.18 USDT | 27.40% | 3.65 months |
| 2.0 USDT | 16,438.36 USDT | 54.79% | 1.83 months |

The release schedule is fixed: every doubling of the price doubles the monthly payout. A 30,000 USDT subscription is paired with a 10,000 USDT XO stake, so both income lines start together — the staking line is Example B.

## Example B — staking 30,000 USDT <a href="#example-b-staking-30-000-usdt" id="example-b-staking-30-000-usdt"></a>

Deposit `P = 30,000 USDT`. The order splits on opening: `8,400 USDT` of fuel buys `8,400 EXON` at 1 USDT each into the fuel wallet; the rest is swapped into XO and staked, settling every 12 hours at 0.3% – 1.0%.

| Term | Bonus | Per day | Per settlement | Per month | Term total |
|---:|---:|---:|---:|---:|---:|
| 30 days | base | 180 – 600 USDT | 90 – 300 USDT | 5,400 – 18,000 USDT | 5,400 – 18,000 USDT |
| 90 days | +10% | 198 – 660 USDT | 99 – 330 USDT | 5,940 – 19,800 USDT | 17,820 – 59,400 USDT |
| 180 days | +20% | 216 – 720 USDT | 108 – 360 USDT | 6,480 – 21,600 USDT | 38,880 – 129,600 USDT |
| 360 days | +30% | 234 – 780 USDT | 117 – 390 USDT | 7,020 – 23,400 USDT | 84,240 – 280,800 USDT |
| 540 days | +50% | 270 – 900 USDT | 135 – 450 USDT | 8,100 – 27,000 USDT | 145,800 – 486,000 USDT |

**Read the per-day column**: 180 to 270 is the 1.5× bonus. The term total runs from 5,400 to 145,800 and beyond — that difference is time, and time works for the staker. Rewards land in XO and can be withdrawn at any time; once 100 USDT has accrued it can be staked as a new order.

## Example C — withdrawing 1,000 USDT of rewards <a href="#example-c-withdrawing-1-000-usdt-of-rewards" id="example-c-withdrawing-1-000-usdt-of-rewards"></a>

| Settlement | Burned | EXON burned (at 1.0 USDT) | Withdrawals a fuel wallet of 8,400 EXON supports |
|---|---:|---:|---:|
| Immediate | 30% | 300 | 28,000 USDT |
| 30-day linear | 20% | 200 | 42,000 USDT |
| 60-day linear | 10% | 100 | 84,000 USDT |

`Burn = W × b ÷ P_EXON`. What burns is EXON from the fuel wallet, gone from circulation for good; the only variable that changes between the three lanes is **how long you wait**. When fuel runs short, pick a slower settlement or top up through the private sale.

## Example D — a three-generation team <a href="#example-d-a-three-generation-team" id="example-d-a-three-generation-team"></a>

Refer 5 people who each stake 10,000 USDT, each of whom refers 5 more — 5 / 25 / 125 people across three generations. Referral rewards are calculated on each downline's daily static output:

| Generation | People · total staked | Rate | Per day |
|---|---|---:|---:|
| Gen 1 | 5 · 50,000 USDT | 15% | 45 – 150 USDT |
| Gen 2 | 25 · 250,000 USDT | 10% | 150 – 500 USDT |
| Gen 3 | 125 · 1,250,000 USDT | 10% | 750 – 2,500 USDT |
| **Total** | | | **945 – 3,150 USDT / day** |

An own stake of 100 USDT and four direct referrals unlock generations 1 – 4. As the team grows deeper, generation 4 pays 5% and the ladder runs to generation 20; each further block of generations opens as own stake and direct referrals reach the corresponding tier.

*Previous: [Staking & Returns](staking-and-returns.md) · Next: [Value Flows](value-flows.md)*
