# PatchHawk／Patch-to-PoC：Wonyoung Jung结合LLM与程序分析研究补丁到触发样例

分类：应用与客户端 · 其他 AI 逆向
记录日期：2026-11-08
阶段：进行中

2026年11月8日15:18:59（北京时间），VXCON（@vxresearch）预告Wonyoung Jung的混合LLM与程序分析框架，目标是自动化补丁差异研究和N-day概念验证生成。背景是分析者需追上游发布、从噪声中找安全变更，再手写输入重现已修复漏洞。

11月9日补读官方WonyoungJung简介，题为Automating N-Day PoC Generation: A Hybrid LLM + Program Analysis Framework for Patch-to-PoC。简介称以检索与代码差异摘要解释修改、LLM分类安全补丁，再由LLM引导输入合成、以fuzzing支撑触发样例；作者拟现场展示从厂商不透明补丁到验证PoC的流程。履历称其为78ResearchLab的AI研究负责人，正在建PatchHawk以自动化补丁分析、PoC和变体发现；未据此断言PatchHawk已完整交付。

会议安排11月28至29日，议程仍标Tentative。Working framework和validated PoC是简介自述与未来展示计划，不是本合集目击的运行结果；无目标版本、仓库、样例、覆盖率、失败表或漏洞披露记录。官网原始日期未标，是窗口后补读文档。REA未提及，本合集未生成或执行利用、运行fuzzing或接触目标。

共同候选封存10赞、726浏览、7转发；整条活动预告的快照，不等于PatchHawk用户量或验证结果。

## 来源

- [本窗候选：VXCON预告LLM与程序分析补丁差异框架，2026-11-08 15:18:59北京时间](https://x.com/i/status/2119328813767409993)
- [补充官方简介：Wonyoung Jung与PatchHawk，2026-11-09取阅，原始日期未标](https://vxcon.hk/#WonyoungJung)

[English](en/vxcon-wonyoung-llm-patch-diffing-nday.md) | [返回目录](../README.zh-CN.md)
