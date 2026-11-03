# Aeon soldecomp：公开Solana反编译与回放工作台，已停止维护

分类：应用与客户端 · 未确认使用 REA
记录日期：2026-11-04
阶段：相关项目

2026年11月4日03:22:35（北京时间），Aaron Mars（@aaronjmars）的Aeon十月月报第22项介绍soldecomp：研究已部署Solana程序，在本地回放真实交易以观察行为。它是AI Agent生态里的逆向相关工具，不是已证明AI自主恢复任意程序。

补充公开仓库README，固定提交dad5fd8fc3be59f6cf67247b027bf1bb5da53493于10月23日01:33:33北京时间，属于窗口前项目资料。文档说明Python标准库CLI可分析sBPF ELF、调用图、字符串与框架；Ghidra可产带Solana调用标签的类C伪码，修改的LiteSVM按交易前slot账户状态回放并比较单输入变异，也能编译候选Rust并比字节／分数。Ghidra、Solana工具与历史RPC按命令另需，并非自动Rust源码恢复，也不是原始链上执行的精确轨迹。

README明确released as-is, no longer maintained。五类检测器的13条判定自报precision0.83、recall1.0，但语料主要是合成控制与干净部署程序，已部署已知漏洞正例仅历史GoonFi一个；field_accuracy_measurable保持false，不能当实战效果。仓库标MIT，修改LiteSVM另保留Apache2.0。未执行基准、下载ELF、访问账户或重放交易；公开文档未确认AI模型或REA参与这项工具内部分析，状态保留related-project。同帖papertrade映射另列。

月报候选快照22赞、680浏览、7转发；为整帖热度，不是soldecomp单独使用量。

## 来源

- [Aaron Mars的Aeon十月月报，第22项soldecomp，2026-11-04](https://x.com/i/status/2117698975213944874)
- [窗口前固定README：功能、停止维护与合成基准限制，2026-10-23北京时间](https://github.com/aaronjmars/soldecomp/blob/dad5fd8fc3be59f6cf67247b027bf1bb5da53493/README.md)

[English](en/aeon-soldecomp-solana-program-transaction-replay.md) | [返回目录](../README.zh-CN.md)
