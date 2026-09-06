---
description: "Why one asset cannot both anchor trust and settle execution. The argument, the side-by-side comparison, and the sentences this paper will never contain."
icon: "scale-balanced"
layout:
  width: wide
---

# Two Assets, Two Jobs

> EXON is what gets spent. XO is what stays bonded.

"Why two?" is the sharpest question anyone asks about this network, and it deserves a structural answer rather than a marketing one. Here it is, in the form used wherever NEXON is described.

## The argument

Because they solve two problems that contradict each other. A network that lets agents move money on people's behalf needs a trust anchor that circulates as little as possible — whoever bonds more, whose agent may do more. It also needs a settlement unit that circulates as fast as possible — however many intents are executed in a day, that much is consumed. These two demands pull the same asset in opposite directions: one wants it to settle and stay, the other wants it to turn over. Make one asset do both and it does neither well — those who bond dare not spend, those who spend will not bond. So there are two, and each does one job. Collateral is not fuel.

Put the same argument in the order the five steps run. For an agent to move money for you, the network must first answer one question: on what grounds should it be trusted? The answer is a Bond. You bond XO, and the network gives you Capacity — the ceiling on what your agent may execute on your behalf. Bond more and your agent may do more, your voice in governance grows, and your standing in the ecosystem rises. **XO never takes part in any single transaction. It is the precondition for that transaction to happen at all.**

Every execution, meanwhile, consumes fuel, needs a unit of account, and has to clear across several systems. That is EXON's job.

**EXON is what gets spent. XO is what stays bonded.** Collateral is not fuel. That's why there are two.

The definition this paper uses from here on is three sentences long, and every later page can be checked against it:

**XO is bonded, never spent: it is the collateral that earns your agent its execution capacity, your governance weight and your standing in the ecosystem. EXON is spent, never bonded: it is the fuel and settlement unit of every executed intent. Collateral is not fuel — which is exactly why they cannot be one asset.**

## At a glance

{% columns %}
{% column %}
### XO

**One word** — Bonded

**Three words** — Built to keep

**What it is** — The trust collateral of the agent network

**What it does** — Bond · Capacity · Seat · standing in the ecosystem
{% endcolumn %}
{% column %}
### EXON

**One word** — Spent

**Three words** — Built to use

**What it is** — The agent's fuel and unit of settlement

**What it does** — Settlement · Redemption · Rebate · circulation
{% endcolumn %}
{% endcolumns %}

## Side by side

| Dimension | XO · primary asset · value layer | EXON · utility asset · circulation layer |
|---|---|---|
| In one line | The trust collateral of the agent network | The agent's fuel and unit of settlement |
| What you do | Bond | Spend |
| What you get | Capacity · governance weight · standing in the ecosystem | One executed Intent |
| Time profile | Long-term, settling; the longer bonded, the better placed | High-frequency, immediate, turning over |
| Source of value | How much trust collateral the network needs | How many Intents the network executes each day |
| Posture | Built to keep | Built to use |
| Analogy | Margin deposit / an exchange seat | Electricity bill / road toll |
| Where it lands | Bond · governance voting · tiered standing | early participation round (`Open`) · equity-linked settlement (`Roadmap`) · travel redemption (`Roadmap`) · fee Rebate |

Every entry in the last row is a capability with a status, and none is described in this paper as live. Any conversion mechanism between the two assets — whether one exists, its ratio, its direction — is an Open Parameter ([OP-06](../open-parameters/README.md)) and is not described here in any form.

## The test

Each asset page that follows describes one ledger without reference to the other. That is not a stylistic choice; it is how the separation is kept honest. Value Flows closes this Part with six invariants, and the sixth is a test you can run on any sentence in this paper, including the ones below.

<details>

<summary>Sentences you will not read in this paper</summary>

**XO side.**

| Not in this paper | Because |
|---|---|
| "Pay with XO", "buy with XO", "XO offsets fees" | XO enters no payment |
| "XO is the ecosystem's fuel", "XO is gas" | The fuel is EXON |
| "XO can be redeemed for travel or equities" | Every Redemption scenario belongs to EXON |
| XO described as "high-frequency" or "for everyday use" | XO is bonded, not circulated |

**EXON side.**

| Not in this paper | Because |
|---|---|
| "Bond EXON for governance" | Governance comes from XO alone |
| "EXON is a store of value", "EXON appreciates over the long term" | EXON is about turnover, not settling |
| "Keep EXON for ecosystem benefits" | Benefits come from the Bond in XO |
| EXON described as "scarce", "deflationary" or "one to keep" | Those words describe what EXON is not |

**Both.**

| Not in this paper | Because |
|---|---|
| Both assets in one sentence, comparing price or return | Each is described on its own terms, on its own page |
| Any conversion mechanism between the two before the token economics is final — whether they convert, at what ratio, in which direction | Open Parameter (OP-06) |

**The one-line test.** Swap "XO" for "EXON" in any sentence. If it still reads true, the sentence is wrong.

</details>

{% hint style="info" %}
**Scope of this section.** Commits to: two assets, two ledgers, one job each — collateral that is bonded and fuel that is spent. Does not commit to: any conversion mechanism, ratio or direction between them, or any figure for either. Open items: [OP-06 · OP-23](../open-parameters/README.md).
{% endhint %}

*Spine: [The Translator](../02-the-translator/README.md) · Next: [XO — Collateral, Not Fuel](xo.md)*
