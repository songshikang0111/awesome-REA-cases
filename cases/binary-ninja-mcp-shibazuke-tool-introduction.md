# Binary Ninja MCP：shibazuke介绍让Agent查询IL、改类型与打补丁的插件

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-26
阶段：相关项目

2026年11月26日22:06:49（北京时间），shibazuke（@shibazukesec）介绍两种供AI Agent使用的二进制分析MCP服务器。其中Binary Ninja MCP是Binary Ninja的插件，帖子列反编译、中间表示IL、交叉引用、函数／变量重命名、类型定义和补丁接口，并称可自动配置Claude Code、Cursor等客户端。目标是让Agent调用现有逆向工具，不是已恢复某个软件或发现漏洞的报告。

已补取确认署名与完整文字。原帖短链未展开，公开搜索有多个同名插件，无法唯一认定作者指哪一仓库，因此不拿检索到的相似项目代替原链接或声称审过实现。候选后半段Docker实试明确指mecha_ghidra，不转移到本插件。无目标样本、版本、编辑前后差异、测试或安全审计；功能均为介绍者转述。保留related-project，REA未提，本合集未安装或执行插件。

同帖封存2赞、93浏览、1转发、0回复；不是本插件独立热度或实测。

## 来源

- [shibazuke同帖第一项：Binary Ninja MCP插件介绍，2026-11-26 22:06:49北京时间](https://x.com/i/status/2125954431783145732)

[English](en/binary-ninja-mcp-shibazuke-tool-introduction.md) | [返回目录](../README.zh-CN.md)
