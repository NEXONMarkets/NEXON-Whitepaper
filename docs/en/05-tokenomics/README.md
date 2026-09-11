---
description: "NEXON's current economics: two asset roles, XO staking settled every 12 hours, a fuel wallet that only fills, burn on withdrawal, and a 0.1 → 1.0 USDT sale."
icon: coins
---

# Token Economics

> NEXON is the ecosystem. XO carries value. EXON drives circulation.

This part sets out NEXON's current economic mechanism (finalised 10 September 2026, confirmed line by line on 11 September) and maps the narrative positioning — XO as **Value Anchor**, EXON as **Circulation Engine** — onto every number in it.

## Read each asset on three levels <a href="#read-each-asset-on-three-levels" id="read-each-asset-on-three-levels"></a>

| Level | XO | EXON |
|---|---|---|
| **Narrative** | Value Anchor: staking, participation, governance and long-term value | Circulation Engine: connecting the exchange, payment, exchange, fees and consumption |
| **Current mechanism** | Staking Principal Token; static rewards, referral rewards and leadership bonuses are all paid in XO; trades freely on NEX | Core Value Token; the private sale at 0.1 USDT is the only way to acquire it, listing at 1.0 USDT; sell only, never buy; 28% of every deposit buys EXON into the fuel wallet, burned on withdrawal |
| **Opening with each entry point** | Governance rules and wider ecosystem rights (Roadmap) | Trading, payment, exchange and fees, connected as each of the five entry points goes live (Roadmap) |

The narrative says what each asset **carries for the ecosystem**; the mechanism says how it **runs today**. Say both.

## One account, two operating layers <a href="#one-account-two-operating-layers" id="one-account-two-operating-layers"></a>

The **NEX exchange** is the spot layer: XO trades freely, EXON lists sell orders only with no buy orders, and the daily release is displayed from listing day. The **Staking Platform** handles XO staking, settlement every 12 hours, term bonuses, referral rewards, leadership bonuses and reward withdrawal. Both share one account system and one back office — open one account, move between the two.

## How a deposit splits <a href="#how-a-deposit-splits" id="how-a-deposit-splits"></a>

Every staking deposit `P` is split in two the moment the order opens, automatically:

```text
Fuel  = 0.28 × P   → buys EXON at 1 USDT each → fuel wallet (burn only)
Stake = the rest   → swapped into XO → staked, settled every 12 hours
```

<figure><img src="../.gitbook/assets/onepage-04-fuel-wallet.svg" alt="A 1,000 USDT deposit: 28%, or 280 USDT, buys 280 EXON at 1 USDT each into the fuel wallet — burn only, no transfer, no trading"><figcaption>A 1,000 USDT deposit: 280 EXON into the fuel wallet, the rest swapped into XO and earning</figcaption></figure>

{% hint style="success" %}
**The fuel wallet only ever fills.** Nothing in it can be transferred out or traded; its EXON has one destination — burned when rewards are withdrawn. The more is staked, the more is bought; the more is withdrawn, the more is burned.
{% endhint %}

## The economic lifecycle <a href="#the-economic-lifecycle" id="the-economic-lifecycle"></a>

**Staking.** XO staking settles every 12 hours at 0.3% – 1.0% per settlement, at 08:00 and 20:00 Beijing time; 1,000 USDT staked earns 6 – 20 USDT a day. Terms of 30 / 90 / 180 / 360 / 540 days carry bonuses of base / +10% / +20% / +30% / +50%, set by term alone. Day 31 is the exit window of the 30-day term — principal plus rewards, no penalty; miss it and the order renews 90 → 180 → 360 → 540 days.

**Withdrawal.** Rewards land in XO and can be withdrawn at any time, through one of three settlement speeds: immediate with a 30% burn, 30-day with 20%, 60-day with 10%. What burns is the equivalent EXON in the fuel wallet, gone from circulation for good.

**Private sale and release.** EXON supply is 1 billion; the private sale offers only 200 million at 0.1 USDT, in three tiers of 1,000 / 5,000 / 10,000 USDT and 11,500 allocations, each paired with an XO stake at 3:1. Listing is at 1.0 USDT, followed by 1,095 days of daily release — one payout every 12 hours, 2,190 in total.

**Dynamic rewards.** Referral rewards reach 20 generations and 76% in total, calculated on each downline's daily static output; leadership bonuses V1 – V12 are paid on the level differential, and V10 – V12 share a global pool of 3% of XO deposits. All are paid in XO, settled in the same cycle as static rewards, and burn on withdrawal in the same way.

## In this part <a href="#in-this-part" id="in-this-part"></a>

<table data-view="cards"><thead><tr><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><strong>Two Assets, Two Jobs</strong></td><td>Why storing value and moving it cannot be the same job.</td><td><a href="two-assets-two-jobs.md">two-assets-two-jobs.md</a></td></tr><tr><td><strong>Distribution &amp; Release</strong></td><td>Three sale tiers, the 3:1 pairing, listing at 1.0 USDT, 1,095 days of linear release.</td><td><a href="distribution.md">distribution.md</a></td></tr><tr><td><strong>Staking &amp; Returns</strong></td><td>0.3% – 1.0% every 12 hours, term bonuses, the exit window, three settlement speeds, 20 generations and V1 – V12.</td><td><a href="staking-and-returns.md">staking-and-returns.md</a></td></tr><tr><td><strong>Worked Examples</strong></td><td>Four cases — release value, staking income, withdrawal burn, team rewards — every number reproducible.</td><td><a href="worked-examples.md">worked-examples.md</a></td></tr><tr><td><strong>Value Flows</strong></td><td>Six flows, each on its own ledger, converging on one flywheel.</td><td><a href="value-flows.md">value-flows.md</a></td></tr><tr><td><strong>XO and EXON</strong></td><td>Each asset's name, role and current mechanism.</td><td><a href="xo.md">xo.md</a></td></tr></tbody></table>

*Next: [Two Assets, Two Jobs](two-assets-two-jobs.md)*
