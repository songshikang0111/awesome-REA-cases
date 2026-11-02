# 0xloworbit的四角色交接指南：分析、规格、重建与验证分开

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-02
阶段：相关项目

2026年11月2日06:40:05（北京时间），0xloworbit（@0xloworbit）发布逆向Agent工作流指南介绍，主张将任务分为Analyst、Spec Writer、Rebuilder、Verifier四个独立职责，并明确列出环境边界、证据文件、行为规格和测试，让每次交接能被审阅。它针对把原目标观察与新实现、验收区分开的工程问题，而不是报告某个软件已经重建成功。

补查原帖确认署名与正文，但指南只由短链给出，未读全文、配置、代码或测试；帖中未明确REA或具体模型，不据四角色名称推断工具栈。与已有francescofaenzi的Grok Bots改编提案作者和发布对象不同，不把两者声称为同一实现。角色分工是方法主张，不保证操作系统权限隔离、法律clean-room合规或行为等价；未安装或执行。

候选快照0赞、10浏览、0转发；仅据指南介绍，未核验全文或案例验收。

## 来源

- [0xloworbit介绍四角色逆向Agent交接指南，2026-11-02](https://x.com/i/status/2117023901058486380)

[English](en/0xloworbit-four-role-reverse-engineering-handoff-guide.md) | [返回目录](../README.zh-CN.md)
