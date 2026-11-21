# Consessus：用REA研究四款Mac编程助手的本机通信，让已有会话互发消息

分类：应用与客户端 · REA
记录日期：2026-11-21
阶段：进行中

2026年11月21日08:53:23（北京时间），ns（@ns0bj）介绍开源项目Consessus：逐个研究Mac上Claude Code、Codex桌面应用、Antigravity和OpenCode如何通信，再把已有聊天连接起来，使一个应用的会话能给另一个发消息并读回答案。08:53:44的方法回复明确说使用自己的逆向Agent rea，列出Codex的长度前缀JSON本地IPC socket、Antigravity语言服务器的Connect-RPC、OpenCode本地HTTP服务器与Claude Code的peer socket。这是本机应用互通，不是重新训练四个模型或恢复整个应用源码。

补读同串08:53:46的说明，作者还报告统一会话列表、同一命令发送并读回、同目录项目房间及有限轮次讨论。另读取固定提交fd0874fe94457adb0ca0f68eedda40f7f8431c56（2026年11月21日09:04:46北京时间）的README相关章节、完整兼容表与协议笔记，作为补充项目文档而非独立候选。文档称11月19日在一台Mac上构建测试，11月20日跑过Antigravity、Codex与OpenCode CLI的发送／读回、四应用房间、轮流讨论，以及四任务四回答的分配；这些均是项目自记，不是本合集复现。

必须保留应用版本与路径区别：文档所列环境为Apple Silicon上的macOS 27.2，Claude Code 2.1.294、Claude Desktop 5.11492.5、Codex桌面26.1111.71025、OpenCode CLI 2.3.2与Antigravity应用2.33.0。OpenCode桌面1.19.5只能在会话内启动listener，不能用统一send直接寻址或读回答案，因此原帖“应用内不用安装任何东西”不能当成无例外保证。Codex CLI终端会话、Gemini CLI、Cursor CLI未覆盖；Antigravity IDE 2.6.0的新路径未实机测试。Claude直接send读回命令本身未跑实机，虽同一reader在房间内有自报测试；free讨论与room lead／set仍只用假对象测试。

项目明确依赖未文档化、易随升级变化的本机行为；socket写入、应用接受、模型读到与实际回答是不同证据。不同权限模式可能被接收端hold、拒绝或过期；peer数据不授予人类指令权限，也不改变应用审批模式。安全说明承认同一OS用户下的恶意进程不在隔离保证内，且有十项todo加固测试；README和兼容表对部分手改房间状态边界的描述也不完全一致，不能据此认证其安全。本合集只读来源，未安装项目、运行目标、联系本机会话、查看凭据或独立验证往返；保留in-progress。

11月21日封存快照：介绍帖0赞、24浏览、0转发、1回复；方法帖1赞、26浏览、0转发、1回复。
本合集未运行项目测试；项目自报live仅限所列版本与一台Mac，不证明全方向兼容或安全隔离。

## 来源

- [ns介绍Consessus跨应用会话互通，2026-11-21 08:53:23北京时间](https://x.com/i/status/2123942816397291683)
- [作者说明rea与四款应用通信入口，2026-11-21 08:53:44北京时间](https://x.com/i/status/2123942908319424668)
- [补充作者串：会话列表与项目房间，2026-11-21 08:53:46北京时间](https://x.com/i/status/2123942914501853479)
- [固定README相关章节，提交于2026-11-21 09:04:46北京时间；项目自报11月19至20日测试](https://github.com/nsozturk/consessus/blob/fd0874fe94457adb0ca0f68eedda40f7f8431c56/README.md)
- [同一固定提交的完整兼容表：实机、未测与已知限制](https://github.com/nsozturk/consessus/blob/fd0874fe94457adb0ca0f68eedda40f7f8431c56/docs/COMPATIBILITY.md)
- [同一固定提交的Claude本机peer协议历史笔记](https://github.com/nsozturk/consessus/blob/fd0874fe94457adb0ca0f68eedda40f7f8431c56/docs/discovery.md)

[English](en/consessus-rea-mac-agent-app-interoperability.md) | [返回目录](../README.zh-CN.md)
