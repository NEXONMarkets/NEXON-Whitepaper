---
description: "XO is NEXON's narrative Value Anchor and, in the current mechanism, the protocol-priced Staking Principal Token."
icon: circle-x
---

# XO — Value Anchor

XO holds a long-term position and a precise current function under one name.

In the NEXON narrative, XO is the **Value Anchor**: the side associated with staking, participation, ecosystem rights and long-term value accumulation. In the approved economic mechanism, XO is the **Staking Principal Token** used inside the Staking Platform.

The second sentence defines what happens now. The first explains why that function matters to the ecosystem.

## Name and narrative role

`X` stands for cross-domain connection and possibility. `O` stands for the ecosystem loop and value accumulation. Together, XO names the asset **around which durable participation can be organized**.

"Value Anchor" describes an ecosystem role, not a price commitment: XO carries the long-duration half of the dual-asset model while EXON handles active circulation.

## The current mechanical role

A user acquires XO from Treasury at a USDT-denominated price managed by the protocol. XO circulates internally under that mechanism, independent of EXON's public secondary-market price.

For qualifying principal `P`, the staking base is:

```text
S = 0.72 × P
```

`S` is the XO staking / PV base used in static reward calculation and dynamic reward accounting. **The separate 28% EXON purchase does not increase `S`**, and the matching EXON balance check does not become XO principal.

The order also records term and weight:

| Term | 30 days | 90 days | 180 days | 360 days | 540 days |
|---|---:|---:|---:|---:|---:|
| Weight `w` | 1.00 | 1.10 | 1.20 | 1.35 | 1.50 |

Rewards accrue in 12-hour epochs using the published Base APY parameter and the selected weight. That parameter is adjustable and may change by issuance round, so an accrual is always read against the parameter version recorded on the order. The 30-day term supports early exit with a 10%–15% deduction from `S`; the exact rate inside that band has not been published.

## Long-term direction (Roadmap)

The narrative anticipates broader participation, rights and governance utility for XO. Those belong to the **long-term direction**, not to current rights. Before any of them goes live, a formal design has to state:

* what governance covers and what it does not;
* eligibility, thresholds and delegation rules;
* how conflicts of interest and concentrated holdings are handled;
* if voting is used: proposal, quorum, voting and execution processes;
* whether rights are transferable or tied to verified participation;
* how emergency action, appeals and parameter changes work;
* which legal entity or contract is responsible.

Until those rules are published, holding XO is not a live vote, a revenue share, an executive authority, or a claim on NEXON or NEX assets (see [Open Parameters](../open-parameters/README.md), OP-G01).

## Relationship to the product ecosystem

The Wallet can display XO positions, term choices, epoch history and redemption state. PayFi can explain or simulate a staking order. The Social App can supply participation context. **None of those interfaces creates a second reward mechanism or alters the confirmed calculation.**

If a future marketplace, card or social product grants an XO-based benefit, its product terms have to define what the benefit is, what funds it, who qualifies, how long it lasts and how it changes. A narrative association with "rights" is not enough on its own.

## XO in three sentences

1. **Narrative:** XO is NEXON's Value Anchor and carries long-term ecosystem value.
2. **Current mechanism:** XO is the USDT-priced Staking Principal Token and carries `S = 0.72 × P` inside the Staking Platform.
3. **Long-term direction:** broader participation, rights and governance require separately published rules.

*Previous: [Two Assets, Two Jobs](two-assets-two-jobs.md) · Next: [EXON — Circulation Engine](exon.md)*
