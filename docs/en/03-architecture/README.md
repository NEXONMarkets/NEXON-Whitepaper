---
description: "The application architecture and the strict boundary between NEX spot operations and the configurable Staking Platform."
icon: "diagram-project"
---

# Protocol Architecture

NEXON is an application layer above the chains, venues and suppliers where assets and services already live. Each execution leg remains subject to its native system and responsible party.

## Core subsystems

| Subsystem | Responsibility |
|---|---|
| Intent Layer | Structured goals and constraints |
| Agent Runtime | Route proposal, approval, scoped delegation and revocation |
| Settlement & Custody | Native execution, reconciliation, rollback and dispute records |
| Staking & Reward Layer | XO principal, EXON reserve checks, 12-hour reward ledger and redemption |
| Data & Oracles | Prices, eligibility attestations, inventory and circuit breakers |

The economic boundary is explicit: NEX Main Exchange/CEX carries EXON spot trading, IEO and release display. The Staking Platform carries single-token staking, term weighting and dynamic rewards. A unified account may expose both, but permissions, ledgers, disclosures and parameter versions remain separate.

Legacy token-role definitions must not be restored in architecture chapters. Current canonical roles are fixed in [Two Assets, Two Jobs](../05-tokenomics/two-assets-two-jobs.md).

*Next: [Intent Layer](intent-layer.md)*
