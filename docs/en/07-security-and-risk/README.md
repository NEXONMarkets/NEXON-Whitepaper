---
description: "Five classes of threat to an agent that moves value on your behalf, how the design answers each, and the three limits it does not hide."
icon: "shield-halved"
---

# Security & Risk

> The agent translates for you; it does not decide for you.

Part II drew a line between a caged agent and a translator, and said the cage answers a safety question rather than a capability one. This section is that safety question, taken on its own terms. An agent that proposes a Route across three markets, holds it in view while every leg executes, and lands the last leg outside the protocol touches more kinds of risk than a payment app does — and each has to be answered without turning the translator back into a hand.

Every action the agent takes is bounded, visible and recorded. Each mitigation below is one of those three properties applied to a specific threat; where the design reaches a limit it cannot engineer past, the limit is stated.

## Five classes of threat

{% tabs %}
{% tab title="Agent authority" %}
**The threat.** An agent with standing to act can act beyond what you meant — a larger amount, a venue you would not have chosen, a leg you never approved.

**The answer.** Authority is layered, and every layer is narrower than the one outside it. The outer ceiling is Capacity — the execution the XO you have bonded entitles your agent to — checked at Bond Check before any Route can be proposed. Inside it, every Route is shown to you as a preview, leg by leg with quote and expiry, and executes only if you approve. Inside the Route, each leg runs under a scoped delegation naming the asset, the venue, the amount and an expiry. While a Route executes, the Capacity it needs is held as a Capacity Reservation and released when the Route closes.

Revocation is on-chain and immediate: a delegation withdrawn through the revocation registry stops the next leg from starting. A Pre-approved envelope that would let a class of Routes run without per-Route approval is `Roadmap` (OP-18), not part of the v1 design.
{% endtab %}

{% tab title="Keys" %}
**The threat.** Whoever holds the keys holds the assets. A runtime that holds your keys is a single point of failure and the most valuable target on the network.

**The answer.** You custody your own assets. The Nexus Agent never holds your root keys; it holds delegations — scoped to one leg, expiring on their own, revocable at any time. A compromised runtime therefore exposes at most the legs currently delegated to it, for at most their remaining validity. Recovery for a lost delegate key follows a time-locked path in which no single party can act alone (`Design Target`). Recovery for your root keys is a wallet question, not a protocol one, and this paper does not pretend otherwise.
{% endtab %}

{% tab title="Contracts" %}
**The threat.** The protocol's own contracts — the Bond ledger, Route escrow, the revocation registry — are code, and code has bugs.

**The answer.** The on-chain surface is kept small. The protocol holds only what it must: bonded XO in the Bond ledger, and EXON in escrow for the duration of a Route. The assets that move through a Route's legs are never held by the protocol at all. Upgrades pass through the time-locked ladder in [Governance](../06-governance/README.md), so a change cannot reach the contracts faster than Seat holders can read it. An audit is `In development`; its scope is an Open Parameter (OP-28). This paper names no auditor and claims no result ahead of one.
{% endtab %}

{% tab title="Market" %}
**The threat.** A quote moves between preview and execution. A leg fills worse than shown, or not at all, and the Route no longer means what you approved.

**The answer.** Every quote in a preview carries an expiry; a leg whose quote has expired is re-quoted, and the Route returns to you if the new quote breaches your constraints. Those constraints are part of the Intent itself — `max_slippage`, `max_burn_rate`, a deadline. A fill outside them is a failed leg, and a failed leg triggers Rollback along the path it came. Route finality is the finality of its slowest leg. Circuit breakers on stale, deviating or unavailable data pause a Route before a leg runs on bad information; their thresholds are a `Design Target` (OP-17).
{% endtab %}

{% tab title="Counterparty and the Real Leg" %}
**The threat.** The last leg lands outside the protocol. A supplier is paid and does not deliver; a booking is confirmed and then cancelled; a card limit is issued and then withdrawn.

**The answer.** Every Real Leg closes with a Landing Receipt — a verifiable record of what the Leg Executor confirmed — which opens a dispute window before the Route is finally closed. A Leg Executor joins on three conditions: its inventory is real, its confirmations are verifiable, its legs can be refunded. Where a Real Leg cannot be reversed after earlier legs already have been, the Route enters `Partially unwound`. What remains is resolved from EXON escrow first and, only if that is exhausted, from the XO held under Capacity Reservation for that Route; the order and limits of that recourse are `Open` (OP-10).
{% endtab %}
{% endtabs %}

A sixth class — data that is stale, deviating, unavailable, spoofed or disputed — runs through every leg above and is treated where data enters the system, in [Data & Oracles](../03-architecture/data-and-oracles.md).

## What the design does not hide

{% hint style="danger" %}
**Three limits this design has, and states.**

**Partial unwinds can require human resolution.** Rollback is automatic while every leg is reversible. Once a Real Leg has landed, code alone cannot always restore the prior state, and a `Partially unwound` Route may need a person — the Leg Executor, a Seat Council member, you — to settle what remains.

**The Real Leg is the hardest leg.** Suppliers, issuers and licensed venues sit outside the protocol. The protocol verifies their receipts; it does not control their inventory, their systems or their solvency.

**Chain-agnostic means inheriting every chain's risk.** Each leg settles where its asset is native, so a Route is exposed to the finality, congestion and contract risk of every chain and venue it touches. The Translation Layer removes the need for a bridge; it does not remove the chains.
{% endhint %}

## Three layers, one sentence

Everything above reduces to three constraints a Route is under from the moment it is proposed.

① An agent's execution ceiling is set by the XO you have bonded — its Capacity; a route beyond that ceiling cannot even be proposed. ② Every Route is visible and refusable before it executes — you are the approver, not a bystander. ③ If any leg fails mid-execution, Rollback returns everything along the path it came. In one sentence: the agent translates for you; it does not decide for you.

{% hint style="info" %}
**Scope of this section.** Commits to: layered authority (Capacity, Route approval, scoped delegation, on-chain revocation), self-custody with delegated keys, Rollback on any failed leg, and a Landing Receipt with a dispute window on every Real Leg. Does not commit to: any named auditor, any recovery mechanism beyond a time-locked path, or automatic resolution once a Real Leg has landed. Open items: [OP-10 · OP-17 · OP-18 · OP-28](../open-parameters/README.md).
{% endhint %}

*Spine: [The Translator](../02-the-translator/README.md) · Next: [Compliance & Legal Posture](../08-compliance/README.md)*

*Turning what you mean into what gets settled.*
