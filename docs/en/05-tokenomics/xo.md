---
description: "XO is NEXON's narrative Value Anchor and, in the current approved mechanism, the protocol-priced Staking Principal Token."
icon: "circle-x"
---

# XO — Value Anchor

XO combines a long-term narrative position with a precise current function. In the approved NEXON narrative, XO is the **Value Anchor**: the asset associated with staking, participation, ecosystem rights and long-term value accumulation. In the approved economic mechanism, XO is the **Staking Principal Token** used inside the Staking Platform.

The second statement defines what happens now. The first describes why that function matters to the broader ecosystem.

## Name and narrative role

`X` represents cross-domain connection and possibility. `O` represents the ecosystem loop and value accumulation. Together, XO names the core asset around which durable participation can be organized.

“Value Anchor” does not mean a fixed market price, guaranteed backing or legal claim on a reserve. It describes an ecosystem role: XO is intended to hold the long-duration side of the dual-asset model while EXON handles active circulation.

## Current mechanical role

A user acquires XO from Treasury at a U-denominated price managed by the protocol. XO circulates internally under that mechanism and is independent of EXON's public secondary-market price.

For qualifying principal `P`, the staking base is:

```text
S = 0.72 × P
```

`S` is the XO staking and reward/PV base used in static reward calculation and dynamic reward accounting. The separate 28% EXON purchase does not increase `S`, and the matching EXON fuel-balance check does not become XO principal.

An order also records the term and weight. The current terms are 30, 90, 180, 360 and 540 days with weights 1.00, 1.10, 1.20, 1.35 and 1.50. Rewards accrue in 12-hour epochs using the published Base APY and selected weight. The 30-day term supports early exit with a 10%–15% deduction from `S`; the exact percentage within the band remains unpublished.

Calling XO principal does not mean the principal is protected. Protocol operation, contract failure, accounting error, custody, access, parameter change and legal restrictions can affect participation and recovery.

## Roadmap utility

The narrative anticipates broader participation, rights and governance utility for XO. These functions are **Roadmap**, not current rights. Before any becomes operational, a formal design should state:

- which decisions, products or communities are in scope;
- eligibility, thresholds and delegation rules;
- how conflicts of interest and concentrated holdings are handled;
- proposal, quorum, voting and execution processes if voting is used;
- whether rights are transferable or tied to verified participation;
- how emergency action, appeals and parameter changes work;
- which legal entity or contract is responsible.

Until those rules are published, holding XO should not be described as granting a live vote, revenue share, executive authority, product access guarantee or claim on NEXON or NEX assets.

## Relationship to the Roadmap products

The future Wallet may display XO positions, term choices, epoch history and redemption state. PayFi may explain or simulate a staking order. The Social App may provide participation context. None of those interfaces creates a second reward mechanism or changes the approved calculation.

If future marketplace, card or social products grant an XO-based benefit, the relevant product terms must define the benefit, funding source, eligibility, duration and change process. A narrative association with rights is insufficient on its own.

## What remains unpublished

The approved paper does not provide a numerical XO supply, external listing plan, comprehensive distribution, governance design or broader-rights schedule. XO's protocol-managed price should not be described as a public market guarantee. These fields remain Open.

## XO statement hierarchy

1. **Narrative:** XO is NEXON's Value Anchor and carries long-term ecosystem value.
2. **Current mechanism:** XO is the U-priced Staking Principal Token and carries `S = 0.72 × P` inside the Staking Platform.
3. **Roadmap:** broader participation, rights and governance require separate published rules.

{% hint style="danger" %}
XO is not equity, debt, a deposit or a guaranteed income claim. The protocol-priced mechanism does not ensure redemption value or principal protection. Participants may lose some or all principal.
{% endhint %}

*Previous: [Two Assets, Two Jobs](two-assets-two-jobs.md) · Next: [EXON — Circulation Engine](exon.md)*
