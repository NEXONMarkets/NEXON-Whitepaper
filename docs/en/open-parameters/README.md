---
description: "Every parameter this paper leaves open, in one table: what it is, where it is referenced, its status, which role owns it and when it is expected."
icon: "list-check"
layout:
  width: wide
---

# Open Parameters

{% hint style="info" %}
**v2 fills cells, does not rewrite chapters.** Every chapter describes its mechanism in full and leaves the numbers, names and thresholds here. Version 2 fills the cells; the sentences that cite them stay as written.
{% endhint %}

Chapters cite rows by ID. A Route can be described, bonded, executed and landed without any row being known; what changes once it is known is scale, not shape.

## Badges in this table

| Badge | Meaning here |
|---|---|
| `Open` | No value chosen. The citing chapter describes the mechanism and the range it must hold under. |
| `Design Target` | A value the current design assumes; it may change before Version 2 without changing the mechanism. |
| `Roadmap` | Beside a parameter whose capability is described but not built; the value is not yet meaningful to fix. |

**Owner** is a role, not a person. **Expected** is a version, not a date: `v2` is the next release; `later` follows it.

## Token base

| ID | Parameter | Referenced in | Status | Owner | Expected |
|---|---|---|---|---|---|
| OP-01 | XO supply | [Distribution & Emission](../05-tokenomics/distribution.md) | `Open` | Tokenomics working group | v2 |
| OP-02 | XO allocation | [Distribution & Emission](../05-tokenomics/distribution.md) | `Open` | Tokenomics working group | v2 |
| OP-03 | XO vesting | [Distribution & Emission](../05-tokenomics/distribution.md) | `Open` | Tokenomics working group | v2 |
| OP-04 | EXON issuance policy | [Distribution & Emission](../05-tokenomics/distribution.md) · [EXON](../05-tokenomics/exon.md) | `Open` | Tokenomics working group | v2 |
| OP-05 | EXON emission | [Distribution & Emission](../05-tokenomics/distribution.md) | `Open` | Tokenomics working group | v2 |
| OP-06 | XO↔EXON relationship | [Distribution & Emission](../05-tokenomics/distribution.md) · [Value Flows](../05-tokenomics/value-flows.md) | `Open` | Tokenomics working group | v2 |

## Bond mechanics

| ID | Parameter | Referenced in | Status | Owner | Expected |
|---|---|---|---|---|---|
| OP-07 | Capacity function | [Trust & Bonding](../03-architecture/trust-and-bonding.md) · [XO](../05-tokenomics/xo.md) | `Open` | Protocol design | v2 |
| OP-08 | Unbond cooldown (linear Capacity decay) | [Trust & Bonding](../03-architecture/trust-and-bonding.md) · [XO](../05-tokenomics/xo.md) | `Design Target` | Protocol design | v2 |
| OP-09 | Seat thresholds | [Trust & Bonding](../03-architecture/trust-and-bonding.md) · [Governance](../06-governance/README.md) | `Open` | Protocol design | v2 |
| OP-10 | Bond recourse | [Trust & Bonding](../03-architecture/trust-and-bonding.md) · [Value Flows](../05-tokenomics/value-flows.md) | `Open` | Protocol design | v2 |
| OP-31 | Migration of custodial Bond records (NEX) to the on-chain Bond ledger | [Trust & Bonding](../03-architecture/trust-and-bonding.md) · [XO](../05-tokenomics/xo.md) · [Compliance](../08-compliance/README.md) | `Open` | Protocol design | v2 |

## Rail economics

| ID | Parameter | Referenced in | Status | Owner | Expected |
|---|---|---|---|---|---|
| OP-11 | EXON fee split | [Value Flows](../05-tokenomics/value-flows.md) | `Open` | Tokenomics working group | v2 |
| OP-12 | Rebate schedule | [EXON](../05-tokenomics/exon.md) · [PayFi](../04-product-stack/payfi.md) | `Open` | Tokenomics working group | v2 |
| OP-12b | Protocol-level EXON flow vs Bond pool | [Value Flows](../05-tokenomics/value-flows.md) | `Open` | Tokenomics working group | v2 |
| OP-13 | Burn Rate per leg type | [EXON](../05-tokenomics/exon.md) · [Settlement & Custody](../03-architecture/settlement-and-custody.md) | `Open` | Tokenomics working group | v2 |

## Deployment

| ID | Parameter | Referenced in | Status | Owner | Expected |
|---|---|---|---|---|---|
| OP-14 | Initial contract chain — decided: BNB Smart Chain (BSC) | [Protocol Architecture](../03-architecture/README.md) · [Settlement & Custody](../03-architecture/settlement-and-custody.md) | `In development` | Protocol design | — |
| OP-15 | Leg executors and venues | [Settlement & Custody](../03-architecture/settlement-and-custody.md) · [Marketplace](../04-product-stack/marketplace.md) | `Open` | Product | later |
| OP-16 | Oracle providers | [Data & Oracles](../03-architecture/data-and-oracles.md) | `Open` | Protocol design | later |
| OP-17 | Circuit-breaker thresholds | [Data & Oracles](../03-architecture/data-and-oracles.md) | `Design Target` | Protocol design | v2 |
| OP-18 | Pre-approved envelope limits `Roadmap` | [Agent Runtime](../03-architecture/agent-runtime.md) · [PayFi](../04-product-stack/payfi.md) | `Open` | Product | later |

## Governance

| ID | Parameter | Referenced in | Status | Owner | Expected |
|---|---|---|---|---|---|
| OP-19 | Time-locks and voting periods | [Governance](../06-governance/README.md) | `Design Target` | Protocol design | v2 |
| OP-20 | Seat Council composition | [Governance](../06-governance/README.md) · [Data & Oracles](../03-architecture/data-and-oracles.md) | `Open` | Protocol design | v2 |

## Compliance

| ID | Parameter | Referenced in | Status | Owner | Expected |
|---|---|---|---|---|---|
| OP-21 | Jurisdictions | [Compliance](../08-compliance/README.md) · [Legal Disclaimer](../legal-disclaimer/README.md) | `Open` | Legal counsel | v2 |
| OP-22 | KYC providers | [Data & Oracles](../03-architecture/data-and-oracles.md) · [Compliance](../08-compliance/README.md) | `Open` | Legal counsel | later |
| OP-23 | Early participation round terms | [EXON](../05-tokenomics/exon.md) · [Compliance](../08-compliance/README.md) | `Open` | Legal counsel | v2 |
| OP-24 | Equity-linked settlement partner `Roadmap` | [Intent, Not Operation](../02-the-translator/intent-over-operation.md) · [Compliance](../08-compliance/README.md) | `Open` | Legal counsel | later |
| OP-25 | Card issuer `Roadmap` | [Stablecoin Card](../04-product-stack/stablecoin-card.md) · [Compliance](../08-compliance/README.md) | `Open` | Legal counsel | later |
| OP-26 | Foresight infrastructure scope `Roadmap` | [Wallet](../04-product-stack/wallet.md) · [Compliance](../08-compliance/README.md) | `Open` | Product | later |
| OP-27 | Patience yield sources `Roadmap` | [Wallet](../04-product-stack/wallet.md) · [Compliance](../08-compliance/README.md) | `Open` | Product | later |

## Assurance

| ID | Parameter | Referenced in | Status | Owner | Expected |
|---|---|---|---|---|---|
| OP-28 | Audit scope | [Security & Risk](../07-security-and-risk/README.md) | `Open` | Protocol design | v2 |
| OP-29 | Capability status confirmation | [The NEXON Stack](../04-product-stack/README.md) · [Roadmap](../09-roadmap/README.md) | `Open` | Product | v2 |
| OP-30 | Contributor disclosure | [Compliance](../08-compliance/README.md) · [Legal Disclaimer](../legal-disclaimer/README.md) | `Open` | Legal counsel | v2 |

{% hint style="info" %}
**Scope of this section.** Commits to: these rows are the complete set of values Version 1 leaves open; Version 2 fills them without rewriting chapters. Does not commit to: any value, party, chain or date. Open items: this table.
{% endhint %}

*Spine: [The Translator](../02-the-translator/README.md)*
