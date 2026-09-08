---
description: "应用架构，以及 NEX 现货运营与可调 Staking Platform 之间的严格边界。"
icon: "diagram-project"
---

# 协议架构

NEXON 是位于资产与服务原生链、场所和供应商之上的应用层。每个执行分段仍受其原生系统与责任方约束。

## 核心子系统 <a href="#core-subsystems" id="core-subsystems"></a>

| 子系统 | 职责 |
|---|---|
| 意图层 | 结构化目标与约束 |
| Agent 运行时 | 路径提议、审批、限定委托与撤销 |
| 结算与托管 | 原生执行、对账、回滚与争议记录 |
| 质押与奖励层 | XO 本金、EXON 储备校验、12 小时奖励账本与赎回 |
| 数据与预言机 | 价格、资格证明、库存与熔断 |

经济边界明确：NEX Main Exchange/CEX 承载 EXON 现货、IEO 和释放呈现；Staking Platform 承载单币质押、期限权重与动态奖励。统一账户可以同时展示两层，但权限、账本、披露和参数版本保持独立。

架构章节不得把 XO 重新定义为 Agent 抵押，也不得把 EXON 改写成通用路径结算燃料。权威角色固定于[双币，两份工作](../05-tokenomics/two-assets-two-jobs.md)。

*下一节：[意图层](intent-layer.md)*
