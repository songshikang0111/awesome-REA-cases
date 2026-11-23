# 闭源Electron到独立客户端：Patch称REA与Claude四分钟梳理IPC及WebSocket

分类：应用与客户端 · REA
记录日期：2026-11-23
阶段：待验证

2026年11月23日05:31:32（北京时间），Patch（@PatchOnChain）称自己将Claude Code通过REA MCP桥接指向一款闭源Electron应用，四分钟内反编译IPC总线、映射隐藏WebSocket API，并写出所谓clean-room客户端。Electron是桌面应用框架；这里的具体目标是理解应用进程间通信及本机或网络接口，重写一个调用这些接口的客户端，不是已证明能自动复制任意闭源二进制。

补取原帖确认署名与文字，没有媒体附件，也未给应用名、版本、操作系统、IPC方法、WebSocket端点、客户端源码、请求响应或运行测试。四分钟是作者自述而非计时验收；clean-room也是作者用语，没有人员隔离或实现来源材料可核。不能据此认定原程序全部功能已恢复、兼容性成立或法律授权已确认。帖子末尾的教程链接不替代项目证据。仅保留unverified报告，本合集未运行应用或客户端。

封存快照1赞、295浏览、0转发、0回复；未取得代码与计时记录。

## 来源

- [Patch的REA MCP／Claude Code闭源Electron客户端报告，2026-11-23 05:31:32北京时间](https://x.com/i/status/2124616797534257495)

[English](en/patch-rea-electron-websocket-client-report.md) | [返回目录](../README.zh-CN.md)
