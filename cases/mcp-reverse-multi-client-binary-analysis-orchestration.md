# mcp-reverse：把静态分析、外部调试器与多AI协作接到同一MCP入口

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-01
阶段：相关项目

2026年11月1日16:46:01（北京时间），《マルウエアの教科書》作者账号@MalwareBibleJP介绍mcp-reverse：把二进制静态分析、外部调试器、技术资料搜索与多AI协作放到一个MCP服务器，面向Claude、Codex和Cursor。背景是游戏／反作弊研究中需要来回切换Ghidra、IDA、x64dbg等工具，帖子也列出恶意软件分析与移动端格式用途。它是逆向工作台项目，不是某个游戏已经被完整恢复的报告，也没有说明使用REA。

候选称内置PE、ELF、Mach-O、DEX、WASM、ZIP、.NET和小型转储等解析、字符串与密码常量检查、签名字节模式；反编译转发给已连接的外部MCP，可比较结果。其简易x86-64／ARM64模拟器用来分析短指令串或解密循环，不支持运行完整目标。帖子还描述Frida桥、任务交接、结果投票、共享JSON知识与MCP sampling：让客户端模型总结反编译结果或建议结构体名；这些都是功能说明，不是本合集运行结果。

补读1llu50ry/mcp-reverse固定提交2aa2e27f2e08e7c3bd2ee9d721d5e032fbd04a1a的README，提交为10月29日21:55:39北京时间，早于候选。文档确实展示5.0.1标记、stdio／HTTP入口、内置解析、外部后端和多客户端mesh，并要求只分析拥有或获准的二进制。但同页工具、后端、技能和测试数量存在不同口径，技术栈旧段写Node18+，候选写24+；不据此发布统一数量或安装版本保证。

帖子称反作弊风险等级是固定表而非实测，文件范围由MCP_FS_ALLOW／MCP_FS_DENY控制且默认不限制，HTTP认证通过MCP_AUTH_TOKEN可选开启。这些安全边界保留为转述，未独立审计代码或验证默认值；不要把服务器本地运行当成模型离线、投票当成正确性证明。未安装依赖、运行工具、连接调试器或测试游戏／样本。

候选快照6赞、698浏览、0转发；README检查不等于功能或权限审计。

## 来源

- [MalwareBibleJP介绍mcp-reverse与功能／安全边界，2026-11-01](https://x.com/i/status/2116814004752613748)
- [补充：mcp-reverse固定README，提交2026-10-29，早于窗口](https://github.com/1llu50ry/mcp-reverse/blob/2aa2e27f2e08e7c3bd2ee9d721d5e032fbd04a1a/README.md)

[English](en/mcp-reverse-multi-client-binary-analysis-orchestration.md) | [返回目录](../README.zh-CN.md)
