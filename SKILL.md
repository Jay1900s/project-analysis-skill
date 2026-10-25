---
name: project-analysis
description: "Evidence-first analysis of crypto projects, tokens, DeFi/GameFi mechanics, mining or share-based reward systems, on-chain strategies, and old research. Use when the user provides a project link, contract, whitepaper, dashboard, wallet case, or asks whether a project can make money, is a scam, or is worth participating in. Produces a Chinese decision-ready report with live verification, marginal unit economics, real cases, exit risk, and explicit disconfirming evidence."
metadata:
  short-description: "链上项目尽调与收益判断"
---

# 项目分析

把项目材料转成可执行判断，不写宣传稿。核心问题不是“项目是什么”，而是：

**按当前条件进入，钱从哪来、成本多少、怎么退出、什么证据会推翻结论。**

## 输出要求

- 默认中文，技术名词保留英文。
- 先给结论，再给证据；结论必须落在“可做 / 小仓验证 / 只研究 / 不参与”。
- 报告写入用户指定目录；未指定时写入当前工作目录。
- 文件名：`项目名-项目分析-YYYY-MM-DD.md`。
- 原始快照放入 `项目名_snapshot_YYYY-MM-DD/`。
- 不连接钱包、不签名、不提交交易，除非用户明确要求并再次确认。

## 执行顺序

1. **确认对象**：官网、官推、文档、合约、链、部署者是否互相对应。旧调研只能当线索。
2. **拉实时快照**：时间、区块、TVL 拆分、供应、费用、队列、交易状态、退出状态。
3. **重建资金流**：谁付款、付给谁、为什么付、谁承担亏损。区分充值、成交额、收入、奖励、增发。
4. **算边际单位经济**：用当前条件算每单位成本、日净现金流、回本天数；做乐观/中性/悲观三档。
5. **拆真实案例**：早期账户、晚期高换手账户、方向性盈利案例各一个。区分已实现/未实现、奖励/本金。
6. **检查退出与权限**：代币能否转让、提现是否排队、合约是否可升级、源码是否匹配、审计是否覆盖当前版本。
7. **写反证条件**：至少 3 条增强证据、3 条削弱证据。
8. **给分级结论**：绿 / 黄 / 橙 / 红，并写清参与限额。

## 关键判断规则

- 旧报告的价格、公式、TVL、状态默认视为过期，必须重新验证。
- 边际发行/边际收益优先于平均值。供应量增长后，旧公式可能完全失效。
- 份额制项目（算力、矿机、节点、NFT 分红）必须先算全网份额，再做算力翻倍压力测试。
- 收益来自新玩家本金或代币涨价时，标注“再融资依赖”，不能称为真实收益。
- 代币不可转让时，不计算市值/FDV，只按现金分红核算回本。
- 单日榜单、单笔盈利、高成交量都不能证明策略可持续。
- “有审计”“多签”“timelock”只降低特定风险，不构成安全保证。
- 无法验证的关键项必须写“未验证”，不能补全成确定事实。

## 参考文件

- 需要完整方法、公式、案例校准和常见错误时，读 [references/analysis-method.md](references/analysis-method.md)。
- 需要生成报告骨架时，读 [references/report-template.md](references/report-template.md)。

## 完成前检查

- 报告带时间戳、链/区块、数据源。
- 所有关键数字能由文中公式或接口复算。
- 结论与证据一致，没有把条件性回本写成固定年化。
- 明确写出未验证项和什么会改变判断。
- 不泄露私钥、API key、签名或完整钱包敏感信息。
