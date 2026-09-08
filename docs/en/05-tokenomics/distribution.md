---
description: "Approved early-round tiers, TGE guide price, later-round release rule and 1,095-day EXON vesting."
icon: "chart-pie"
---

# Distribution & Release

## Pricing and rounds

| Stage | Price mechanism | Release |
|---|---|---|
| Early round | Fixed at `0.1 U` with capped tiers | Enters the common 1,095-day release from TGE |
| TGE | Guide price `1.0 U`; NEX spot market opens | Linear release begins |
| Later rounds | Discount to prevailing market price; discount disclosed per round | Release begins T+1 |

The early-round capacity stated by the project paper is:

| Order size | Shares | Gross value |
|---:|---:|---:|
| 1,000 U | 10,000 | 10,000,000 U |
| 5,000 U | 1,000 | 5,000,000 U |
| 10,000 U | 500 | 5,000,000 U |
| **Total** | **11,500** | **20,000,000 U** |

## Linear release

An allocation `A` releases over 1,095 days in two 12-hour epochs per day, for 2,190 epochs:

```text
D = A / 1,095
R_epoch = D / 2 = A / 2,190
```

Released EXON enters the spot account and may be held or traded. Market access, liquidity and execution price are not guaranteed.

## Unpublished fields

- Numerical EXON total supply.
- Complete team, ecosystem, Treasury and market allocation.
- Initial circulating supply.
- Later-round size, discount and individual cap.
- Final TGE and round dates.

*Previous: [EXON](exon.md) · Next: [Staking & Returns](staking-and-returns.md)*
