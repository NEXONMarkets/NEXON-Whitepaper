---
description: "已定稿的早期轮档位、TGE 指导价、后续轮释放规则与 1,095 天 EXON 释放。"
icon: "chart-pie"
---

# 分配与释放

## 价格与轮次 <a href="#pricing-and-rounds" id="pricing-and-rounds"></a>

| 阶段 | 价格机制 | 释放 |
|---|---|---|
| 早期轮 | 固定 `0.1 U`，按档位限额 | TGE 起进入统一 1,095 天释放 |
| TGE | 指导价 `1.0 U`，NEX 开放现货 | 线性释放启动 |
| 后续轮 | 以实时市价折价，折扣逐轮披露 | T+1 开始释放 |

定稿给出的早期轮容量：

| 单份金额 | 份数 | 总额 |
|---:|---:|---:|
| 1,000 U | 10,000 | 10,000,000 U |
| 5,000 U | 1,000 | 5,000,000 U |
| 10,000 U | 500 | 5,000,000 U |
| **合计** | **11,500** | **20,000,000 U** |

## 线性释放 <a href="#linear-release" id="linear-release"></a>

数量 `A` 在 1,095 天内释放，每天两个 12 小时 Epoch，共 2,190 次：

```text
D = A / 1,095
R_epoch = D / 2 = A / 2,190
```

释放的 EXON 进入现货账户，可持有或交易；市场准入、流动性与成交价均不受保证。

## 未公布字段 <a href="#unpublished-fields" id="unpublished-fields"></a>

- EXON 数字总量。
- 团队、生态、Treasury 与市场的完整分配。
- 初始流通量。
- 后续轮规模、折扣与个人上限。
- 最终 TGE 与轮次日期。

*上一节：[EXON](exon.md) · 下一节：[质押与收益](staking-and-returns.md)*
