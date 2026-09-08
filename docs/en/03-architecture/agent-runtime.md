---
description: "Account-bound execution controls that do not derive authority from XO or EXON ownership."
icon: "microchip"
---

# Agent Runtime

The runtime is bound to one account and should hold scoped authority, not unrestricted keys. It proposes routes, waits for the required approval, grants one-leg permissions and checks revocation before the next action.

Three nested controls apply:

1. account and jurisdiction eligibility;
2. a visible route-level amount and deadline approved by the user;
3. asset, venue, amount and validity limits for each leg.

For a Staking Platform order, the runtime additionally validates `F = 0.28 × O` of EXON before opening the order. This is a balance check only; the EXON remains in the user's account. XO carries staking principal but does not set the agent's execution ceiling or governance rights.

Each event should log the responsible actor, rule version, input balances, decision and resulting receipt. Product-specific limits are independent of token ownership unless the approved terms explicitly say otherwise.

*Next: [Settlement & Custody](settlement-and-custody.md)*
