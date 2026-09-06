---
description: "NEXON 词汇表的二十个固定术语，按四层排列：英文、中文配对、定义、定义所在章节，另有本文新增的五个术语。"
icon: "book"
layout:
  width: wide
---

# 术语表

> 三个市场，一种语言。

{% hint style="info" %}
**中文配对固定；本文以英文版为准。** 下表每个术语只有一个中文配对，中文版不使用任何其他译法。两版措辞如有出入，以英文版为准——只有一处例外：有一小组句子先以中文写成（本文句库中的 S5、S6c 与 S22–S30，包括对两种资产的定性，以及「NEXON 的连接不是靠桥，是靠 Agent」这一句）。这几句以中文为准，英文是固定英译。
{% endhint %}

二十个术语撑起这份白皮书，按主轴的四层分组：Agent 把一个 Intent（意图）翻译成一条 Route（路径）时做了什么；围绕这个 Agent 的生态是什么；押住什么，Agent 才能行动；行动时又花掉什么。每个定义只在这里给一次。**见**一列指向在上下文里定义该术语的章节。

## Agent 层 <a href="#agent-layer" id="agent-layer"></a>

主轴本身的词汇：一句话与一个已结算的结果之间发生的事。

| EN | ZH | 定义 | 见 |
|---|---|---|---|
| Intent | 意图 | 用户用自然语言表达的目标，Agent 的输入单元 | [意图层](../03-architecture/intent-layer.md) |
| Nexus Agent | 连接体 | NEXON 的核心 Agent，负责跨市场翻译与执行 | [译者](../02-the-translator/README.md) · [Agent 运行时](../03-architecture/agent-runtime.md) |
| Parse | 解析 | 把一句自然语言变成结构化 Intent | [意图层](../03-architecture/intent-layer.md) |
| Route | 路径 | Agent 在三个市场间规划出的可执行路线 | [Agent 运行时](../03-architecture/agent-runtime.md) |
| Real Leg | 现实腿 | 一条 Route 里最后落到现实世界的那一段 | [商城](../04-product-stack/marketplace.md) · [结算与托管](../03-architecture/settlement-and-custody.md) |
| Rollback | 回滚 | 执行中任一段失败时的原路退回 | [结算与托管](../03-architecture/settlement-and-custody.md) |

## 生态层 <a href="#ecosystem-layer" id="ecosystem-layer"></a>

| EN | ZH | 定义 | 见 |
|---|---|---|---|
| The Three Markets | 三个市场 | 资本市场 / 数字资产 / 真实消费 | [三种价值语言](../01-the-split/three-value-languages.md) |
| Translation Layer | 翻译层 | NEXON 的核心定位——让 Agent 跨三个市场行动的应用层协议 | [译者](../02-the-translator/README.md) |
| Circle | 圈层 | 社交层的基本单位，意图的来源 | [社交](../04-product-stack/social.md) |
| Foresight | 前瞻 | 钱包内的去中心化观点市场，Agent 读取它作为判断信号；NEXON 只做基建与入口 `Roadmap` | [钱包](../04-product-stack/wallet.md) |
| Patience | 耐心 | 等待执行期间资产不闲置的链上收益（浮动 · 非承诺 · 非保本）`Roadmap` | [钱包](../04-product-stack/wallet.md) |
| Storefront | 落地端 | 商城与 Stablecoin Card 的统称 | [NEXON 产品栈](../04-product-stack/README.md) |

## XO —— 价值层 <a href="#xo-value-layer" id="xo-value-layer"></a>

只押不花。

| EN | ZH | 定义 | 见 |
|---|---|---|---|
| Bond | 押注 | 押住 XO 的动作 | [信任与抵押](../03-architecture/trust-and-bonding.md) |
| Capacity | 执行额度 | Bond 换来的、Agent 可替你执行的上限 | [信任与抵押](../03-architecture/trust-and-bonding.md) · [XO](../05-tokenomics/xo.md) |
| Seat | 席位 | 治理与生态权益的位次 | [治理](../06-governance/README.md) |
| Depth | 沉淀 | Bond 的时间长度 | [信任与抵押](../03-architecture/trust-and-bonding.md) · [XO](../05-tokenomics/xo.md) |

## EXON —— 流通层 <a href="#exon-circulation-layer" id="exon-circulation-layer"></a>

只花不押。

| EN | ZH | 定义 | 见 |
|---|---|---|---|
| Settlement Rail | 结算轨 | EXON 承载的跨市场结算通道 | [EXON](../05-tokenomics/exon.md) |
| Burn Rate | 消耗 | 一次 Intent 执行消耗的 EXON。是被消耗，不是被销毁 | [EXON](../05-tokenomics/exon.md) |
| Redemption | 兑换 | 股权挂钩结算 / 旅行兑换这类场景的统称 `Roadmap` | [EXON](../05-tokenomics/exon.md) |
| Rebate | 抵扣 | 手续费抵扣 | [EXON](../05-tokenomics/exon.md) · [PayFi](../04-product-stack/payfi.md) |

## 四层之外 <a href="#outside-the-four-layers" id="outside-the-four-layers"></a>

| EN | ZH | 定义 | 见 |
|---|---|---|---|
| NEX | NEX | 一家持牌数字资产交易所。NEXON 是在 NEX 生态内由社区自发发起的独立项目，不是 NEX 的官方产品；XO 与 EXON 都不是交易所平台币。 | [为什么叫 NEXON](../01-the-split/why-nexon.md) · [合规立场](../08-compliance/README.md) |

## 固定序列 <a href="#fixed-sequences" id="fixed-sequences"></a>

有两组序列是固定说法，永不调序。每个 Intent 的五步：**Parse → Route → Bond Check → Execute → Land the Real Leg**。三个市场：**资本市场 → 数字资产 → 真实消费**。

## 本文新增术语 <a href="#terms-introduced-by-this-paper" id="terms-introduced-by-this-paper"></a>

五个术语是词汇表的新成员。每一个都为架构、经济或治理章节需要命名的某个机制而设，每一个都落在四层之内。

| EN | ZH | 层 | 定义 | 见 | |
|---|---|---|---|---|---|
| Capacity Reservation | 额度冻结 | XO | 一条 Route 执行期间被冻结的那部分 Capacity，Route 关闭时释放 | [Agent 运行时](../03-architecture/agent-runtime.md) | `NEW` |
| Landing Receipt | 落地凭证 | Agent | 证明 Real Leg 已经落地的可验证记录 | [结算与托管](../03-architecture/settlement-and-custody.md) · [PayFi](../04-product-stack/payfi.md) | `NEW` |
| Seat Council | 席位议会 | XO | 由 Seat 持有者选出、有时限、持有暂停权的小组 | [治理](../06-governance/README.md) | `NEW` |
| Protocol Reserve | 协议储备 | EXON | 协议金库——EXON 经结算轨被花掉时的去向之一 | [价值流转](../05-tokenomics/value-flows.md) | `NEW` |
| Leg Executor | 腿执行方 | 生态 | 执行一条 Route 中某一腿的场所、持牌方或供应商 | [结算与托管](../03-architecture/settlement-and-custody.md) · [价值流转](../05-tokenomics/value-flows.md) | `NEW` |

{% hint style="info" %}
**本节口径。** 本节承诺：这二十个术语、它们的中文配对与定义，在本文两个版本中固定不变。本节不承诺：任何术语所指能力的状态；Foresight、Patience 与 Redemption 的徽章沿用描述它们的章节。待定项：[OP-29](../open-parameters/README.md)。
{% endhint %}

*主轴：[译者](../02-the-translator/README.md) · 下一节：[法律声明](../legal-disclaimer/README.md)*
