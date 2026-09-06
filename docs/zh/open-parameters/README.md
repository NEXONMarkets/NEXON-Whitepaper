---
description: "本文留白的每一个参数，汇成一张表：它是什么、在哪里被引用、状态如何、由哪个角色负责、预计何时给出。"
icon: "list-check"
layout:
  width: wide
---

# 待定参数汇总

{% hint style="info" %}
**v2 填格子，不重写章节。** 每一章都把机制讲完整，把数字、名称与阈值留在这里。第二版填入这些格子；引用它们的句子一字不改。
{% endhint %}

各章按 ID 引用本表的行。一条 Route（路径）可以在任何一行都未知的情况下被描述、被押住（Bond）、被执行、被落地；这些值一旦确定，改变的是规模，不是形状。

## 本表中的徽章 <a href="#badges-in-this-table" id="badges-in-this-table"></a>

| 徽章 | 在本表中的含义 |
|---|---|
| `Open` | 尚未选定取值。引用它的章节描述了机制，以及该值必须落在其中的范围。 |
| `Design Target` | 当前设计假定的取值；第二版之前可能变更，机制不变。 |
| `Roadmap` | 标在某个参数旁，表示其对应能力已描述但未建成；此时固定取值尚无意义。 |

**负责角色**是角色，不是人。**预期**是版本，不是日期：`v2` 是下一版；`之后` 指 v2 以后。

## 代币基础 <a href="#token-base" id="token-base"></a>

| ID | 参数 | 引用章节 | 状态 | 负责角色 | 预期 |
|---|---|---|---|---|---|
| OP-01 | XO 总量（supply） | [分配与释放](../05-tokenomics/distribution.md) | `Open` | 代币经济工作组 | v2 |
| OP-02 | XO 分配（allocation） | [分配与释放](../05-tokenomics/distribution.md) | `Open` | 代币经济工作组 | v2 |
| OP-03 | XO 解锁（vesting） | [分配与释放](../05-tokenomics/distribution.md) | `Open` | 代币经济工作组 | v2 |
| OP-04 | EXON 发行政策（issuance policy） | [分配与释放](../05-tokenomics/distribution.md) · [EXON](../05-tokenomics/exon.md) | `Open` | 代币经济工作组 | v2 |
| OP-05 | EXON 释放（emission） | [分配与释放](../05-tokenomics/distribution.md) | `Open` | 代币经济工作组 | v2 |
| OP-06 | XO↔EXON 关系 | [分配与释放](../05-tokenomics/distribution.md) · [价值流转](../05-tokenomics/value-flows.md) | `Open` | 代币经济工作组 | v2 |

## Bond 机制 <a href="#bond-mechanics" id="bond-mechanics"></a>

| ID | 参数 | 引用章节 | 状态 | 负责角色 | 预期 |
|---|---|---|---|---|---|
| OP-07 | Capacity（执行额度）函数 | [信任与抵押](../03-architecture/trust-and-bonding.md) · [XO](../05-tokenomics/xo.md) | `Open` | 协议设计 | v2 |
| OP-08 | Unbond 冷却期（Capacity 线性衰减） | [信任与抵押](../03-architecture/trust-and-bonding.md) · [XO](../05-tokenomics/xo.md) | `Design Target` | 协议设计 | v2 |
| OP-09 | Seat（席位）门槛 | [信任与抵押](../03-architecture/trust-and-bonding.md) · [治理](../06-governance/README.md) | `Open` | 协议设计 | v2 |
| OP-10 | Bond 追偿（Bond recourse） | [信任与抵押](../03-architecture/trust-and-bonding.md) · [价值流转](../05-tokenomics/value-flows.md) | `Open` | 协议设计 | v2 |
| OP-31 | NEX 托管型 Bond 记录向链上 Bond 账本的迁移 | [信任与抵押](../03-architecture/trust-and-bonding.md) · [XO](../05-tokenomics/xo.md) · [合规立场](../08-compliance/README.md) | `Open` | 协议设计 | v2 |

## 结算轨经济 <a href="#rail-economics" id="rail-economics"></a>

| ID | 参数 | 引用章节 | 状态 | 负责角色 | 预期 |
|---|---|---|---|---|---|
| OP-11 | EXON 手续费分配（fee split） | [价值流转](../05-tokenomics/value-flows.md) | `Open` | 代币经济工作组 | v2 |
| OP-12 | Rebate（抵扣）计划表（schedule） | [EXON](../05-tokenomics/exon.md) · [PayFi](../04-product-stack/payfi.md) | `Open` | 代币经济工作组 | v2 |
| OP-12b | 协议层 EXON 流是否触及 Bond 池 | [价值流转](../05-tokenomics/value-flows.md) | `Open` | 代币经济工作组 | v2 |
| OP-13 | 各类腿的 Burn Rate（消耗） | [EXON](../05-tokenomics/exon.md) · [结算与托管](../03-architecture/settlement-and-custody.md) | `Open` | 代币经济工作组 | v2 |

## 部署 <a href="#deployment" id="deployment"></a>

| ID | 参数 | 引用章节 | 状态 | 负责角色 | 预期 |
|---|---|---|---|---|---|
| OP-14 | 首发合约链——已定：BNB Smart Chain（BSC） | [协议架构](../03-architecture/README.md) · [结算与托管](../03-architecture/settlement-and-custody.md) | `In development` | 协议设计 | — |
| OP-15 | 腿执行方与交易场所（Leg Executors / venues） | [结算与托管](../03-architecture/settlement-and-custody.md) · [商城](../04-product-stack/marketplace.md) | `Open` | 产品 | 之后 |
| OP-16 | 预言机供应商（Oracle providers） | [数据与预言机](../03-architecture/data-and-oracles.md) | `Open` | 协议设计 | 之后 |
| OP-17 | 熔断阈值（Circuit-breaker thresholds） | [数据与预言机](../03-architecture/data-and-oracles.md) | `Design Target` | 协议设计 | v2 |
| OP-18 | 预授权额度包（Pre-approved envelope）限额 `Roadmap` | [Agent 运行时](../03-architecture/agent-runtime.md) · [PayFi](../04-product-stack/payfi.md) | `Open` | 产品 | 之后 |

## 治理 <a href="#governance" id="governance"></a>

| ID | 参数 | 引用章节 | 状态 | 负责角色 | 预期 |
|---|---|---|---|---|---|
| OP-19 | 时间锁与投票期（Time-locks / voting periods） | [治理](../06-governance/README.md) | `Design Target` | 协议设计 | v2 |
| OP-20 | Seat Council（席位议会）组成 | [治理](../06-governance/README.md) · [数据与预言机](../03-architecture/data-and-oracles.md) | `Open` | 协议设计 | v2 |

## 合规 <a href="#compliance" id="compliance"></a>

| ID | 参数 | 引用章节 | 状态 | 负责角色 | 预期 |
|---|---|---|---|---|---|
| OP-21 | 辖区（Jurisdictions） | [合规立场](../08-compliance/README.md) · [法律声明](../legal-disclaimer/README.md) | `Open` | 法务 | v2 |
| OP-22 | KYC 供应商 | [数据与预言机](../03-architecture/data-and-oracles.md) · [合规立场](../08-compliance/README.md) | `Open` | 法务 | 之后 |
| OP-23 | 早期参与轮条款（Early participation round terms） | [EXON](../05-tokenomics/exon.md) · [合规立场](../08-compliance/README.md) | `Open` | 法务 | v2 |
| OP-24 | 股权挂钩结算合作方（Equity-linked settlement partner）`Roadmap` | [表达意图，而非操作产品](../02-the-translator/intent-over-operation.md) · [合规立场](../08-compliance/README.md) | `Open` | 法务 | 之后 |
| OP-25 | 发卡机构（Card issuer）`Roadmap` | [稳定币卡](../04-product-stack/stablecoin-card.md) · [合规立场](../08-compliance/README.md) | `Open` | 法务 | 之后 |
| OP-26 | Foresight（前瞻）基建范围 `Roadmap` | [钱包](../04-product-stack/wallet.md) · [合规立场](../08-compliance/README.md) | `Open` | 产品 | 之后 |
| OP-27 | Patience（耐心）收益来源 `Roadmap` | [钱包](../04-product-stack/wallet.md) · [合规立场](../08-compliance/README.md) | `Open` | 产品 | 之后 |

## 保障 <a href="#assurance" id="assurance"></a>

| ID | 参数 | 引用章节 | 状态 | 负责角色 | 预期 |
|---|---|---|---|---|---|
| OP-28 | 审计范围（Audit scope） | [安全与风险](../07-security-and-risk/README.md) | `Open` | 协议设计 | v2 |
| OP-29 | 能力状态确认（Capability status confirmation） | [NEXON 产品栈](../04-product-stack/README.md) · [路线图](../09-roadmap/README.md) | `Open` | 产品 | v2 |
| OP-30 | 贡献者披露（Contributor disclosure） | [合规立场](../08-compliance/README.md) · [法律声明](../legal-disclaimer/README.md) | `Open` | 法务 | v2 |

{% hint style="info" %}
**本节口径。** 本节承诺：这些行是第一版留白取值的完整集合；第二版填入它们，不重写章节。本节不承诺：任何取值、参与方、链或日期。待定项：本表。
{% endhint %}

*主轴：[译者](../02-the-translator/README.md)*
