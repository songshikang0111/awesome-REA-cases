# Metis：静态分析与LLM合成EDK2启动期协议fuzz harness

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-04
阶段：分析测试

2026年11月4日10:29:21（北京时间），Tanat Tonguthaisri（@gastronomy）转发Towards Effective Fuzzing of EDK2 Components摘要。Metis针对TianoCore EDK2的UEFI启动期接口，将协议重托管成用户态程序；DCR（直接依赖组件重托管）为依赖构造语义mock，让协议接口及依赖交互都作为输入通道。静态分析结合LLM引导的合成来生成、迭代fuzz harness，基于HBFA实现。

摘要称评估60驱动、162协议，覆盖73.1%、约为FuzzUEr的1.7倍；发现137个此前未知bug，已报告26个、其中12个可远程触发，且已报告项均获厂商确认。这些是论文摘要主张，不把137个bug都写成确认漏洞，也不当本合集运行结果。补取确认转发者，arXiv检索超时，未取得论文全文、提交、样本、覆盖口径或厂商公告。模型与REA未知，未下载固件或执行fuzzer。

候选快照0赞、4浏览、0转发；所有覆盖率、bug数与确认情况按摘要归因。

## 来源

- [Tanat转发Metis／EDK2论文摘要，2026-11-04](https://x.com/i/status/2117806376432853251)

[English](en/metis-edk2-llm-guided-rehosting-fuzzing.md) | [返回目录](../README.zh-CN.md)
