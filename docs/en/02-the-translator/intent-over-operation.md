---
description: "An intent is a bounded request for an outcome, not a blank cheque for an agent; every route stays inspectable, revocable and attributable."
icon: route
---

# Express Intent, Not Operations

Most financial software is organized around **operations**: pick a market, pick an asset, enter an amount, set an order type, move the proceeds, convert the currency, then open the next app and start over. The interface hands you every control and leaves you the entire plan.

An intent starts one level up. It describes the result you want, and the boundaries that must hold while it is pursued.

> "Leave that reserve alone, use only these balances, show me the total cost, and ask me before anything moves."

That is an intent. It is not "improvise with any account you can see."

Natural language makes it easier to say all of that in one breath, but the executable object has to be structured and testable. Before a route exists, an intent should be able to represent at least:

* the target outcome and amount;
* the assets and accounts that may be used;
* assets, venues or categories that must **never** be touched;
* a deadline and a route-expiry time;
* acceptable price movement, fees and execution limits;
* identity, geography and product-eligibility constraints;
* whether each leg is approved individually or covered by a narrow standing rule;
* what happens if price, inventory or eligibility changes.

**Ambiguity is not permission.** When a material field is missing, the correct move is to ask, narrow the route, or stop.

## One complete round trip

Take a concrete case: turn a defined digital-asset budget into a travel booking while a separate reserve stays untouched. The conversation can be simple. The controls underneath cannot be skipped.

{% tabs %}
{% tab title="1 · Intent" %}
The system records destination, dates, budget ceiling, excluded assets, reserve floor and approval preference — and keeps **soft preferences** ("close to the venue") apart from **hard constraints** ("the reserve does not go below this").

It also flags which parts of the request carry sensitive information and how long that information may be kept. Travel, finances and relationships are about as sensitive as data gets; the route needs the approved constraints, not the whole conversation that produced them.
{% endtab %}

{% tab title="2 · Route" %}
The runtime proposes candidate legs: an asset conversion, a supported payment method, a supplier reservation. Each is a separate leg, and they depend on each other.

If the conversion quote expires, the purchase leg cannot keep running on stale assumptions. If no supported route exists, the system says so — instead of inventing one that looks like it would work.
{% endtab %}

{% tab title="3 · Policy Check" %}
The route passes through four layers of rules, and a model's confidence score substitutes for none of them:

* **User policy** — personal limits, allowlists, reserve floors;
* **Product policy** — balances, order minimums, disclosed terms;
* **Venue policy** — account status and jurisdictional eligibility;
* **Supplier policy** — inventory and fulfillment conditions.

Where the Staking Platform is involved, the check follows the real mechanism: 28% buys EXON at 1 USDT each into the fuel wallet, and the rest is swapped into XO and staked. The interface cannot present the fuel purchase as a fee, nor the fuel wallet as a transferable balance.
{% endtab %}

{% tab title="4 · User Approval" %}
Approval is a decision object a person can actually read: what moves, the maximum amount, the destination, the executor, the expiry, the receipt to expect.

A confirmation button that reveals none of those is consent in form and control in name only.

Authority should be scoped to **the smallest thing that finishes the job**. A user can approve one transaction, a chain of dependent legs, or a standing rule with a hard amount and a hard clock. A new destination, a higher amount, a wider asset scope or a longer duration all require fresh approval.
{% endtab %}

{% tab title="5 · Execution" %}
Each leg is executed by the system responsible for it. The agent may prepare a transaction, compare quotes or call an approved interface — and never becomes the exchange, custodian, issuer or merchant by doing so.

State has to distinguish at least: proposed, approved, submitted, settled, fulfilled, failed, refunded. **"Processing" is not a permanent state.**
{% endtab %}

{% tab title="6 · Receipt" %}
The final record joins the route that was approved to what actually happened: identifiers, timestamps, prices and fees, permissions consumed, deviation from quote, who is responsible and who follows up.

For anything physical, **payment settlement** and **fulfillment** are recorded as two separate events.
{% endtab %}
{% endtabs %}

## Failure is part of the route

A serious intent system explains the failure path before it needs one.

| Failure | Safe default |
|---|---|
| Quote expires before approval | Re-price and ask again |
| Eligibility check fails | Stop that leg and name the rule that blocked it |
| Balance changes | Recalculate — **never** quietly substitute another asset |
| One leg settles, the next fails | Preserve the receipts and enter the disclosed refund, offset or dispute path |
| Supplier does not fulfill | Mark delivery failed even though payment settled, and escalate |
| Agent output conflicts with product rules | Product rules win; the instruction is refused |

Not every action can be rolled back. A settled trade may only be reversed by a new trade at a new price. A chain transfer may be irreversible. A merchant refund takes time. So the interface has to use precise words — cancel, revoke, refund, reverse, offset, retry — instead of promising a universal undo.

## Who owns what

| Party | Owns |
|---|---|
| **The user** | The objective, the bounded approval, and the disclosed market and principal risk |
| **The orchestration layer** | Parsing intent, building candidate routes, enforcing user policy, recording decisions |
| **The executing venue** | Its orders, settlement, custody and eligibility controls |
| **The Staking Platform** | Applying the published mechanism at its published version |
| **The merchant or supplier** | Inventory, delivery, cancellation and disputes |
| **Data and model providers** | Signals. Their output is evidence to weigh, not authority to obey |

This table is why NEXON describes a connection network rather than one omnipotent application. The experience can be unified; the division of responsibility cannot be left vague.

## Holding a token is not an authorization

XO is the Value Anchor and currently carries staking principal. EXON is the Circulation Engine and is currently the spot, release, purchase, check and burn asset. Holding either grants an agent no standing right to spend from an account, skip a policy check or execute a regulated transaction. **Authority comes from the user and the responsible executor — never from a balance.**

Intent is the better abstraction precisely because it still ends in visible operations. It hides repetitive navigation, not consequence. It removes manual translation, not the user's say.

*Previous: [The Value Translator](README.md) · Next: [Not "AI Plus Payments"](not-ai-plus-payments.md)*
