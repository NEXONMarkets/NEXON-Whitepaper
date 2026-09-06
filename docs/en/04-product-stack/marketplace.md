---
description: "The landing layer inside the ecosystem: where a Route's last leg becomes a delivered good or a booking, proven by a Landing Receipt."
icon: "store"
---

# Marketplace — the Real Leg

> Settlement to the real leg — a booking, a card limit, a delivered good. Not another swap.

The value of a Route is realised entirely in its last leg. The Marketplace is the landing inside the ecosystem; the Card is the landing outside it — only together does the agent truly touch the real world. This layer is the hardest, and the one that can least be skipped: a connection without a Real Leg is just another place to swap tokens.

That is why this paper groups the two under one name, the Storefront, and why the Marketplace comes first. It is the landing the protocol can see end to end — supplier, inventory, receipt — and so the first place where "Land the Real Leg" can be shown rather than asserted.

## The landing inside the ecosystem

### Marketplace

**Status** · `In development`

The Marketplace is the last leg's venue, not a shop with a token checkout. The Nexus Agent arrives with a Route whose earlier legs have landed and with EXON in escrow for this one. The Marketplace's job is to turn that escrow into a real thing — a good shipped, a booking confirmed — and hand back proof that it did. Nothing is browsed here in the ordinary sense. The agent is fulfilling an Intent, and the Marketplace is where the object of that Intent lives.

```mermaid
flowchart LR
    E["EXON escrow<br/><i>for the last leg</i>"] --> M["Marketplace<br/><i>landing layer</i>"]
    M --> G["A good · a booking<br/><i>Landing Receipt</i>"]
    M -.-> T["travel redemption<br/><i>Roadmap</i>"]
    %% NEXON palette v0 · placeholder until VI locks
    classDef navy  fill:#0B1220,stroke:#22D3EE,stroke-width:1.5px,color:#E6EDF3
    classDef cyan  fill:#22D3EE,stroke:#0B1220,stroke-width:1.5px,color:#0B1220
    classDef light fill:#E6EDF3,stroke:#0B1220,stroke-width:1px,color:#0B1220
    classDef ghost fill:#FFFFFF,stroke:#22D3EE,stroke-width:1px,stroke-dasharray:4 3,color:#0B1220
    class E cyan
    class M navy
    class G light
    class T ghost
```

### Landing Receipt and the dispute window

**Status** · `In development`

A Route does not close when the supplier is paid. It closes when the Real Leg can be shown. The Landing Receipt is that proof: a record that can be checked against the supplier's own system, not against a NEXON log alone. It opens a dispute window, and inside that window a Real Leg paid for and not delivered is handled as a partial unwind — escrow returns, the supplier's standing is affected, and the Route closes as partially unwound rather than complete.

### Who may be a supplier

**Status** · `In development`

Three conditions, no exceptions. Inventory must be real: what is offered exists, and is held when the leg executes. It must be refundable: a failed leg can be unwound in the supplier's own system. It must be verifiable: the supplier can produce a confirmation that stands as a Landing Receipt. A supplier that meets all three is a Leg Executor for the Real Leg. The set is an open parameter ([OP-15](../open-parameters/README.md)); this version names none.

### travel redemption

**Status** · `Roadmap`

The Tokyo example in Part II ends in four nights in a hotel. When that landing happens inside the ecosystem, it happens here: the booking is the Real Leg, the hotel is the supplier, the confirmation is the Landing Receipt. Nothing in the mechanism changes; only the object does. Travel redemption is `Roadmap`, and until it is built the Marketplace lands goods before it lands rooms.

## Inside and outside

{% columns %}
{% column %}
**Inside — the Marketplace.** The supplier is a Leg Executor the protocol has admitted. Inventory, refund and receipt are visible to the agent before the leg runs. This is the landing the protocol can vouch for.
{% endcolumn %}
{% column %}
**Outside — the Stablecoin Card.** The last leg becomes a spending limit on a card from a licensed issuer, and the real world is reached wherever that card is accepted. NEXON is only the access layer. This is the landing the protocol can enable but not vouch for. `Roadmap`.
{% endcolumn %}
{% endcolumns %}

<details>

<summary>The real leg is the hard part</summary>

Every earlier leg settles in a system built for settlement. The last one settles in a hotel's booking engine or a warehouse. A supplier can say yes and not deliver; a room can be confirmed and then overbooked. No chain can force delivery. Only escrow, receipt, dispute and standing can make it likely — and they are slow, manual and unglamorous to build. They are also the entire difference between a translation and a swap.

</details>

{% hint style="info" %}
**Scope of this section.** Commits to: the Marketplace as the in-ecosystem Real Leg, a Landing Receipt verifiable against the supplier's system, a dispute window that resolves into partial unwinds, and three admission conditions for suppliers. Does not commit to: any supplier, any category of goods, or travel redemption being available. Open items: [OP-15](../open-parameters/README.md).
{% endhint %}

*Spine: [The Translator](../02-the-translator/README.md) · Next: [Stablecoin Card](stablecoin-card.md)*
