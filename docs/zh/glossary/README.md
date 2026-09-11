---
description: "NEXON 叙事、现行机制、长期产品与披露边界的中英对照词表。"
icon: book
---

# 术语表

## 架构与单位 <a href="#architecture-and-units" id="architecture-and-units"></a>

| 术语 | English | 定义 |
|---|---|---|
| U | U | 计价单位，锚定 USDT |
| NEX 交易所 / 现货层 | NEX Exchange | XO 自由交易、EXON 现货（只卖不买）与逐日释放呈现；不含质押奖励模型 |
| 质押与奖励层 | Staking Platform | XO 质押、每 12 小时结算、期限加成、推广奖励、领导奖金与收益提取 |
| 结算周期 | Epoch | 12 小时的收益与释放间隔，每天两次，北京时间 08:00 / 20:00 |
| 燃料钱包 | Fuel wallet | 入金的 28% 按当时 1 U 等值买入的 EXON 的去处；只能销毁，不能转出、不能交易 |
| 上线 | Listing | EXON 以 1.0 U 在 NEX 现货开放、首日释放的起点 |

## 资产与角色 <a href="#assets-and-roles" id="assets-and-roles"></a>

| 术语 | English | 定义 |
|---|---|---|
| 新一代价值连接网络 | NEXON | NEX（Nexus）+ ON；连接资本、数字金融与真实消费的生态 |
| 价值锚 | Value Anchor | XO 的叙事角色：质押、参与、治理与长期价值沉淀 |
| 流通引擎 | Circulation Engine | EXON 的叙事角色：连接交易所、支付、兑换、费用与消费 |
| 质押本金代币 | Staking Principal Token | XO 的当前机制角色：本金在它上面计息，三种奖励一律以它发放，在 NEX 自由交易 |
| 核心价值代币 | Core Value Token | EXON 的当前机制角色：私募唯一渠道、只能卖不能买、燃料钱包买入、提取即销毁 |

## 经济机制 <a href="#economic-mechanism" id="economic-mechanism"></a>

| 术语 | English | 定义 |
|---|---|---|
| 入金拆分 | Deposit split | 入金的 28% 买入 EXON 存入燃料钱包，其余兑换 XO 进入质押 |
| 单次产出 | Per-epoch yield | 每 12 小时结算一次，0.3% – 1.0%；质押 1,000 U 一天 6 – 20 U |
| 期限加成 | Term bonus | 30 / 90 / 180 / 360 / 540 天对应基础 / +10% / +20% / +30% / +50%，只看期限不看金额 |
| 退出窗口 | Exit window | 30 天档的第 31 天，本金加收益一起领，不收违约金；错过自动续期 |
| 到账方式 | Settlement speed | 提取收益的三档：立即到账销毁 30%、30 天到账 20%、60 天到账 10% |
| 私募 | Private sale | EXON 唯一的获取渠道：0.1 U，三档 1,000 / 5,000 / 10,000 U，共 11,500 份 |
| 认购与质押配置 | Subscription-to-stake ratio | 私募期 3:1（质押金额取整数），上线后 1:1 |
| 线性释放 | Linear release | 上线当日起 1,095 天、2,190 次逐日释放 |
| 推广奖励 | Referral rewards | 最多 20 代、合计 76%，按下级每日静态产出计算，以 XO 发放 |
| 等级极差 | Differential Matching Bonus | 领导奖金 V1 – V12 的发放方法：本人比例减去下级比例 |
| 永久销毁 | Burn | 提取收益时从燃料钱包销毁的 EXON，永久退出流通 |

## 控制路径 <a href="#the-control-path" id="the-control-path"></a>

| 术语 | English | 定义 |
|---|---|---|
| 意图 | Intent | 结构化的用户目标、约束与审批方式；不是交易，也不是授权 |
| 路径 | Route | 带版本的合格分段序列，含成本、执行方、权限与失败行为 |
| 策略校验 | Policy Check | 对账户、辖区、余额、限额与产品规则的确定性判定 |
| 凭证 | Receipt | 关于批准了什么、执行了什么、结算了什么、履约了什么的证据 |

## 产品 <a href="#products" id="products"></a>

| 术语 | English | 定义 |
|---|---|---|
| AI 原生 PayFi | AI-Native PayFi | 已上线的价值路由器；EXON 是它的流通与结算通证；AI 不是收益引擎 |
| 钱包 | Wallet | 状态、权限、质押入口与合格第三方体验的金融主页（开发中） |
| 预测市场 | Prediction market | 第三方入口，受其自身托管、结算与辖区规则约束 |
| 商城 | Marketplace | 旅游、酒店、商品与服务的真实消费面，按供应商条款执行（开发中） |
| 稳定币卡 / U 卡 | Stablecoin Card | 需要一个持牌发卡 / 运营方的日常受理产品（Roadmap） |
| 去中心化社交 App | Decentralized Social App | 发现与社区面；社交语境不授权金融执行（开发中） |
| 待定 | Open | 有待项目方书面决定的实现字段 |

## 用词纪律 <a href="#usage-discipline" id="usage-discipline"></a>

「单次产出」「期限加成」「ROI」「收回认购款」描述的是**机制参数或算术**。「价值锚」说的是生态角色。「流通引擎」说的是 EXON 随五个入口逐个接入的方向。

叙事术语与机制术语同时出现时，**两层都要说**。推荐写法：

> XO 是价值锚，当前是质押本金代币：每 12 小时结算，三种奖励一律以 XO 发放。
>
> EXON 是流通引擎，当前是核心价值代币：私募唯一渠道，只能卖不能买，提取即销毁。

*上一节：[路线图](../09-roadmap/README.md) · 下一节：[法律声明](../legal-disclaimer/README.md)*
