---
description: "The distinct failure modes of the current staking mechanism and of each long-term product, and the control programme that answers them."
icon: shield
---

# Security & Risk

The systems NEXON connects **fail in different ways**. A unified experience can make a route easier to understand; it cannot remove market loss, technical failure, counterparty default, legal restriction or real-world non-performance. So risk is assessed **per asset, per product and per execution leg** — not as one blanket judgment about "the project."

## Risks in the current economic mechanism

| Risk | What it actually is |
|---|---|
| **Principal** | Day 31 is the only exit window of the 30-day term; missed, the order renews. Other failures can also impair principal or access |
| **Market and liquidity** | EXON can fall, lack buyers, or trade with material spread and slippage. Guide and early prices do not guarantee a later execution price |
| **Parameter** | The per-settlement range, term bonuses and leadership execution rates are set by market stage where the mechanism permits |
| **Release pressure** | Fixed supply does not prevent selling pressure: EXON keeps reaching spot accounts across 1,095 days |
| **Dual-asset dependency** | EXON price and fuel-wallet balance set how much a withdrawal burns and which settlement speed is available |
| **Dynamic rewards** | Referral rewards follow each downline's daily static output, so team size moves individual payouts directly; leadership rates are published as ranges |
| **Custody and counterparty** | Exchanges, fuel-wallet operations, contracts, account providers and service providers can fail, restrict access or become unavailable |
| **Technical and accounting** | Contract bugs, bad price inputs, reward-ledger errors, compromised credentials and faulty reconciliation can all cause loss |

## Risks in the long-term products

{% tabs %}
{% tab title="AI authorization" %}
A model can misread intent, hallucinate a capability, rely on stale data, or be manipulated by untrusted content.

Deterministic limits, simulation, scoped approval and revocation reduce the risk; they cannot make every route correct. **Submission, settlement and fulfillment stay separate throughout.**
{% endtab %}

{% tab title="Wallet and keys" %}
Lost credentials, malicious approvals, provider compromise and failed recovery can all cause permanent loss.

A unified wallet view **obscures different custody models** unless each balance and permission names the system that controls it.
{% endtab %}

{% tab title="Prediction markets" %}
Third-party decentralized prediction markets can be restricted, illiquid, manipulated, or resolved through disputed oracles.

**A market price is neither certainty nor advice.** NEXON names the independent operator, the resolution rules and the jurisdiction rather than implying control.
{% endtab %}

{% tab title="Marketplace and delivery" %}
Merchants and travel suppliers can change inventory, cancel, fail to deliver or dispute a refund.

**Payment settlement is not proof of fulfillment.** Consumer rights and recovery depend on supplier and payment terms.
{% endtab %}

{% tab title="Stablecoin Card" %}
Issuer, network, merchant and custodian failures can cause declines, freezes, conversion loss or delayed refunds.

Availability and protections vary by jurisdiction.
{% endtab %}

{% tab title="Social content" %}
Impersonation, promotion, coordinated manipulation and selective performance claims all shape user judgment.

**Social context never authorizes a financial action, and popularity does not establish suitability.**
{% endtab %}
{% endtabs %}

## Cross-jurisdiction and legal risk

Token, staking, payment, prediction-market, card, data and promotion rules differ across jurisdictions and change over time. **A product can be technically available and legally unavailable to a particular user.** Licensed status in one operating domain does not automatically cover another.

## The control programme

<table><thead><tr><th width="220">Category</th><th>Controls</th></tr></thead><tbody><tr><td><strong>Change management</strong></td><td>Parameter versioning, role-separated approvals, published change notices</td></tr><tr><td><strong>Access</strong></td><td>Least privilege, permission review, credential rotation</td></tr><tr><td><strong>Code and contracts</strong></td><td>Code review, contract audit, external security testing</td></tr><tr><td><strong>Data</strong></td><td>Price-source cross-checks, balance reconciliation, monitoring and alerting</td></tr><tr><td><strong>Operations</strong></td><td>Incident response, backup and recovery, provider diligence</td></tr><tr><td><strong>AI-specific</strong></td><td>Threat models for prompt injection and malicious content, duplicate-execution protection, privacy minimization</td></tr><tr><td><strong>Honesty</strong></td><td>An honest "unknown" state whenever native systems cannot be reconciled</td></tr></tbody></table>

These controls reduce **specific** risks. They do not create principal protection, guaranteed delivery or guaranteed recovery — stated here so the table above reads as an engineering checklist rather than as reassurance.

*Previous: [Governance](../06-governance/README.md) · Next: [Compliance & Legal Posture](../08-compliance/README.md)*
