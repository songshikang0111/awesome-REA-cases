# rhabdomancer v1：在IDA数据库标注潜在危险API调用供后续分析

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-17
阶段：相关项目

2026年11月17日06:37:01（北京时间），吉川孝志（@MalwareBibleJP）整理Hex-Rays对haruspex、rhabdomancer与augur的v1介绍。rhabdomancer的独立任务是在IDA分析数据库中显示可能通向风险的API调用位置，让研究者聚焦可疑代码，再交LLM细看并由人静态、动态验证。

补读Marco Ivaldi的Hex-Rays作者文章，发布2026年11月12日19:52:28 UTC，及rhabdomancer固定ffed414 README，提交11月16日09:11:44 UTC，均是窗口前补证。文档确认调用点打印到stdout并标记IDB、按三档风险优先级组织，可配置API列表；作者文章把LLM深度初筛放在人工确认之前，并称Claude帮助编写测试。文章自测280个AArch64 ELF共14MB，旧v0.9.3／IDA 9.3为356秒，新v1.2.0／IDA 9.5为342秒，同一MacBook Air M3、无既有IDB且计初始分析；工具与IDA都升级，不能隔离各自收益。

危险API调用不自动等于可利用漏洞，工具也不是自主LLM Agent。函数导出属haruspex、字符串关联及39.3分钟对124秒属augur，不转移性能。LLM联动增强与LibAFL自动确认仍是作者计划。仅读原帖、作者文章与固定README，未审完整源码、配置规则或结果，也未运行IDA或目标；REA未提及，保留related-project。

同一三工具候选封存4赞、414浏览、1转发、0回复；不是rhabdomancer单独测试或漏洞数量。

## 来源

- [吉川孝志转述Hex-Rays三工具v1，其中rhabdomancer的API调用标注，2026-11-17 06:37:01北京时间](https://x.com/i/status/2122458950763499685)
- [窗口前补证：Marco Ivaldi的审计管线与组合版本比较，2026-11-12 19:52:28 UTC](https://hex-rays.com/blog/divining-vulnerabilities-contributor-program)
- [窗口前补证：rhabdomancer固定README，提交2026-11-16 09:11:44 UTC](https://github.com/0xdea/rhabdomancer/blob/ffed41482fd650e86b1256ae70146e5247aa8932/README.md)

[English](en/rhabdomancer-ida-risky-api-triage-tool.md) | [返回目录](../README.zh-CN.md)
