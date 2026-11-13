# Paranoia：Dopax介绍本地Rust逆向平台与可选AI／MCP入口

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-13
阶段：相关项目

2026年11月13日09:22:38（北京时间），Dopax（@tensorstaff）在开源五选中介绍Paranoia，定位为Rust写的本地优先逆向平台，分析PE、ELF和Mach-O等可执行文件，用于授权软件研究。它是具体逆向工具项目，而不是已完成某个目标的案例。

清单称其有反汇编、控制流图、x86/x64伪代码与调试，同一引擎供桌面、CLI、浏览器WASM与MCP使用；无遥测、默认不联网，但可选AI助手是例外。作者称Apache-2.0、约60星，桌面安装包只有Windows，Linux/macOS需源码编译或用跨平台CLI。不能把默认离线扩张成使用云模型也不发送数据，或把格式支持理解为每种架构均能生成伪代码。

补取只核清单作者与正文；没有审查项目源码、AI提供商、网络行为、许可证文本或安装包，没有反汇编样本、运行调试器或复现兼容性。60星只是2026年11月13日清单快照，非本合集GitHub测量。未说明使用REA引擎，归other-ai／related-project。

候选快照2赞、136浏览、0转发、0回复；约60星与Apache-2.0来自发帖者，未直接核仓库。

## 来源

- [Dopax清单第五项：Paranoia的逆向功能、可选AI与平台边界，2026-11-13北京时间](https://x.com/i/status/2121051078401614304)

[English](en/paranoia-rust-local-reverse-engineering-ai-platform.md) | [返回目录](../README.zh-CN.md)
