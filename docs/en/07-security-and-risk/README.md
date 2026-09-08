---
description: "Principal, market, parameter, custody, contract, operational and disclosure risks in the current NEXON model."
icon: "shield"
---

# Security & Risk

The current model exposes participants to several independent risks:

- **Principal risk.** The 30-day early-exit rule deducts 10%–15% of the staking base; other losses may also occur.
- **Market and liquidity risk.** EXON may fall in price, lack buyers or trade with material slippage.
- **Parameter risk.** Base APY, weights, payout ratio and future-round terms may change where the model allows adjustment.
- **Release pressure.** A fixed supply does not prevent selling pressure as vested EXON reaches spot accounts.
- **Custody and counterparty risk.** Exchanges, Treasury operations, contracts and service providers may fail or become unavailable.
- **Technical risk.** Bugs, incorrect price inputs, accounting errors or compromised credentials can cause loss.
- **Legal risk.** Availability and token treatment vary by jurisdiction.
- **Disclosure risk.** A conditional ROI or payback calculation may be mistaken for an expected outcome.

Controls should include parameter versioning, role-separated approvals, balance reconciliation, source-code review, contract audits, monitoring, incident response and public change notices. These controls reduce risk; they do not eliminate it.

{% hint style="danger" %}
Programmatic EXON purchases, locks and burns do not create a price floor or protect principal. Participants may lose some or all principal.
{% endhint %}

*Next: [Compliance](../08-compliance/README.md)*
