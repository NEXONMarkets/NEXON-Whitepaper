---
description: "Custody, reconciliation and rollback boundaries for product execution, EXON spot activity and staking redemption."
icon: "shield-halved"
---

# Settlement & Custody

Assets remain subject to the custody terms of the account, venue, contract or supplier that actually holds them. An agent instruction is not custody, and a route proposal does not move funds.

NEX spot records cover EXON purchases, sales and vesting releases. Staking records cover XO principal, the order parameter version, epoch accruals and the selected redemption schedule. Treasury records cover the EXON acquired by the 28% build. These ledgers must reconcile without merging their legal or operational responsibilities.

Reward redemption produces two explicit values:

```text
Net = W × (1 − b)
Burn = W × b
```

The system must verify the equivalent EXON burn and issue a permanent destruction record before completing a burn-bearing redemption. This mechanism is unrelated to a route fee.

Failures require a defined state, responsible party and audit trail. Neither an automated rollback nor a Treasury balance guarantees recovery of user funds.

*Next: [Staking & Reward Layer](trust-and-bonding.md)*
