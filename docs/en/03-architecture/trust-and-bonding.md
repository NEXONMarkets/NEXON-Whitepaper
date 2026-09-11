---
description: "The staking and reward layer: XO staking, the EXON fuel wallet, settlement every 12 hours and three settlement speeds, each independent of the app layer."
icon: layer-group
---

# Staking & Reward Layer

The authoritative product of this layer is the standalone **Staking Platform**, running NEXON's current economic mechanism (finalised 10 September 2026).

It has five core jobs: **open XO staking orders, buy 28% of every deposit into EXON in the fuel wallet, settle term-weighted rewards every 12 hours, settle 20 generations of referral rewards and V1 – V12 leadership bonuses, and execute withdrawals and burns across three settlement speeds.** It can share identity, account visibility and fund operations with the NEX exchange, but its reward rules are not part of the exchange's spot rulebook.

## One account, two operating layers <a href="#one-account-two-operating-layers" id="one-account-two-operating-layers"></a>

```mermaid
flowchart LR
    A["Unified account"] --> E["NEX exchange · spot layer"]
    A --> S["Staking Platform"]
    E --> X["XO trades freely · EXON sell only · daily release displayed"]
    S --> O["XO staking order"]
    O --> F["28% buys EXON → fuel wallet"]
    O --> R["Settled every 12 h at 0.3% – 1.0% × term bonus"]
    R --> D["Immediate · 30-day · 60-day settlement"]
    D --> B["Fuel wallet burns 30% · 20% · 10%"]
    classDef anchor fill:#047854,stroke:#047854,stroke-width:1.5px,color:#F5F3F0
    classDef engine fill:#8B5CF6,stroke:#8B5CF6,stroke-width:1.5px,color:#F5F3F0
    classDef solid fill:#F5F3F0,stroke:#141414,stroke-width:1.2px,color:#141414
    class A,E,X solid
    class S,O,R anchor
    class F,D,B engine
```

The NEX exchange **does not distribute** the staking rewards described here. Nor does the Staking Platform turn its own product variables into general payment, card, marketplace or agent rules.

## Opening an order <a href="#opening-an-order" id="opening-an-order"></a>

For a deposit `P`, the current mechanism records two entries:

```text
Fuel  = 0.28 × P   → buys EXON at 1 USDT each → fuel wallet (burn only)
Stake = the rest   → swapped into XO → staked, settled every 12 hours
```

<figure><img src="../.gitbook/assets/onepage-04-fuel-wallet.svg" alt="A 1,000 USDT deposit: 28%, or 280 USDT, buys 280 EXON at 1 USDT each into the fuel wallet — burn only, no transfer, no trading"><figcaption>A 1,000 USDT deposit: 280 EXON into the fuel wallet, the rest swapped into XO and earning</figcaption></figure>

The fuel wallet only ever fills: no transfers out, no trading, burned only when rewards are withdrawn. Minimum order 100 USDT. Every acquisition of EXON comes through the private sale and carries its own price and liquidity.

## A parameterised reward ledger <a href="#a-parameterized-reward-ledger" id="a-parameterized-reward-ledger"></a>

**Settlement every 12 hours, 0.3% – 1.0% each time, at 08:00 and 20:00 Beijing time**, multiplied by the term bonus:

```text
Per settlement = staked amount × (0.3% – 1.0%) × (1 + bonus)
```

<figure><img src="../.gitbook/assets/onepage-05-term-ladder.svg" alt="Term ladder: 30 days base, 90 days +10%, 180 days +20%, 360 days +30%, 540 days +50%; 1,000 USDT staked earns from 6–20 to 9–30 USDT a day"><figcaption>The longer the term, the higher the bonus — set by term alone, never by amount</figcaption></figure>

| Term | Bonus | 1,000 USDT staked · per day | At maturity | Cumulative lock |
|---:|---:|---:|---|---:|
| 30 days | base | 6 – 20 USDT | Day-31 exit window, no penalty | 1,200 days |
| 90 days | +10% | 6.6 – 22 USDT | Rolls into the next term | 1,170 days |
| 180 days | +20% | 7.2 – 24 USDT | Rolls into the next term | 1,080 days |
| 360 days | +30% | 7.8 – 26 USDT | Rolls into the next term | 900 days |
| 540 days | +50% | 9 – 30 USDT | Principal returned | 540 days |

Every order and every settlement records the **parameter version** it ran under. A later parameter change cannot quietly rewrite a historical accrual. The ledger keeps the deposit, term, bonus, settlement time, total rewards, and any correction or reversal with its stated reason.

## Withdrawal and burn <a href="#withdrawal-and-burn" id="withdrawal-and-burn"></a>

Rewards land in XO and can be withdrawn at any time through one of three settlement speeds:

<figure><img src="../.gitbook/assets/onepage-08-withdrawal-lanes.svg" alt="Withdraw 1,000 USDT: immediate settlement burns 300 EXON, 30-day burns 200, 60-day burns 100 (at 1.0 USDT)"><figcaption>The faster the settlement, the larger the burn: three outcomes of withdrawing 1,000 USDT of rewards</figcaption></figure>

| Settlement | Wait | Fuel-wallet burn |
|---|---:|---:|
| Immediate | none | 30% |
| 30-day linear | 30 days | 20% |
| 60-day linear | 60 days | 10% |

For a withdrawal `W` and burn share `b`: `Burn = W × b ÷ P_EXON`. Burned EXON leaves circulation for good. If the fuel wallet holds enough, settle immediately; if not, pick a slower settlement or top up through the private sale. **The platform never sells another asset to top up fuel on the user's behalf.**

## Referral rewards and leadership bonuses <a href="#referral-rewards-and-leadership-bonuses" id="referral-rewards-and-leadership-bonuses"></a>

Referral rewards are calculated on each downline's daily static output, up to 20 generations and 76% in total, unlocked block by block by own stake and direct referrals; leadership bonuses V1 – V12 are paid as a Differential Matching Bonus, assessed cumulatively on deposits with no demotion, and V10 – V12 share a global pool of 3% of XO deposits. Both settle in the same cycle as static rewards, are always paid in XO, and burn EXON from the fuel wallet on withdrawal in the same way. The full rate tables are in [Staking & Returns](../05-tokenomics/staking-and-returns.md).

## How it relates to the product ecosystem <a href="#how-it-relates-to-the-product-ecosystem" id="how-it-relates-to-the-product-ecosystem"></a>

The Staking Platform can appear inside the Wallet and be explained through the PayFi interface, but **an interface never creates a new source of yield**. The AI layer can explain term choices or simulate the formula under assumptions the user supplies; it cannot change the order split and cannot touch the fuel wallet.

In the narrative, XO is the Value Anchor and EXON the Circulation Engine — positions that explain the long-term ecosystem. The current staking and withdrawal operations are exactly what is written above.

## Six implementation controls <a href="#six-implementation-controls" id="six-implementation-controls"></a>

1. Parameter versions on recorded events are immutable except through a disclosed correction;
2. Fuel purchase, XO stake, each settlement, settlement-speed choice and burn each keep their own record;
3. Exchange permissions and staking permissions can be separated;
4. Every reward view distinguishes **pending / settling / settled**;
5. User-facing calculations state the price assumption they rely on next to the result;
6. Leadership execution rates are recorded by parameter version, and the interface shows the version governing each order.

This layer is the most concretely defined economic core today. The wider application architecture is built around it and does not rewrite it.

*Previous: [Settlement & Custody](settlement-and-custody.md) · Next: [Data & Oracles](data-and-oracles.md) · The full economics: [Token Economics](../05-tokenomics/README.md)*
