---
description: "A structured Intent schema keeps user goals, execution constraints and staking orders explicit."
icon: "comment-dots"
---

# Intent Layer

An Intent captures a goal without hiding the operations needed to achieve it. A minimal schema records the owner, desired outcome, amount, deadline, venue limits, price tolerance and approval mode. Missing material fields trigger clarification before a route is proposed.

Economic orders add a product type and parameter version. A staking order records principal `P`, EXON build `B`, staking base `S`, term, weight, fuel-reserve result and the redemption schedule selected later. The immutable relationship is:

```text
B = 0.28 × P
S = 0.72 × P
```

The schema must not repurpose EXON as an execution-cost unit for unrelated routes. Fees for non-staking products belong to their own disclosed terms.

*Next: [Agent Runtime](agent-runtime.md)*
