---
description: "The twenty fixed terms of the NEXON vocabulary in four layers — English, Chinese pairing, definition, defining section — plus five terms this paper introduces."
icon: "book"
layout:
  width: wide
---

# Glossary

> Three markets. One language.

{% hint style="info" %}
**English is canonical; Chinese pairings are fixed.** Every term below has exactly one Chinese pairing, and the Chinese edition uses no other. Where the two editions differ in wording, the English text governs — with one exception. A small set of sentences was written in Chinese first (S5, S6c and S22–S30 in the paper's sentence register, including the characterisation of the two assets and the line that NEXON's connection runs on agents). For those, the Chinese text governs and the English is a fixed rendering.
{% endhint %}

Twenty terms carry this paper, grouped by the four layers of its spine: what the agent does when it translates an Intent into a Route, what the ecosystem around that agent is, what is bonded so that the agent may act, and what is spent when it does. Each definition is given once, here. The **See** column points to the section that defines the term in context.

## Agent layer

The vocabulary of the spine itself: what happens between a sentence and a settled outcome.

| EN | ZH | Definition | See |
|---|---|---|---|
| Intent | 意图 | The goal a user states in natural language; the agent's unit of input. | [Intent Layer](../03-architecture/intent-layer.md) |
| Nexus Agent | 连接体 | NEXON's core agent, responsible for translation and execution across markets. | [The Translator](../02-the-translator/README.md) · [Agent Runtime](../03-architecture/agent-runtime.md) |
| Parse | 解析 | Turning a natural-language sentence into a structured Intent. | [Intent Layer](../03-architecture/intent-layer.md) |
| Route | 路径 | The executable path an agent plans across the three markets. | [Agent Runtime](../03-architecture/agent-runtime.md) |
| Real Leg | 现实腿 | The last segment of a Route — the one that lands in the real world. | [Marketplace](../04-product-stack/marketplace.md) · [Settlement & Custody](../03-architecture/settlement-and-custody.md) |
| Rollback | 回滚 | Return along the original path when any leg fails during execution. | [Settlement & Custody](../03-architecture/settlement-and-custody.md) |

## Ecosystem layer

| EN | ZH | Definition | See |
|---|---|---|---|
| The Three Markets | 三个市场 | Capital markets / digital assets / real-world spending. | [Three Value Languages](../01-the-split/three-value-languages.md) |
| Translation Layer | 翻译层 | NEXON's core positioning: the application-layer protocol through which agents act across the three markets. | [The Translator](../02-the-translator/README.md) |
| Circle | 圈层 | The basic unit of the social layer; the source of intent. | [Social](../04-product-stack/social.md) |
| Foresight | 前瞻 | A decentralised market of views inside the wallet, read by the agent as a judgment signal. NEXON builds the infrastructure and the entry point only. `Roadmap` | [Wallet](../04-product-stack/wallet.md) |
| Patience | 耐心 | On-chain yield while an Intent waits to execute, so that assets do not sit idle — floating · not guaranteed · non-principal-protected. `Roadmap` | [Wallet](../04-product-stack/wallet.md) |
| Storefront | 落地端 | The collective name for the Marketplace and the Stablecoin Card. | [The NEXON Stack](../04-product-stack/README.md) |

## XO — value layer

Bonded, never spent.

| EN | ZH | Definition | See |
|---|---|---|---|
| Bond | 押注 | The act of bonding XO. | [Trust & Bonding](../03-architecture/trust-and-bonding.md) |
| Capacity | 执行额度 | The ceiling on what an agent may execute on your behalf, obtained through Bond. | [Trust & Bonding](../03-architecture/trust-and-bonding.md) · [XO](../05-tokenomics/xo.md) |
| Seat | 席位 | Standing in governance and in ecosystem entitlements. | [Governance](../06-governance/README.md) |
| Depth | 沉淀 | The length of time a Bond has been held. | [Trust & Bonding](../03-architecture/trust-and-bonding.md) · [XO](../05-tokenomics/xo.md) |

## EXON — circulation layer

Spent, never bonded.

| EN | ZH | Definition | See |
|---|---|---|---|
| Settlement Rail | 结算轨 | The cross-market settlement channel that EXON carries. | [EXON](../05-tokenomics/exon.md) |
| Burn Rate | 消耗 | The EXON one Intent's execution consumes as it settles, leg by leg. Consumed, not destroyed. | [EXON](../05-tokenomics/exon.md) |
| Redemption | 兑换 | The collective name for scenarios such as equity-linked settlement and travel redemption. `Roadmap` | [EXON](../05-tokenomics/exon.md) |
| Rebate | 抵扣 | Rebate on fees. | [EXON](../05-tokenomics/exon.md) · [PayFi](../04-product-stack/payfi.md) |

## Outside the four layers

| EN | ZH | Definition | See |
|---|---|---|---|
| NEX | NEX | A licensed digital-asset exchange. NEXON is an independent, community-initiated project within its ecosystem — not an official NEX product; neither XO nor EXON is an exchange token. | [Why NEXON](../01-the-split/why-nexon.md) · [Compliance](../08-compliance/README.md) |

## Fixed sequences

Two sequences are set phrases and are never reordered. The five steps of every Intent: **Parse → Route → Bond Check → Execute → Land the Real Leg**. The three markets: **capital markets → digital assets → real-world spending**.

## Terms introduced by this paper

Five terms are new to the vocabulary. Each names a mechanism the architecture, economics or governance chapters needed a word for, and each sits inside one of the four layers.

| EN | ZH | Layer | Definition | See | |
|---|---|---|---|---|---|
| Capacity Reservation | 额度冻结 | XO | The portion of Capacity frozen for the duration of a Route's execution and released when the Route closes. | [Agent Runtime](../03-architecture/agent-runtime.md) | `NEW` |
| Landing Receipt | 落地凭证 | Agent | The verifiable record that a Real Leg has landed. | [Settlement & Custody](../03-architecture/settlement-and-custody.md) · [PayFi](../04-product-stack/payfi.md) | `NEW` |
| Seat Council | 席位议会 | XO | A time-limited group elected by Seat holders, holding a pause power. | [Governance](../06-governance/README.md) | `NEW` |
| Protocol Reserve | 协议储备 | EXON | The protocol treasury — one destination of EXON as it is spent through the Settlement Rail. | [Value Flows](../05-tokenomics/value-flows.md) | `NEW` |
| Leg Executor | 腿执行方 | Ecosystem | The venue, licensed party or supplier that executes one leg of a Route. | [Settlement & Custody](../03-architecture/settlement-and-custody.md) · [Value Flows](../05-tokenomics/value-flows.md) | `NEW` |

{% hint style="info" %}
**Scope of this section.** Commits to: these twenty terms, their Chinese pairings and their definitions are fixed across both editions of this paper. Does not commit to: the status of any capability a term names; Foresight, Patience and Redemption carry their badges from the chapters that describe them. Open items: [OP-29](../open-parameters/README.md).
{% endhint %}

*Spine: [The Translator](../02-the-translator/README.md) · Next: [Legal Disclaimer](../legal-disclaimer/README.md)*
