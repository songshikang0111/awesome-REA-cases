# Joying.eth的17仓库逆向工作室：REA路由反编译、调试与流量工具

分类：应用与客户端 · REA
记录日期：2026-11-02
阶段：相关项目

2026年11月2日05:47:53（北京时间），Joying.eth（@Joyingeth）把“REA + 16 repos”称为自己的逆向工作室，报告粘贴一份配置后17个仓库在同一会话、五组结构中接入一个MCP。目的是把不同分析路径接到Agent：REA组织流程，原生二进制交Ghidra，APK交jadx，.NET用ILSpy和dnSpy，Frida做运行时观察，另列radare2、x64dbg、ImHex、mitmproxy与angr。

作者将范围限定自有应用和开放二进制，不做保护绕过或许可破解。补查原帖确认署名和全文，但没有完整17项名单、配置、连接日志、具名分析目标或验收结果；附视频未观看。412.4k／96.2k星数是作者给REA／Ghidra的推广快照，不是本合集核验，亦不作为功能证据。“每个二进制可读”“每个包可见”等绝对措辞不表示实际覆盖，工具被列出也不证明已通过MCP完整接通。保留具体编排方案与集成自述，不安装或执行任何仓库。

候选快照20赞、943浏览、1转发；17仓库／五组为作者口径，缺完整配置与测试。

## 来源

- [Joying.eth的REA与17仓库逆向工作室配置自述，2026-11-02](https://x.com/i/status/2117010764972044602)

[English](en/joying-rea-seventeen-repo-reverse-engineering-studio.md) | [返回目录](../README.zh-CN.md)
