---
description: "稳定币卡把合格的数字价值延伸到日常商户受理，依赖一个持牌发卡 / 运营方。"
icon: credit-card
---

# 稳定币卡

*产品阶段 · Roadmap*

稳定币卡是从合格数字价值通往**日常商户受理**的一座桥。它把 NEXON 的价值闭环延伸到商城库存之外——延伸到便利店、餐厅和任何一台收单终端。

## 卡不是界面发的 <a href="#an-interface-does-not-issue-a-card" id="an-interface-does-not-issue-a-card"></a>

一张卡由**发卡机构**发出。持牌发卡 / 运营方决定资格、KYC / AML 要求、接受的充值资产、兑换、托管、授权、结算、费用、限额、退款、争议和持卡人保护。卡组织规则与商户规则同样适用。

NEXON 这一侧的工作是把体验接起来：准备一条合格的充值路径、展示报价与成本、请求有边界的授权、显示授权状态、把发卡机构的凭证对上账。**发卡机构必须始终可见**，而不是让 Agent 看起来像那个批准交易的金融机构。

## 目标流程 <a href="#the-target-flow" id="the-target-flow"></a>

{% stepper %}
{% step %}
### 选来源与额度

用户选择一个受支持的充值来源和一笔消费额度。
{% endstep %}

{% step %}
### 校验

PayFi 检查产品与辖区资格、储备策略和报价新鲜度。
{% endstep %}

{% step %}
### 展示

界面展示兑换、费用、限额、发卡机构与有效期。
{% endstep %}

{% step %}
### 审批

用户批准这个写明范围的动作。
{% endstep %}

{% step %}
### 执行

发卡 / 运营方按自己的条款处理充值、卡授权与结算。
{% endstep %}

{% step %}
### 对账

钱包把金融结算与任何商户退款或争议**分开记录**。
{% endstep %}
{% endstepper %}

离线授权、商户周期扣款、小费、冲正和拒付，都需要产品层面的专门处理。**它们不能被硬塞进一个通用的链上最终性模型里。**

## 代币与经济边界 <a href="#token-and-economics-boundary" id="token-and-economics-boundary"></a>

定稿的 Tokenomics 没有把 EXON 指定为当前的卡结算燃料，也没有把 XO 指定为卡抵押。EXON 的支付与费用角色属于长期方向。如果未来某张卡直接支持 EXON，或在一条已披露的兑换路径中使用它，那份支持必须写明价格来源、流动性、点差、费用、托管与退款处理。

卡的经济与 Staking Platform 的奖励、EXON 的赎回销毁**各走各的**。一笔卡交易不会因为出现在同一个生态里就获得质押收益；一次商户退款也不受赎回销毁规则管辖。

## 上线之前要交付什么 <a href="#what-has-to-ship-before-launch" id="what-has-to-ship-before-launch"></a>

指名的授权运营方、责任的合同分配、辖区覆盖、支持的充值资产、托管与资金保管条款、反欺诈与制裁筛查、安全审查、清晰的费率、客户支持与争议流程。发卡机构、日期、费率与辖区属于[待定参数](../open-parameters/README.md)（OP-P05）。

*上一节：[商城](marketplace.md) · 下一节：[通证经济](../05-tokenomics/README.md)*
