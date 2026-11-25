# mcp-reverse现名Decompile：把二进制分析与多AI协作接到同一MCP入口

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-25
阶段：相关项目

2026年11月1日16:46:01（北京时间），《マルウエアの教科書》作者账号@MalwareBibleJP介绍mcp-reverse：把二进制静态分析、外部调试器、技术资料搜索与多AI协作放到一个MCP服务器，面向Claude、Codex和Cursor。背景是游戏／反作弊研究中需要来回切换Ghidra、IDA、x64dbg等工具，也列恶意软件分析与移动端格式用途。这是逆向工作台，不是某个游戏已完整恢复的报告，未说明使用REA。

旧候选称内置PE、ELF、Mach-O、DEX、WASM、ZIP、.NET与小型转储解析、字符串／密码常量与字节签名检查；反编译转发外部MCP并比较结果。简易x86-64／ARM64模拟器用于短指令串或解密循环，不能运行完整目标。Frida桥、任务交接、投票、共享JSON知识与MCP sampling让客户端模型总结反编译或建议结构体名，均是功能说明，不是本合集执行结果。

此前补读固定提交2aa2e27f2e08e7c3bd2ee9d721d5e032fbd04a1a的README，提交时间10月29日21:55:39北京时间，早于旧候选。文档展示5.0.1、stdio／HTTP入口、内置解析、外部后端及多客户端mesh，要求仅研究拥有或获准的二进制；同页工具、后端、技能、测试数量口径不同，旧技术栈Node18+与候选24+不一致，不统一成安装保证。

11月25日17:38:18新候选用1llu50ry/Decompile介绍同类工作台，称230多个工具、60多个后端、6000多个技能、170多个Agent、160多个子Agent、190多个插件和3000多提示词，Node24+；具体例子是pak_parse读取UE4／UE5 pak尾部魔数0x5A6F12E1、索引位置／大小及SHA1，hash_identify定位散列／密码常量，file_identify识别二进制格式。这些数量和行为仅为新帖说明，未读实现或重新计数，不能将解析器说成已破解加密pak或完成逆向。

本次补查GitHub公开API，旧路径mcp-reverse与Decompile均解析到同一仓库ID 1405229384、现名1llu50ry/Decompile，因此保留原案例ID和旧来源，追加更名而非重复收录。API是补充读取时的当前身份信息，不能据此确定更名原始日期或新帖时各功能均已实现。

旧帖安全描述仍保留：反作弊风险等级为固定表非实测，MCP_FS_ALLOW／MCP_FS_DENY默认不限制，MCP_AUTH_TOKEN可选HTTP认证；未审代码或默认值，不认证现版继承这些设置。服务器本地运行不等于模型离线，投票也不证明正确。未安装依赖、运行工具、连接调试器或测试游戏／样本。

11月1日候选快照6赞、698浏览、0转发；README检查不等于功能或权限审计。
11月25日候选封存0赞、24浏览、0转发、0回复；新工具／资源数未独立清点。

## 来源

- [MalwareBibleJP介绍mcp-reverse与功能／安全边界，2026-11-01](https://x.com/i/status/2116814004752613748)
- [补充：mcp-reverse固定README，提交2026-10-29，早于窗口](https://github.com/1llu50ry/mcp-reverse/blob/2aa2e27f2e08e7c3bd2ee9d721d5e032fbd04a1a/README.md)
- [Decompile的pak／常量分析与MCP工作台转述，2026-11-25 17:38:18北京时间](https://x.com/i/status/2125524470882517208)
- [补充公开API：旧仓库路径的当前身份与更名映射，读取2026-11-25，非功能验证](https://api.github.com/repos/1llu50ry/mcp-reverse)
- [补充公开API：Decompile当前仓库ID，读取2026-11-25，非原始更名日期](https://api.github.com/repos/1llu50ry/Decompile)

[English](en/mcp-reverse-multi-client-binary-analysis-orchestration.md) | [返回目录](../README.zh-CN.md)
