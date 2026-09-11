---
description: "NEXON 现行经济机制：双币角色，每 12 小时结算的 XO 质押，只进不出的 EXON 燃料钱包，提取即销毁，私募 0.1 U 上线 1.0 U。"
icon: coins
---

# 通证经济

> NEXON 是生态，XO 承载价值，EXON 驱动流通。

这一部分写的是 NEXON 现行的经济机制（2026 年 9 月 10 日定稿，9 月 11 日逐条确认），并把叙事定位——XO 是**价值锚**、EXON 是**流通引擎**——落到每一个数字上。

## 每种资产读三层 <a href="#read-each-asset-on-three-levels" id="read-each-asset-on-three-levels"></a>

| 层级 | XO | EXON |
|---|---|---|
| **叙事** | 价值锚：质押、参与、治理与长期价值沉淀 | 流通引擎：连接交易所、支付、兑换、费用与消费 |
| **当前机制** | 质押本金代币；静态收益、推广奖励、领导奖金一律以 XO 发放；在 NEX 二级市场自由交易 | 核心价值代币；私募 0.1 U 是唯一获取渠道，上线 1.0 U；只能卖、不能买；入金的 28% 买入存入燃料钱包，提取收益时销毁 |
| **随入口开放** | 治理规则与更广的生态权益（Roadmap） | 交易、支付、兑换与手续费随五个入口逐个接入（Roadmap） |

叙事说的是每种资产**为生态承担什么**，机制说的是它**今天怎么运转**。两句一起说。

## 一个账户，两个运营层 <a href="#one-account-two-operating-layers" id="one-account-two-operating-layers"></a>

**NEX 交易所**是现货层：XO 自由交易，EXON 只挂卖单、不挂买单，上线当日起呈现每日释放。**质押与奖励层（Staking Platform）**处理 XO 质押、每 12 小时结算、期限加成、推广奖励、领导奖金与收益提取。两层共用同一套账户与资金后台，一次开户、两层切换。

## 一笔入金怎么拆 <a href="#how-a-deposit-splits" id="how-a-deposit-splits"></a>

每一笔质押入金 `P` 开单即分成两份，系统自动完成：

```text
燃料  = 0.28 × P   → 按当时 1 U 等值买入 EXON → 燃料钱包（只能销毁）
质押  = 其余部分   → 兑换 XO → 进入质押，每 12 小时结算
```

<figure><img src="../.gitbook/assets/onepage-04-fuel-wallet.svg" alt="入金 1,000 U：28% 即 280 U，按 1 U 等值买入 280 枚 EXON 存入燃料钱包，只能销毁、不能转出、不能交易"><figcaption>入金 1,000 U：280 枚 EXON 进燃料钱包，其余兑换 XO 开始计息</figcaption></figure>

{% hint style="success" %}
**燃料钱包只进不出。** 里面的 EXON 不能转出、不能交易，只有一个去处：提取收益时销毁。质押越多，买入越多；提取越多，烧得越多。
{% endhint %}

## 经济生命周期 <a href="#the-economic-lifecycle" id="the-economic-lifecycle"></a>

**质押。** XO 质押每 12 小时结算一次，单次 0.3% – 1.0%，北京时间 08:00 / 20:00；质押 1,000 U，一天 6 – 20 U。期限 30 / 90 / 180 / 360 / 540 天，加成基础 / +10% / +20% / +30% / +50%，只看期限不看金额。30 天档第 31 天是退出窗口，本金加收益一起领，不收违约金；错过自动续期 90 → 180 → 360 → 540 天。

**提取。** 收益以 XO 到账，随时可提取。到账方式三选一：立即到账销毁 30%、30 天到账销毁 20%、60 天到账销毁 10%，销毁的是燃料钱包里等值的 EXON，永久退出流通。

**私募与释放。** EXON 总量 10 亿枚，私募只放 2 亿枚，按 0.1 U 认购，三档 1,000 / 5,000 / 10,000 U 共 11,500 份；认购与质押按 3:1 配置。上线 1.0 U，当日起 1,095 天逐日释放，每 12 小时到账一次，共 2,190 次。

**动态。** 推广奖励最多 20 代、合计 76%，按下级每日静态产出计算；领导奖金 V1 – V12 按等级极差发放，V10 – V12 分享全球 XO 入金 3% 的奖金池。全部以 XO 发放，与静态收益同一个周期结算，提取时同样销毁。

## 这一部分包含 <a href="#in-this-part" id="in-this-part"></a>

<table data-view="cards"><thead><tr><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><strong>双币，两份工作</strong></td><td>为什么价值沉淀和活跃流通不能是同一份工作。</td><td><a href="two-assets-two-jobs.md">two-assets-two-jobs.md</a></td></tr><tr><td><strong>分配与释放</strong></td><td>私募三档、3:1 配置、1.0 U 上线、1,095 天线性释放。</td><td><a href="distribution.md">distribution.md</a></td></tr><tr><td><strong>质押与收益</strong></td><td>每 12 小时 0.3% – 1.0%、期限加成、退出窗口、提取三档、20 代与 V1 – V12。</td><td><a href="staking-and-returns.md">staking-and-returns.md</a></td></tr><tr><td><strong>完整演算案例</strong></td><td>四个案例：释放价值、质押收益、提取销毁、团队奖励，每个数字都能复算。</td><td><a href="worked-examples.md">worked-examples.md</a></td></tr><tr><td><strong>价值流转</strong></td><td>六条流各自记账，最后汇成同一个飞轮。</td><td><a href="value-flows.md">value-flows.md</a></td></tr><tr><td><strong>XO 与 EXON</strong></td><td>两种资产各自的名字、角色与当前机制。</td><td><a href="xo.md">xo.md</a></td></tr></tbody></table>

*下一节：[双币，两份工作](two-assets-two-jobs.md)*
