---
description: "The Stablecoin Card extends eligible digital value into everyday merchant acceptance, resting on a licensed issuer/operator."
icon: credit-card
---

# Stablecoin Card

*Product stage · Roadmap*

The Stablecoin Card is a bridge from eligible digital value to **everyday merchant acceptance**. It extends the NEXON value loop past marketplace inventory — to the corner shop, the restaurant, any terminal that takes a card.

## An interface does not issue a card

A card is issued by an **issuer**. The licensed issuer/operator determines eligibility, KYC/AML requirements, accepted funding assets, conversion, custody, authorization, settlement, fees, limits, refunds, disputes and cardholder protections. Card-network and merchant rules apply on top.

NEXON's side of the work is joining up the experience: prepare an eligible funding route, show the quote and costs, request bounded approval, display authorization status, and reconcile the issuer's receipt. **The issuer has to stay visible** — never obscured behind an agent that looks like the approving financial institution.

## The target flow

{% stepper %}
{% step %}
### Choose a source and an amount

The user selects a supported funding source and a spending amount.
{% endstep %}

{% step %}
### Check

PayFi checks product and jurisdiction eligibility, reserve policy and quote freshness.
{% endstep %}

{% step %}
### Show

The interface shows conversion, fees, limits, issuer and expiry.
{% endstep %}

{% step %}
### Approve

The user approves the action as scoped.
{% endstep %}

{% step %}
### Execute

The issuer/operator handles funding, card authorization and settlement under its own terms.
{% endstep %}

{% step %}
### Reconcile

The Wallet records financial settlement **separately** from any merchant refund or dispute.
{% endstep %}
{% endstepper %}

Offline authorization, recurring merchant charges, tips, reversals and chargebacks each need product-specific handling. **None of them fits a generic blockchain-finality model.**

## Token and economics boundary

The approved Tokenomics does not designate EXON as current card settlement fuel, nor XO as card collateral. EXON's payment and fee roles belong to the long-term direction. If a future card supports EXON directly or uses it in a disclosed conversion path, that support must name the price source, liquidity, spread, fee, custody and refund treatment.

Card economics and Staking Platform rewards and EXON redemption burns **run on separate tracks**. A card transaction does not earn the staking APY because it shares an ecosystem, and a merchant refund is not governed by a redemption burn.

## What has to ship before launch

A named authorized operator, contractual allocation of responsibility, jurisdiction coverage, supported funding assets, custody and safeguarding terms, fraud and sanctions controls, security review, clear fees, customer support and dispute procedures. Issuer, dates, fee schedule and jurisdictions are [Open Parameters](../open-parameters/README.md) (OP-P05).

*Previous: [Marketplace](marketplace.md) · Next: [Token Economics](../05-tokenomics/README.md)*
