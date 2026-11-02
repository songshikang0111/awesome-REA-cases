# RDX：Dopax转述Rust原生APK／DEX反编译桌面工具与MCP

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-02
阶段：相关项目

2026年11月2日09:24:17（北京时间），Dopax（@tensorstaff）介绍RDX为9月开始的Rust原生APK／DEX反编译桌面项目，自带MCP，可从清单进入重建Java并跟踪调用关系，不需JVM或外部反编译服务。用途是把Android安装包研究与导航集成到桌面及Agent流程。

补查原帖后，按名称找到Ch0pin/rdx并读固定提交4e5a6576c8999acd4b9a88b7bd363267a07227d3的README；提交为10月31日19:50:21北京时间，是窗口前补充文档。项目说明可让AI通过本地MCP浏览类、Java或DEX、清单与资源，多实例区分项目；支持APK、XAPK、APKS与DEX。状态为alpha，Java重建仍扩展中，未支持的方法显示带标签的DEX反汇编。README标Apache-2.0并披露改编JADX算法，不能写成未复用任何既有反编译知识的从零实现。

162星与9月开始是报道者口径，未独立核实。只读公开文档，未审算法实现、第三方许可细项、真实APK或原始Java对照，不证明完整源码恢复、所有APK可用或AI完成底层研发；REA未提及。与knife独立收录，未运行目标或安装依赖。

候选快照0赞、21浏览、0转发；162星与9月新项目均为报道口径，未独立核实。

## 来源

- [Dopax五项盘点中的RDX介绍，2026-11-02](https://x.com/i/status/2117065226063667699)
- [窗口前补充：RDX固定提交README，提交2026-10-31北京时间](https://github.com/Ch0pin/rdx/blob/4e5a6576c8999acd4b9a88b7bd363267a07227d3/README.md)

[English](en/rdx-rust-apk-dex-mcp-secondary-report.md) | [返回目录](../README.zh-CN.md)
