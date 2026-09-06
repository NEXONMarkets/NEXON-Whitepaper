---
description: "What v1 discloses about supply, allocation, vesting and emission — the structure and the principles — and why the figures wait for v2."
icon: "table-list"
---

# Distribution & Emission

> NEXON is the ecosystem. XO carries value. EXON drives circulation.

{% hint style="warning" %}
**No figures in v1.** This page sets out what will be disclosed and under which principles. It contains no supply, allocation, vesting, emission or conversion figure. Every cell that will hold one is listed below as an Open Parameter, and v2 fills those cells without rewriting this page.
{% endhint %}

## Why the figures wait

The token economics are designed on the project side and are still being finalised. Until they are, this paper will not describe a conversion mechanism, a ratio or a direction between the two assets, and it will not describe a supply. A figure given too early, and later revised, damages one thing above all: the community's trust. The mechanism, by contrast, is settled enough to write down — which is why the other pages of this Part describe roles, flows and invariants in full, while this one describes a table with empty cells.

## What v2 will state

| Item | What the disclosure will contain | Open Parameter | Status |
|---|---|---|---|
| XO supply | Total supply, and whether it is fixed | [OP-01](../open-parameters/README.md) | `Open` |
| XO allocation | Allocation by category, with the purpose of each category | [OP-02](../open-parameters/README.md) | `Open` |
| XO vesting | Lock and release schedule, per category | [OP-03](../open-parameters/README.md) | `Open` |
| EXON issuance policy | How EXON enters circulation, and what anchors the amount | [OP-04](../open-parameters/README.md) | `Open` |
| EXON emission | The schedule, and how it tracks executed Intents | [OP-05](../open-parameters/README.md) | `Open` |
| Relationship between the assets | Whether the two relate, how, and in which direction | [OP-06](../open-parameters/README.md) | `Open` |

## Four principles the figures will follow

1. **XO is allocated to stay.** Allocation and vesting are designed for participants who bond and stay. No category is designed to turn over quickly, and no category is exempt from the Bond mechanics described on [XO's page](xo.md).
2. **EXON issuance is anchored to execution.** What enters circulation tracks Intents executed, not a calendar alone. A Rail that executes little needs little.
3. **Early participation allocations are locked by default and released linearly.** The terms of any early participation round are an Open Parameter ([OP-23](../open-parameters/README.md)); the default shape of its release is not. Locked, then linear.
4. **Disclosure is complete or it does not happen.** The full allocation table and the release curve are published together, in one version, with every category named and every schedule drawn. Partial figures are not published.

<details>

<summary>What v2 will add</summary>

- The allocation table by category — early participation, ecosystem and Leg Executor incentives, Protocol Reserve, contributors — each with its purpose and its vesting schedule.
- A release curve over time for each category, and the combined curve.
- The issuance policy and emission schedule for EXON, with the execution measure it is anchored to.
- The relationship between the two assets, if any, stated in one sentence for each direction.
- An allocation chart. This version deliberately contains none: a chart implies proportions, and there are no proportions to show yet.

</details>

{% hint style="info" %}
**Scope of this section.** Commits to: the structure of the disclosure and the four principles above. Does not commit to: any figure, schedule, ratio or date. Open items: [OP-01 · OP-02 · OP-03 · OP-04 · OP-05 · OP-06 · OP-23](../open-parameters/README.md).
{% endhint %}

*Spine: [The Translator](../02-the-translator/README.md) · Next: [Value Flows](value-flows.md)*
