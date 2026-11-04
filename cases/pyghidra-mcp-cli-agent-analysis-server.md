# PyGhidra-MCP：让Agent从CLI或共享GUI调用Ghidra

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-04
阶段：相关项目

2026年11月4日15:39:34（北京时间），候选介绍pyghidra-mcp命令行MCP服务，让智能Agent与LLM工具调用Ghidra。按名称查到clearbluejar/pyghidra-mcp并补读README，对照固定提交aeaf4d16b0ce09b6dc5e16bb56d204025d2f6f8e（11月2日21:59:25北京时间）；该提交是窗口外工具背景，不是本轮新发布或新实验。

项目通过PyGhidra与JPype把Ghidra的ProgramAPI／FlatProgramAPI接入Python，再开放MCP。README区分headless分析与--gui共享实时工程状态，推荐streamable HTTP，CLI客户端需先有运行中的HTTP服务，stdio用于不能接HTTP的MCP宿主。文档列反编译、交叉引用、字节、调用图、符号／字符串／代码搜索，以及重命名、类型、原型和注释修改；用ChromaDB做语义搜索，异步启动分析。

文档明确仍为积极开发的beta。收录为具体AI逆向基础设施，不声称这些接口能保证反编译准确、任意工程并行成功或自动恢复全部语义。README提单元及集成测试，本合集未检查CI执行记录、运行服务、安装依赖或分析二进制；也未认定它属于morluto/rea。

候选快照0赞、15浏览、0转发；公开文档功能不是本合集运行结果。

## 来源

- [候选：pyghidra-mcp服务介绍，2026-11-04](https://x.com/i/status/2117884444992512437)
- [补充项目README，固定提交2026-11-02，早于本窗口](https://github.com/clearbluejar/pyghidra-mcp/blob/aeaf4d16b0ce09b6dc5e16bb56d204025d2f6f8e/README.md)

[English](en/pyghidra-mcp-cli-agent-analysis-server.md) | [返回目录](../README.zh-CN.md)
