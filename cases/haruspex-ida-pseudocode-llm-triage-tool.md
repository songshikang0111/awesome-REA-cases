# haruspex v1：从IDA导出函数伪代码，供模式匹配与LLM漏洞初筛

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-17
阶段：相关项目

2026年11月17日06:37:01（北京时间），吉川孝志（@MalwareBibleJP）整理Hex-Rays对三个IDA工具v1的介绍。其中haruspex利用无界面IDA的idalib Rust绑定，按函数导出反编译伪代码文件，供Semgrep或weggli匹配以初筛二进制漏洞候选，之后再由LLM细看、人做静态与动态验证。报道说haruspex与augur同时输出结构体、枚举等类型定义，并调整IDA新显示形式供后续分析工具读取，涉及IDA 9.5支持。

补读Marco Ivaldi／HN Security在Hex-Rays的作者文章，发布日期2026年11月12日19:52:28 UTC，早于本窗口，仅作补证。作者明确描述上述LLM初筛链，并称用Claude辅助编写新单元、集成与回归测试。其MacBook Air M3自测：280个AArch64 ELF共14MB，工具v0.9.3／IDA 9.3的827秒，对v1.2.0／IDA 9.5的744秒，均从无既有IDB开始且包含初始分析；Semgrep 1.183.0可解析新版伪代码约99.1%的行，对旧版98.3%。这是语法可解析率，不是漏洞检测准确率。

另读固定e41b312 README，提交2026年11月16日09:11:37 UTC，确认逐函数文件、全局与局部类型头文件及最新IDA版本支持；Semgrep／weggli更紧密集成仍在TODO。LLM联动增强与LibAFL自动确认也是作者未来计划，不把现有人工确认写成全自动。性能同时包含工具与IDA升级影响，不能隔离成模型加速；39.3分钟对124秒仅属augur。同帖另两个工具分别记录。已读原帖、作者文章与固定README，未审完整源码、测试输出或复跑，没有安装IDA或执行目标；REA未提及，保留related-project。

同一三工具候选封存4赞、414浏览、1转发、0回复；共用快照，不是各工具独立热度或漏洞验证。

## 来源

- [吉川孝志转述Hex-Rays三工具v1，其中haruspex的伪代码与类型导出，2026-11-17 06:37:01北京时间](https://x.com/i/status/2122458950763499685)
- [窗口前补证：Marco Ivaldi作者文章与组合版本基准，2026-11-12 19:52:28 UTC](https://hex-rays.com/blog/divining-vulnerabilities-contributor-program)
- [窗口前补证：haruspex固定README，提交2026-11-16 09:11:37 UTC](https://github.com/0xdea/haruspex/blob/e41b312c0249854e894ce140c1103cebe3b23031/README.md)

[English](en/haruspex-ida-pseudocode-llm-triage-tool.md) | [返回目录](../README.zh-CN.md)
