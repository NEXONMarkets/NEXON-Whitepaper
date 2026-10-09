---
description: "Four worked examples — release value, 10,000 USDT deposited with and without restaking, withdrawal burn, team rewards — all from the current parameters."
icon: calculator
---

# Worked Examples

Four cases, all computed from the current parameters; wherever a price assumption is used, it is written into the sentence.

## Example A — the release value of a 30,000 USDT subscription <a href="#example-a-the-release-value-of-a-30-000-usdt-subscription" id="example-a-the-release-value-of-a-30-000-usdt-subscription"></a>

Subscribe `30,000 USDT` in the private sale at `0.1 USDT` and receive `300,000 NX`.

```text
D = 300,000 ÷ 1,095 = 273.97 NX / day
R_epoch = 273.97 ÷ 2 = 136.99 NX / payout
ROI_month = (D × P_market × 30) ÷ P_in × 100%
```

The release speed is fixed: **273.97 NX a day, 136.99 every 12 hours.** Every day pays, and every payout can be sold on NEX.

| Market price | Monthly release value | Monthly ROI | Subscription recovered in |
|---:|---:|---:|---:|
| 1.0 USDT (listing price) | 8,219.18 USDT | 27.40% | 3.65 months |
| 2.0 USDT | 16,438.36 USDT | 54.79% | 1.83 months |

The release schedule is fixed: every doubling of the price doubles the monthly payout. A 30,000 USDT subscription is paired with a 10,000 USDT XO stake, so both income lines start together — the staking line is Example B.

## Example B — staking 10,000 USDT <a href="#example-b-staking-10-000-usdt" id="example-b-staking-10-000-usdt"></a>

Deposit `P = 10,000 USDT`. The order splits on opening: `2,800 USDT` of fuel buys `2,800 NX` at 1 USDT each as fuel; the rest is swapped into XO and staked, settling every 12 hours at 0.2% – 0.6% — 0.4% – 1.2% a day, or 28.8 – 86.4 USDT.

**Rewards on the original order only**, at maturity:

| Term | Term bonus | Daily output with bonus | Rewards at maturity | Principal + rewards at maturity | Multiple of principal |
| :-- | --: | --: | --: | --: | --: |
| 30 days | none | 28.8 – 86.4 USDT | 864 – 2,592 USDT | 8,064 – 9,792 USDT | 1.1× – 1.4× |
| 90 days | +10% | 31.7 – 95 USDT | 2,851.2 – 8,553.6 USDT | 10,051.2 – 15,753.6 USDT | 1.4× – 2.2× |
| 360 days | +30% | 37.4 – 112.3 USDT | 13,478.4 – 40,435.2 USDT | 20,678.4 – 47,635.2 USDT | 2.9× – 6.6× |
| 540 days | +50% | 43.2 – 129.6 USDT | 23,328 – 69,984 USDT | 30,528 – 77,184 USDT | 4.2× – 10.7× |

**Reinvest and compound.** Rewards are reinvested as they land: a reinvested order carries the same term bonus as the original, settles every 12 hours, and its own rewards keep compounding — all the way to the original order's maturity. Total at maturity = principal + original order rewards + reinvested rewards. At 0.2% per settlement:

| Term | Original order rewards | New order rewards | Principal + all rewards at maturity | Multiple of principal | Original order only |
| :-- | --: | --: | --: | --: | --: |
| 30 days | 864 USDT | 47 USDT | **8,111 USDT** | **1.1×** | 1.1× |
| 90 days | 2,851 USDT | 621 USDT | **10,672 USDT** | **1.5×** | 1.4× |
| 360 days | 13,478 USDT | 25,799 USDT | **46,477 USDT** | **6.5×** | 2.9× |
| 540 days | 23,328 USDT | 151,616 USDT | **182,144 USDT** | **25.3×** | 4.2× |

The longer the term, the more it compounds: the 540-day term ends at **182,144 USDT, 25.3× the principal**, against 4.2× on the original order alone. Time works for the staker.

## Example C — withdrawing 10,000 USDT of rewards <a href="#example-c-withdrawing-10-000-usdt-of-rewards" id="example-c-withdrawing-10-000-usdt-of-rewards"></a>

| Settlement | Burned | NX burned (at 1.0 USDT) | Withdrawals a fuel balance of 2,800 NX supports |
|---|---:|---:|---:|
| Immediate | 30% | 3,000 | 9,333 USDT |
| 30-day linear | 20% | 2,000 | 14,000 USDT |
| 60-day linear | 10% | 1,000 | 28,000 USDT |

`Burn = W × b ÷ P_NX`. What burns is NX from the fuel, gone from circulation for good; the only variable that changes between the three lanes is **how long you wait**. When fuel runs short, pick a slower settlement or top up through the private sale.

## Example D — a three-generation team <a href="#example-d-a-three-generation-team" id="example-d-a-three-generation-team"></a>

Refer 5 people, each of whom refers 5 more: 5 / 25 / 125 people across three generations, everyone staking 10,000 USDT and producing 28.8 – 86.4 USDT of static yield a day. The referral reward is that generation's combined daily static output times that generation's rate:

| Generation | People in it | Their combined daily static output | Rate | Your daily referral reward |
|---|---:|---:|---:|---:|
| Gen 1 | 5 | 200 – 600 USDT | 15% | 21.6 – 64.8 USDT |
| Gen 2 | 25 | 1,000 – 3,000 USDT | 10% | 100 – 300 USDT |
| Gen 3 | 125 | 5,000 – 15,000 USDT | 10% | 500 – 1,500 USDT |
| **Three generations** | | | | **630 – 1,890 USDT / day** |

An own stake of 100 USDT and 4 qualified direct referrals already open generations 1 – 4. As the team grows deeper, generation 4 pays 5% and the ladder runs to generation 20; each additional qualified direct referral opens one more generation, provided the own stake has reached the matching tier. Rewards are paid in NX, with USDT as the unit of account, and the downline's own static yield is never reduced.

*Previous: [Staking & Returns](staking-and-returns.md) · Next: [Value Flows](value-flows.md)*
