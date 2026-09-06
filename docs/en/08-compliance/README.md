---
description: "NEXON routes; licensed parties execute. Asset characterization, jurisdiction and identity, and a plain disclosure of every licence-dependent capability."
icon: "scale-balanced"
---

# Compliance & Legal Posture

> XO and EXON are utility assets. XO is used to obtain agent execution capacity and governance standing; EXON is used for settlement and circulation. Neither represents equity, debt, or a right to the profits or distributions of any entity. A formal legal opinion will be issued as required.

A Translation Layer touches regulated activity by construction. A Route spans capital markets, digital assets and real-world spending, and at least one leg of almost any Route is executed by a party licensed to do so. The posture follows: NEXON routes, and licensed parties execute. This section states what the two assets are, where the protocol stands on jurisdiction and identity, and — capability by capability — who performs each activity whose legal treatment depends on who performs it.

## Characterization

The sentence above is the whole of it. XO is bonded to obtain Capacity and standing; EXON is spent to settle Routes. Neither is a share, a note, or a claim on any entity's revenue. Bonding XO gives your agent standing, and standing is not a dividend. Consuming EXON pays for execution, and a Rebate on fees is a discount, not a distribution.

A formal legal opinion on both assets will be issued as the processes ahead require. This paper is not that opinion, and until it exists nobody speaking for NEXON offers a personal view on legal characterization.

## Relationship to NEX

NEXON is an independent, community-initiated project built within the NEX ecosystem. It is not an official NEX product, and neither XO nor EXON is an exchange token. NEX is a licensed digital-asset exchange; NEXON draws on its resources and its standing, and at launch XO is bonded through a custodial product that NEX operates under its own terms ([Trust & Bonding](../03-architecture/trust-and-bonding.md)). NEX's licences, disclosures and product terms are NEX's own and are published by NEX. This paper does not restate them, and nothing in it is a statement by or on behalf of NEX.

## Jurisdiction and identity

The jurisdictional stance — where the protocol is offered and where it is not — is `Open` (OP-21). Until it is fixed, no jurisdiction is named here as served or excluded; once fixed, the list lives in the [Legal Disclaimer](../legal-disclaimer/README.md).

Identity follows the same pattern as every other regulated activity on the network: a licensed party performs it, and the protocol records that it was performed. Know-your-customer and anti-money-laundering checks are run by licensed identity providers who issue an attestation; the protocol stores a reference to that attestation and never the underlying documents. Legs that require identity — a capital-market leg through a licensed venue (`Roadmap`), a card limit through a licensed issuer (`Roadmap`) — are gated on the attestation being present and current. Providers, and the jurisdictions they cover, are `Open` (OP-22).

## Capabilities that depend on a licensed party

Seven capabilities in this paper are, or may be, regulated activities depending on jurisdiction and on who performs them. Each is disclosed in the same form, under one rule: the protocol supplies the Intent, the Route and the access; the regulated act is performed by a party licensed to perform it.

| Capability | Who executes | NEXON's role | Status |
|---|---|---|---|
| **Custodial XO bonding at launch** | NEX, under its own product terms | Reads the record at Bond Check; sets no reward and promises none | `In development` (OP-31) |
| **Early participation round** | The issuing entity, under terms disclosed once fixed | Publishes the terms; allocations are subject to lock-up and linear release ([Distribution & Emission](../05-tokenomics/distribution.md)) | `Open` (OP-23) |
| **Equity-linked settlement** | A licensed third party; NEXON never brokers securities and never holds the position | Routes the capital-market leg of an Intent to that party and records its confirmation | `Roadmap` (OP-24) |
| **Travel redemption** | Travel suppliers onboarded to the Marketplace as Leg Executors | Lands the Real Leg and issues the Landing Receipt; holds no inventory | `Roadmap` |
| **Stablecoin Card** | A licensed card issuer and a compliant aggregation channel | Access layer only: the Land step delivers a card limit; the protocol issues no card and holds no card funds | `Roadmap` (OP-25) |
| **Foresight** | Independent operators of the venues that produce the signal | Settlement and entry infrastructure only; the protocol operates no venue and makes no market | `Roadmap` (OP-26) |
| **Patience** | The on-chain yield sources the Wallet routes idle assets into | Routing during a waiting window only; the protocol sets no rate and promises none | `Roadmap` (OP-27) |

Two rows carry fixed wording wherever they appear in this paper. Patience is **on-chain yield — floating · not guaranteed · non-principal-protected** in every mention, because any shorter form reads as a deposit. Equity-linked settlement is always paired with **executed by a licensed third party; NEXON never brokers securities**, because any shorter form reads as brokerage.

## Filing is not launch

Every third-party process this paper refers to — an audit, a legal opinion, a licence, a venue's review — has two dates: the day it is filed and the day it concludes. This paper reports the first as a filing and the second when it exists, and never describes a filing as an outcome. Nothing in between is promised, and no date or counterparty is named ahead of the outcome. The Roadmap that follows is held to the same rule.

{% hint style="warning" %}
**Nothing here is legal advice.** This section describes the posture adopted for NEXON and the parties relied on. It is not an opinion on how any regulator will treat either asset or any capability above, and it does not substitute for counsel in your own jurisdiction. The formal legal opinion, once issued, supersedes this section wherever the two differ.
{% endhint %}

{% hint style="info" %}
**Scope of this section.** Commits to: utility characterization of both assets, licensed-party execution for every regulated activity, attestation-based identity with no document custody, and the table above as the complete list of licence-dependent capabilities in v1. Does not commit to: any jurisdiction, provider, partner, issuer or venue, or any legal outcome ahead of a formal opinion. Open items: [OP-21 · OP-22 · OP-23 · OP-24 · OP-25 · OP-26 · OP-27 · OP-31](../open-parameters/README.md).
{% endhint %}

*Spine: [The Translator](../02-the-translator/README.md) · Next: [Roadmap](../09-roadmap/README.md)*

*Turning what you mean into what gets settled.*
