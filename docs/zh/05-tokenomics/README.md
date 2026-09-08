---
description: "NEXON 权威经济模型：双层架构、双代币职责、7228 资金路径、质押、释放、赎回与风险边界。"
icon: "coins"
---

# 通证经济

> 一个账户、两个运营层、一条可审计的经济流。

本部分执行项目方 2026 年 9 月 6 日定稿经济模型。任何早期 NEXON 文档与本部分不一致时，均由本部分覆盖。

NEX Main Exchange/CEX 是合规现货层，承载 EXON 现货、IEO 与释放呈现；Staking Platform 是独立的质押与奖励层，承载单币质押、期限权重、动态奖励与收益赎回。两层共享账户和资金后台，但质押参数不属于交易所现货规则。

每笔本金 `P` 都沿同一条路径拆分：

```text
B = 0.28 × P  → 按实时价买入 EXON → Treasury Liquidity
S = 0.72 × P  → 质押本金与奖励计算基数
B + S = P
```

{% hint style="danger" %}
本部分数值是协议参数与条件化演算，不构成收益、价格、回本周期或本金安全承诺。APY、代币价格、奖励率、执行参数与结果均可能调整或波动，参与者可能损失部分或全部本金。
{% endhint %}

## 本部分内容 <a href="#in-this-part" id="in-this-part"></a>

- [双币，两份工作](two-assets-two-jobs.md)划清 XO 与 EXON 的职责。
- [XO](xo.md)说明质押本金资产。
- [EXON](exon.md)说明核心价值与现货资产。
- [分配与释放](distribution.md)记录价格、早期档位与 1,095 天释放。
- [质押与收益](staking-and-returns.md)给出 APY、期限与奖励公式。
- [完整演算案例](worked-examples.md)复现项目方定稿中的条件化数学。
- [价值流转](value-flows.md)连接买入、锁仓、赎回与销毁。

EXON 数字总量、完整分配、初始流通、未来轮次限额及完整动态奖励表尚未公布，不得推测补齐。

*下一节：[双币，两份工作](two-assets-two-jobs.md)*
