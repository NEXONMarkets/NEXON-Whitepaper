---
description: "项目方定稿的 NEXON 经济：双币叙事角色，原封不动地映射到 7228、释放、收益与赎回机制上。"
icon: coins
---

# 通证经济

> NEXON 是生态，XO 承载价值，EXON 驱动流通。

这一部分实现的是项目方 2026 年 9 月 6 日定稿的经济模型，并把叙事定位——XO 是**价值锚**、EXON 是**流通引擎**——映射到这套模型上，**不改动它的任何一处算术**。

## 每种资产读三层 <a href="#read-each-asset-on-three-levels" id="read-each-asset-on-three-levels"></a>

| 层级 | XO | EXON |
|---|---|---|
| **叙事** | 价值锚：参与、质押、权益与长期价值沉淀 | 流通引擎：连接数字金融、交易所、支付、费用与消费 |
| **当前机制** | 以 U 计价的质押本金代币，用在 Staking Platform 内 | 核心价值代币，公开现货 / 释放 / 买入 / 校验 / 销毁资产 |
| **长期方向** | 更广的生态权益与治理，等待规则发布 | 支付、兑换、费用与消费用途，等待产品条款发布 |

叙事说的是每种资产**打算**为生态贡献什么，机制说的是它**现在**在做什么。这两句话都要说，顺序不要颠倒。

## 一个账户，两个运营层 <a href="#one-account-two-operating-layers" id="one-account-two-operating-layers"></a>

**NEX Main Exchange / CEX** 是现货层，承载 EXON 交易、IEO 与释放呈现。独立的 **Staking Platform** 处理单币质押、期限权重、动态奖励与赎回。它们可以共享账户体系和资金后台；质押参数不会变成交易所的现货规则，交易所也不发放这里所说的质押奖励。

每一笔合格本金 `P` 走同一条 7228 路径：

```text
B = 0.28 × P   → 按实时价买入 EXON → Treasury Liquidity
S = 0.72 × P   → XO 质押本金与收益 / PV 基数
B + S = P
F = 0.28 × P   → 等值 EXON 余额校验；仍归用户
```

{% hint style="info" %}
`B` 和 `F` 的 **U 价值相同，归属和作用完全不同**。`B` 是买入并注入 Treasury Liquidity 的 EXON；`F` 是在用户账户里被校验的余额，开单时不转走、不收费、不销毁。把这两笔混为一谈，是读这套机制最容易犯的错。
{% endhint %}

## 经济生命周期 <a href="#the-economic-lifecycle" id="the-economic-lifecycle"></a>

早期轮 EXON 从 TGE 起进入统一的 **1,095 天线性释放**，分 2,190 个 12 小时 Epoch 完成。XO 质押收益按 **200% 基础年化**参数、**1.00 – 1.50** 的期限权重、每天两个 Epoch 计算。30 天期限提前退出，从 72% 的质押基数中扣除 10% – 15%。

收益赎回有 T+0、30D、60D 三档，分别净释放 70%、85%、100%，并对应永久销毁等值的 30%、15%、0% EXON。动态奖励采用相邻等级的 Differential Matching Bonus，Reward Payout Ratio 区间 150% – 200%。

## 还没有公布的部分 <a href="#what-has-not-been-published" id="what-has-not-been-published"></a>

EXON 的数字总量、完整分配、初始流通量、后续轮次额度与折扣、最终日期，以及完整的动态奖励等级表，在定稿来源里没有给出。这些字段保持[待定](../open-parameters/README.md)状态，不由任何其他文件替它补齐。

## 这一部分包含 <a href="#in-this-part" id="in-this-part"></a>

<table data-view="cards"><thead><tr><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><strong>双币，两份工作</strong></td><td>为什么价值沉淀和活跃流通不能是同一份工作。</td><td><a href="two-assets-two-jobs.md">two-assets-two-jobs.md</a></td></tr><tr><td><strong>分配与释放</strong></td><td>早期档位、TGE 指导价、1,095 天线性释放。</td><td><a href="distribution.md">distribution.md</a></td></tr><tr><td><strong>质押与收益</strong></td><td>200% 基础年化、期限权重、续期阶梯与提前退出。</td><td><a href="staking-and-returns.md">staking-and-returns.md</a></td></tr><tr><td><strong>完整演算案例</strong></td><td>三个案例，把每一个数字连同它的假设一起摆出来。</td><td><a href="worked-examples.md">worked-examples.md</a></td></tr><tr><td><strong>价值流转</strong></td><td>六条流，各自记账，不合并成一个故事。</td><td><a href="value-flows.md">value-flows.md</a></td></tr><tr><td><strong>XO 与 EXON</strong></td><td>两种资产各自的名字、角色与当前机制。</td><td><a href="xo.md">xo.md</a></td></tr></tbody></table>

*下一节：[双币，两份工作](two-assets-two-jobs.md)*
