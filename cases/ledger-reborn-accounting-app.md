# Ledger Reborn：研究 QuickBooks 后制作独立记账应用

分类：应用与客户端 · REA
记录日期：2026-11-01
阶段：相关项目

一则第三方quote帖将Ledger Reborn描述为针对QuickBooks作REA／Ghidra研究后开发的独立记账应用，涉及库存成本、预算与对账。帖文称维护者独立编写Python／SQLite引擎和界面，并称已有Windows与Mac预览版，可用保存的数据生成发票、处理部分付款及查看报告。原帖未标明维护者身份，也不是维护者本人确认。

2026年11月1日01:30:00（北京时间），新候选在REA6.7.0介绍中补充：创建者实际使用REA6.4.0与Ghidra研究QuickBooks Desktop for Mac2024，逐项调查库存计算、账户类型如何影响预算、对账余额与现金制报表；据称用Intuit官方示例公司逐账户比较损益表、资产负债表和试算表，精确到分一致。具体方法是每次问一个行为问题，以真实输入输出例子约束规格，区分观察、推断与未知，重建差一分钱就视为解释不对。

新帖仍是第三方转述，没有独立审计、可复核比较文件、已识别维护者或本合集实测；不能推广为所有账务、税务或版本兼容。6.7.0是介绍对象，不误写成该案例使用版本。帖子提醒REA并非沙箱、以本机权限运行，材料可能到达模型供应商；这是操作边界，不是本次检查过的安全保证。保留旧来源和项目ID，按明确REA归因的相关项目补证，不把两次转述当两次复现。

Reported target: QuickBooks
Reported research: inventory costs, budgets and reconciliation
Reported implementation: Python + SQLite engine and interface
Reported availability: Windows and Mac preview
Evidence is a third-party quote post, not direct maintainer confirmation
11月1日候选快照0赞、20浏览；到分匹配为转述，未取得比较文件。

## 来源

- [Third-party quote post; project maintainer not identified or directly confirming](https://x.com/i/status/2110262015063105757)
- [11月1日第三方补充：Mac2024、REA6.4.0与逐账户到分报表比较，未独立审计](https://x.com/i/status/2116583480067076206)

[English](en/ledger-reborn-accounting-app.md) | [返回目录](../README.zh-CN.md)
