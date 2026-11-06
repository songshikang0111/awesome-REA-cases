# REA Rust与原生Ghidra worker：公开移植文档补足早期基准线索

分类：应用与客户端 · REA
记录日期：2026-11-06
阶段：相关项目

2026年10月24日19:32:18（北京时间），Nicolas Krassas（@Dinosn）分享Java vs Rust Ghidra in REA的早期基准标题，彼时只有标题、未取得实现或数字。11月6日09:29:00，EveryDev.ai（@EveryDevAi）介绍@linanashi的本地Rust移植，称CLI与MCP共享handler、原生Ghidra worker不需JVM，195／209个冻结工具有原生handler。这是第三方功能覆盖说法，不是195项语义等价或独立测试。

补充找到描述吻合的nanashili/rea-rust，静态读固定提交0fb566c88620004af8a4c6f63ccfb56fe7f39962的README，提交为10月26日22:53:24北京时间，早于候选。保留既有REA／Rust Ghidra调查ID，不另建同目标；不据此证明10月24日短链文章一定指该仓库，也不把分享者当开发者。项目是morluto/rea的Rust移植，CLI和MCP共用实现，运行时不需Node，预编译发行包含worker。源码构建时worker需单独构建；文档说使用原生Ghidra反编译器且不需JVM，其他分析后端仍须自行安装，Frida为可选特性。本地工具不等于所接Agent或模型不联网。README标MIT，许可正文未另查。

README给出10月24日M1 Pro、热文件缓存、冻结构建、各七次会话的项目比较：Go元数据冷启动570对64毫秒，但常驻会话重复请求7.3对16.2毫秒，Rust并非每项都更快。小C函数首次反编译9.43对0.39秒，采样进程族峰值内存1022对214MiB；两边分别用Java与Rust Ghidra，不能将差异单归Rust语言。较大Go样本Rust因导入名冲突失败，Java返回三个请求函数。另提11款macOS应用与Go、25流程125样本及失败重测；未读其全套原始结果，也未复核195／209数量。

本次公开文档补足原先无仓库与数值的证据空白，但不证明完整替代Java Ghidra、跨平台功能等价或移植由AI完成。本合集没有构建、安装发行包、运行目标或重测基准。

旧标题仍只代表分享线索；本次补读公开实现文档，未确认旧文章与仓库直接对应。
11月6日候选封存0赞、15浏览、0转发；195／209来自第三方，性能来自项目自测，均未独立运行。

## 来源

- [Nicolas Krassas分享早期Rust/Java Ghidra对照标题，2026-10-24](https://x.com/i/status/2113956746242994214)
- [EveryDev.ai介绍Rust REA与195／209 handler说法，2026-11-06 09:29北京时间](https://x.com/i/status/2118515963494809669)
- [补充固定README：2026-10-26提交，原生worker与有失败边界的基准](https://github.com/nanashili/rea-rust/blob/0fb566c88620004af8a4c6f63ccfb56fe7f39962/README.md)

[English](en/rea-ghidra-rust-port-early-benchmarks.md) | [返回目录](../README.zh-CN.md)
