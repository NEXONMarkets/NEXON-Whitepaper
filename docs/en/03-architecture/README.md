---
description: "A Roadmap architecture for one coherent user experience across separate accounts, venues, staking rules, applications and real-world executors."
icon: "diagram-project"
---

# Protocol Architecture

> One experience does not require one system to own every asset, decision or obligation.

NEXON is designed as a coordination layer above the chains, venues, account systems and suppliers where value already lives. The architecture seeks a unified experience while preserving the native controls of every execution leg. This is essential to the value-connection thesis: a route becomes trustworthy because responsibility is visible, not because an interface hides it.

The architecture in this Part is a **Roadmap design** except where it restates the currently approved two-layer economic mechanism. It should not be read as evidence that an agent runtime, card integration, marketplace or cross-market route is operating today.

## Five responsibility domains

| Domain | Primary responsibility | Boundary |
|---|---|---|
| Unified identity and account services | Session, account view, eligibility references, permissions and user policy | A unified view does not merge custody or legal obligations |
| NEX Main Exchange / CEX | EXON spot activity, IEO and release display | It does not distribute NEXON staking rewards |
| Staking Platform | XO staking principal, order validation, term weighting, epoch rewards and redemption | Its rules do not become universal PayFi or marketplace rules |
| Roadmap application orchestration | Intent capture, route construction, policy checks, approval and receipts | It proposes and coordinates; it does not silently acquire custody or authority |
| Licensed or third-party execution | Regulated settlement, card issuance, merchant supply, travel inventory and other external legs | Each operator remains accountable under its own terms and jurisdiction |

One account may make these domains easier to navigate. It does not turn them into one balance sheet. A user should be able to see which domain currently holds an asset, which rules govern it and which party can resolve a failure.

## Functional subsystems

The Roadmap application layer is divided by responsibility rather than by screen.

| Subsystem | Responsibility | Core evidence |
|---|---|---|
| [Intent Layer](intent-layer.md) | Convert an objective and constraints into a structured, versioned request | Intent record |
| [Agent Runtime](agent-runtime.md) | Propose routes, apply policy, request approval and coordinate bounded execution | Route and authorization log |
| [Settlement & Custody](settlement-and-custody.md) | Reconcile native execution without pretending all assets share one custodian | Venue, chain or supplier receipt |
| [Staking & Reward Layer](trust-and-bonding.md) | Apply the approved XO/EXON order, epoch and redemption rules | Order and reward ledger |
| [Data & Oracles](data-and-oracles.md) | Supply prices, eligibility signals, inventory and failure thresholds | Timestamped source record |

These subsystems map directly to the six-stage control path: **Intent → Route → Policy Check → User Approval → Execution → Receipt.** The Intent Layer owns the first structured object. The runtime owns route construction, checks and authorization. Native executors own settlement or delivery. Reconciliation owns the receipt.

## The economic boundary that exists now

The current economic architecture is narrower and more precise than the product Roadmap. NEX Main Exchange/CEX carries EXON spot trading, IEO and release display. The Staking Platform carries single-token staking, term weighting, dynamic rewards and redemption. The platforms may share identity, account visibility and capital operations, but their ledgers, permissions and disclosures remain distinct.

A Staking Platform order applies the approved 72/28 structure. The 72% component establishes the XO staking/PV base. The 28% component purchases EXON into Treasury Liquidity. A matching 28% EXON balance is checked as fuel and remains in the user's account. This is a product-specific rule, not a generic architecture pattern and not a fee model for future applications.

## A route across boundaries

A future route may touch several domains without transferring responsibility to the agent. For example, a user could discover an opportunity in the Social App, inspect balances and permissions in the Wallet, review a conversion and purchase path in PayFi, then complete a service order through a marketplace supplier. The social product supplies context. The wallet exposes state. PayFi coordinates the proposal and approval. The venue settles the conversion. The supplier confirms delivery.

If the supplier fails after payment, the route does not label the entire journey successful. If the venue settles but delivery remains pending, the receipt shows both states. If a policy check becomes invalid, later legs stop. Architecture is the discipline of keeping those distinctions intact while the user experiences one connected flow.

## Non-negotiable controls

- **Least authority.** Each approval covers defined assets, destinations, amounts, actions and time.
- **No token-derived permission.** Holding XO or EXON does not by itself authorize an agent or broaden account access.
- **Versioned rules.** Every economic calculation and policy decision references the rules used at that time.
- **Separable custody.** An orchestration interface must identify the actual custodian or executor for every leg.
- **Observable failure.** Partial completion, pending delivery, dispute and reversal are first-class states.
- **Roadmap honesty.** Interfaces, integrations and cross-market routes are not current capabilities until their specifications and operators are published.

The result is not one monolithic protocol. It is a controlled connection among distinct systems, built around a common route and evidence model.

*Previous: [Not “AI Plus Payments”](../02-the-translator/not-ai-plus-payments.md) · Next: [Intent Layer](intent-layer.md)*
