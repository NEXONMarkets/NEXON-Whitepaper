---
description: "Four worked examples — release value, 10,000 USDT staked with and without restaking, withdrawal burn, team rewards — all from the current parameters."
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

## Example B — staking 10,000 USDT <a href="#example-b-staking-10-000-usdt" id="example-b-staking-10-000-usdt"></a>

Deposit `P = 10,000 USDT`. The order splits on opening: `2,800 USDT` of fuel buys `2,800 EXON` at 1 USDT each as fuel; the rest is swapped into XO and staked, settling every 12 hours at 0.2% – 0.6% — 40 – 120 USDT a day.

**Rewards on the original order only**, at maturity:

| Term | Term bonus | Daily output with bonus | Rewards at maturity | Principal + rewards at maturity | Multiple of principal |
| :-- | --: | --: | --: | --: | --: |
| 30 days | none | 40 – 120 USDT | 1,200 – 3,600 USDT | 11,200 – 13,600 USDT | 1.1× – 1.6× |
| 90 days | +10% | 44 – 132 USDT | 3,960 – 11,880 USDT | 13,960 – 21,880 USDT | 1.2× – 3.0× |
| 360 days | +30% | 52 – 156 USDT | 18,720 – 56,160 USDT | 28,720 – 66,160 USDT | 6.0 × – 10.4× |
| 540 days | +50% | 60 – 180 USDT | 32,400 – 97,200 USDT | 42,400 – 107,200 USDT | 2.6× – 10.7 × |

**Reinvest and compound.** Rewards are reinvested as they land: a reinvested order carries the same term bonus as the original, settles every 12 hours, and its own rewards keep compounding — all the way to the original order's maturity. Total at maturity = principal + original order rewards + reinvested rewards. At 0.2% per settlement:

| Term | Original order rewards | New order rewards | Principal + all rewards at maturity | Multiple of principal | Original order only |
| :-- | --: | --: | --: | --: | --: |
| 30 days | 1,200 USDT | 68 USDT | **11,268 USDT** | **1.1×** | 1.1× |
| 90 days | 3,960 USDT | 871 USDT | **14,831 USDT** | **1.5×** | 1.4× |
| 360 days | 18,720 USDT | 35,945 USDT | **64,665 USDT** | **6.5×** | 2.9× |
| 540 days | 32,400 USDT | 211,006 USDT | **253,406 USDT** | **25.3×** | 4.2× |

The longer the term, the more it compounds: the 540-day term ends at **253,406 USDT, 25.3 × the principal**, against 2.6× on the original order alone. Time works for the staker.

## Example C — withdrawing 10,000 USDT of rewards <a href="#example-c-withdrawing-10-000-usdt-of-rewards" id="example-c-withdrawing-10-000-usdt-of-rewards"></a>

| Settlement | Burned | EXON burned (at 1.0 USDT) | Withdrawals a fuel balance of 2,800 EXON supports |
|---|---:|---:|---:|
| Immediate | 30% | 3,000 | 9,333 USDT |
| 30-day linear | 20% | 2,000 | 14,000 USDT |
| 60-day linear | 10% | 1,000 | 28,000 USDT |

`Burn = W × b ÷ P_EXON`. What burns is EXON from the fuel, gone from circulation for good; the only variable that changes between the three lanes is **how long you wait**. When fuel runs short, pick a slower settlement or top up through the private sale.

## Example D — a three-generation team <a href="#example-d-a-three-generation-team" id="example-d-a-three-generation-team"></a>

Refer 5 people who each stake 10,000 USDT, each of whom refers 5 more — 5 / 25 / 125 people across three generations. Referral rewards are calculated on each downline's daily static output:

| Generation | People · total staked | Rate | Per day |
|---|---|---:|---:|
| Gen 1 | 5 · 50,000 USDT | 15% | 30 – 90 USDT |
| Gen 2 | 25 · 250,000 USDT | 10% | 100 – 300 USDT |
| Gen 3 | 125 · 1,250,000 USDT | 10% | 500 – 1,500 USDT |
| **Total** | | | **630 – 1,890 USDT / day** |

An own stake of 100 USDT and four direct referrals unlock generations 1 – 4. As the team grows deeper, generation 4 pays 5% and the ladder runs to generation 20; each further block of generations opens as own stake and direct referrals reach the corresponding tier.

*Previous: [Staking & Returns](staking-and-returns.md) · Next: [Value Flows](value-flows.md)*
