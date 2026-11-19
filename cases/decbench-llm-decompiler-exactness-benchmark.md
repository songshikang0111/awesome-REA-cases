# DecBench：用结构、类型与重编译相似度分别评估LLM反编译

分类：算法与功能重建 · 其他 AI 逆向
记录日期：2026-11-19
阶段：分析测试

2026年11月19日16:30:13（北京时间），yibie在工具目录更新中列出Noelo Lab的DecBench，称用于比较反编译器与现代LLM恢复精确源码的能力，并提Kuna榜首。该候选还介绍两个独立游戏项目，分别收录，不把整份目录当单一实验。

补读提交b65837037c7e93dbd3db01e72fa8d46641686dcb的README；该提交为11月11日04:38:13北京时间，早于窗口，只作方法补证。文档列控制流图编辑距离GED、相对DWARF的类型正确性，以及使用原工具链在编译修正fixup后重编译、归一化链接相关操作数、用Jaccard比较汇编的指标。Union是函数在三项任意一项完美的比例，不是三项同时正确或整二进制字节一致。

文档提供公开数据集和250函数外部参评样本，声明许多代码由coding agent生成，但人类拥有与负责核心思路和提交，不接受完全自动化贡献。未读取完整指标实现、实际排行榜或逐函数结果，故不确认Kuna当前第一、不采用137星为已核实热度，也未运行基准。保留analysis-test，评价的是有范围的函数指标，不是AI已恢复全部原始源码；未提REA。

## 来源

- [yibie的DecBench与两个游戏项目目录更新，2026-11-19 16:30:13北京时间](https://x.com/i/status/2123333006870131110)
- [补充DecBench固定README，提交2026-11-11 04:38:13北京时间](https://github.com/Noelo-Lab/decbench/blob/b65837037c7e93dbd3db01e72fa8d46641686dcb/README.md)

[English](en/decbench-llm-decompiler-exactness-benchmark.md) | [返回目录](../README.zh-CN.md)
