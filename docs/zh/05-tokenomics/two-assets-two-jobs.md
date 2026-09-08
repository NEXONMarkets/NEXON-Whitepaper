---
description: "XO 承载长期价值，EXON 驱动流通；两者当前的机制角色各自独立、边界精确。"
icon: arrows-split-up-and-left
---

# 双币，两份工作

NEXON 用两种资产，是因为**价值沉淀和活跃流通不是同一份工作**。

**XO 是价值锚。EXON 是流通引擎。** 在这条叙事之下，定稿机制又给每种资产一个更窄、可实现、可审计的当前功能。

## 完整角色表 <a href="#the-complete-role-map" id="the-complete-role-map"></a>

| 维度 | XO | EXON |
|---|---|---|
| 名字怎么来的 | `X` 跨域连接与可能性；`O` 生态闭环与价值沉淀 | `EX` exchange / experience；`ON` 流通开启 |
| 叙事角色 | 价值锚 | 流通引擎 |
| 叙事功能 | 质押、参与、生态权益与长期价值沉淀 | 交易、支付、兑换、费用与消费流通 |
| 当前正式名称 | 质押本金代币 | 核心价值代币 |
| 当前获取方式 | 向 Treasury 申购，协议统一管理 U 价 | 早期轮、7228 自动建仓、二级市场买入 |
| 当前市场 | 体系内流转，协议定价 | TGE 起在 NEX 主交易所公开现货流通 |
| 当前机制作用 | 承载 72% 的质押与收益 / PV 基数 | 承接程序化买入、余额校验、线性释放与赎回销毁 |
| 长期边界 | 治理与更广权益等待设计发布 | 支付、费用与消费用途等待具体产品支持与条款 |

`U` 是定稿文件里与 USDT 锚定的计价单位。XO 由协议管理的价格与体系内流转，跟 EXON 的公开二级市场价格是**刻意分开**的两件事。

## 为什么非分开不可 <a href="#why-the-split-is-not-optional" id="why-the-split-is-not-optional"></a>

如果把质押本金和流通资产当成同一份工作，两件事会立刻糊掉：一次**市场价格波动**会被误读成**计息基数变化**；一笔**产品费用**会被误读成**质押燃料校验**。

双币结构把四个问题保持独立：

{% stepper %}
{% step %}
### 什么金额建立收益基数？

`S = 0.72 × P`，由 XO 承载。
{% endstep %}

{% step %}
### 哪种资产暴露在公开价格与流动性之下？

EXON，从 TGE 起在现货市场流通。
{% endstep %}

{% step %}
### 开单资格要求账户里有什么？

等值 `F = 0.28 × P` 的 EXON，**被校验，仍归用户**。
{% endstep %}

{% step %}
### 选更快赎回时，销毁的是什么？

等值 EXON 被永久销毁——T+0 档 30%，30D 档 15%。
{% endstep %}
{% endstepper %}

四个问题，四个不同的答案。任何一次表述都不应该把它们中的任意两个合并。

## 叙事不是算术 <a href="#narrative-is-not-arithmetic" id="narrative-is-not-arithmetic"></a>

叫 XO「价值锚」，是为了让它不被读成一笔可有可无的记账条目——它把质押参与和长期生态命题连起来。这不改变它当前的确定功能：**协议定价的质押本金**。

叫 EXON「流通引擎」，解释的是为什么这种资产能随时间把数字与现实的活动连起来。这不会让它现在就变成通用支付或费用代币。它今天被确认的操作是：现货、释放、28% 的 Treasury 买入、用户余额校验、等值赎回销毁。

## 对外表述必须守住的边界 <a href="#boundaries-that-public-copy-has-to-hold" id="boundaries-that-public-copy-has-to-hold"></a>

<table><thead><tr><th width="60">#</th><th>边界</th></tr></thead><tbody><tr><td>1</td><td>XO 不是 NEX 官方平台币，也不是股权、债权或收益索取权</td></tr><tr><td>2</td><td>EXON 是 NEXON 的项目资产，不是 NEX 平台币</td></tr><tr><td>3</td><td>进 Treasury 的 28% <code>B</code> 与用户账户里被校验的 28% <code>F</code>，<strong>不是同一笔余额</strong></td></tr><tr><td>4</td><td>EXON 的赎回销毁是永久销毁，不是转给某个运营方</td></tr><tr><td>5</td><td>持有任何一种资产，都不授权 AI、PayFi、钱包或别的用户动这个账户</td></tr><tr><td>6</td><td>长期代币用途需要一个受支持的产品、已发布的规则、资格与一个能问责的运营方</td></tr></tbody></table>

## 一句对外的话 <a href="#one-sentence-for-external-use" id="one-sentence-for-external-use"></a>

> **NEXON 是生态，由 XO 承载价值，通过 EXON 激活流通。**

讨论当前机制时，把更窄的那句补上：**XO 是质押本金代币；EXON 是核心价值代币与公开现货 / 释放 / 买入 / 校验 / 销毁资产。** 两句一起说，叙事和事实源就都护住了。

*上一节：[通证经济](README.md) · 下一节：[XO —— 价值锚](xo.md)*
