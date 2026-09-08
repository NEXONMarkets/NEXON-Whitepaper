---
description: "A Roadmap card access layer that depends on a responsible licensed issuer/operator and separately disclosed funding and fee terms."
icon: "credit-card"
---

# Stablecoin Card

**Status** · `Roadmap`

The Stablecoin Card is a planned bridge from eligible digital value to everyday merchant acceptance. It can extend the NEXON value loop beyond integrated marketplace inventory, but it cannot be treated as available until a responsible licensed issuer or operator, supported jurisdictions and product terms are formally published.

## Responsibility before branding

A card is not issued by an interface. The responsible issuer/operator would determine eligibility, KYC/AML requirements, accepted funding assets, conversion, custody, authorization, settlement, fees, limits, refunds, disputes and cardholder protections. Card-network and merchant rules would also apply.

NEXON's Roadmap role is to integrate the user experience: prepare an eligible funding route, display the quote and costs, request bounded approval, show authorization status and reconcile the issuer receipt. It must keep the issuer visible rather than representing the agent as the approving financial institution.

## A typical target flow

1. The user selects a supported funding source and a spending amount.
2. PayFi checks product and jurisdiction eligibility, reserve policy and quote freshness.
3. The interface shows conversion, fees, limits, issuer and expiry.
4. The user approves the defined action.
5. The issuer/operator handles funding, card authorization and settlement under its terms.
6. The Wallet records financial settlement separately from any merchant refund or dispute.

Offline authorization, recurring merchant charges, tips, reversals and chargebacks require product-specific handling. They should not be forced into a generic blockchain-finality model.

## Token and economics boundary

The approved Tokenomics paper does not specify EXON as current card settlement fuel or XO as card collateral. EXON's payment and fee roles are Roadmap. If a future card supports EXON directly or uses it in a disclosed conversion path, that support must identify price source, liquidity, spread, fee, custody and refund treatment.

Card economics remain separate from Staking Platform rewards and EXON redemption burns. A card transaction does not earn the published staking APY merely because it appears in the same ecosystem, and a merchant refund is not governed by a redemption burn.

## Launch gates and risks

Necessary gates include a named authorized operator, contractual allocation of responsibility, jurisdiction coverage, supported funding assets, custody and safeguarding terms, fraud and sanctions controls, security review, clear fees, customer support and dispute procedures. No issuer, launch date, fee schedule or jurisdiction is committed in this paper.

{% hint style="danger" %}
Card access can be declined, limited, suspended or unavailable. Conversion creates price and liquidity risk. Issuer, custodian, network and merchant failures follow their own recovery processes; NEXON cannot guarantee acceptance or reimbursement.
{% endhint %}

*Previous: [Marketplace](marketplace.md) · Next: [Token Economics](../05-tokenomics/README.md)*
