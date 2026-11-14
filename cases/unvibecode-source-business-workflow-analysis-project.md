# UnvibeCode：从代码库重建业务流程与风险，混合许可且AI分析可能外发代码

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-15
阶段：相关项目

2026年11月15日00:01:03（北京时间），Micha(el) Bladowski（@michabbb）介绍UnvibeCode，针对复杂或AI生成代码库难以理解业务流程的问题，按源码追踪执行路径、决策、依赖和状态变化，而非反编译二进制。补充检索找到FinanceFlash/unvibecode并阅读README；仓库快照提交c75b75e为2026年11月4日07:32:04 UTC，早于本窗口，是文档补证，不是新候选或本轮实测。

介绍与文档列四类输出：业务工作流图、文件／导入／符号／依赖的交互关系图、有源码证据的潜在业务缺陷，以及完整或聚焦文件周边的代码上下文包。文档给Python3.11+和review --repository入口，并链接smolagents、PocketFlow、mini-swe-agent、django-payments的示例分析。没有在此阅读示例逐项结果，不能从发布示例推出准确率、完整覆盖或已确认漏洞；项目自己也说证据不足时不应输出确认发现。

候选简写Apache-2.0，但README明确混合许可：Apache覆盖的材料保留其许可，官方Python包还可能含专有业务定义、工作流原型与分析资产，内部商用与提取／独立再分发限制须分别核对。文档说不需激活或客户OpenAI key，同时明确客户端会在AI分析外发代码前替换可识别凭据，深度编码或自定义格式可能漏检；这不是全离线、绝不外发或秘密安全保证。本合集未安装、运行项目、上传代码、核读全部许可资产或复核样例，仅据公开项目说明收录。REA未提及。

候选封存0赞、31浏览、0转发、2回复；100000行是介绍中的问题设定，不是此次实测规模。

## 来源

- [Micha(el) Bladowski的UnvibeCode介绍，2026-11-15 00:01:03北京时间](https://x.com/i/status/2121634523704328567)
- [窗口前项目README：输出、隐私与混合许可，仓库快照提交2026-11-04 07:32:04 UTC](https://github.com/FinanceFlash/unvibecode/blob/c75b75e26cfd2cca923d2030f3b0a7056eadd89d/README.md)

[English](en/unvibecode-source-business-workflow-analysis-project.md) | [返回目录](../README.zh-CN.md)
