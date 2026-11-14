# muse4ai：用Windows本地Muse会话向Agent开放REST／MCP的项目转述

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-13
阶段：相关项目

2026年11月13日09:51:48（北京时间），AI少年（@aehyok）的Muse集成清单介绍muse4ai在Windows本地使用自己的登录会话，经REST、MCP、OAuth向Claude、ChatGPT、Cursor、Codex及n8n提供图像和视频生成。它是AI工具互通相关项目，不是重建Muse模型，也没有确认AI辅助研究私有协议。

11月13日补充GitHub检索定位andrew-babo/muse4ai并读README前部，原更新日期未核，不另计候选。文档描述本机桥接、不经开发者中间服务器，OAuth授权需应用屏幕上的六位确认码，也可用有作用域、限流及可撤销的API key；这些是文档设计而非本合集安全审计。它仍向Muse服务发送生成请求，本地桥接不等于本地模型推理或无凭据访问。

658星为原清单快照，不以补查替换。未核许可文本、会话处理代码、授权实现、日志、测试徽章或生成作品，未登录、运行桥接或调用服务。REA未提及，标unknown／related-project；不把近乎免费宣传写成费用保证。

整帖封存7赞、648浏览、1转发、3回复；658星仅为清单的项目传播快照。

## 来源

- [AI少年Muse清单第三项：muse4ai本地会话与REST／MCP／OAuth，2026-11-13北京时间](https://x.com/i/status/2121058416340975899)
- [补充项目README：Windows本地REST／MCP与OAuth说明，11月13日查阅，原更新日期未核](https://github.com/andrew-babo/muse4ai/blob/main/README.md)

[English](en/muse4ai-local-session-rest-mcp-bridge.md) | [返回目录](../README.zh-CN.md)
