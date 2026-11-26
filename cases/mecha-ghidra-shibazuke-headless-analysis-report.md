# mecha_ghidra：shibazuke报告Docker接MCP自动读二进制，文档补足分析边界

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-26
阶段：待验证

2026年11月26日22:06:49（北京时间），shibazuke（@shibazukesec）在二工具介绍的第二项，称亲自用Docker启动mecha_ghidra、接MCP后，Agent自动读入二进制、反编译并分析，无须打开GUI。帖子列多二进制切换、BSim相似函数搜索及长输出处理；这是一次未具名目标的个人试用，不是独立代码恢复验收，也不把同帖Binary Ninja MCP并成一个工具。

补读ghidra-user-jp/mecha_ghidra固定7ff4264d07c52572b2c555a82044d38ad7877558的README，提交于2026年10月26日12:19:58 UTC（北京时间20:19:58），早于本窗口，仅作为项目文档补充。文档说明独立MCP经PyGhidra访问Ghidra API，由Agent选择分析步骤；可以改名、类型、注释、撤销和导出，Ghidra Server共享结果供人类GUI继续，BSim可搜索已登记二进制的相似函数。大结果通过分页／搜索按需读取，不是已证明无损语义压缩。

本地分析不要求Server或BSim；共享编辑需checkout／check-in，不支持headless冲突合并。README明确启动不自动建项目／导入，加载也不分析，未分析目标须另行analyze_program。文档列Python 3.10+、uv、兼容JDK与Ghidra，原生构建当前针对12.2；这些是依赖说明，本合集未安装。文档自述Apache 2.0，未审LICENSE原文。没有作者试用的样本hash、模型、调用日志、准确率或分析结果；只读文档，未启动Docker、审完源码或复跑，不认证自动分析正确、无副作用或漏洞检出，REA未提。

同帖封存2赞、93浏览、1转发、0回复；Docker试用为作者自述，不是本合集复跑。

## 来源

- [shibazuke同帖第二项的mecha_ghidra实试，2026-11-26 22:06:49北京时间](https://x.com/i/status/2125954431783145732)
- [补充固定README：PyGhidra、BSim与加载／分析边界，提交2026-10-26 12:19:58 UTC，窗口前](https://github.com/ghidra-user-jp/mecha_ghidra/blob/7ff4264d07c52572b2c555a82044d38ad7877558/README.md)

[English](en/mecha-ghidra-shibazuke-headless-analysis-report.md) | [返回目录](../README.zh-CN.md)
