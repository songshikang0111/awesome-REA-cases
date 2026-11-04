# Linux显卡驱动idea：从NVIDIA反编译到NVIDIA／AMD电源管理与144Hz

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-05
阶段：待验证

2026年10月24日01:40:46（北京时间），@_fluk3_问@Wr0zen为什么没人用AI尝试反编译NVIDIA驱动。早期提案没有操作系统或用途，不替其补写意图。11月4日03:05:15另一读者提出AI逆向NVIDIA Linux驱动、用Rust重写改善稳定性；这是新增Linux与语言方向，不代表原作者已实现或两人合作。

11月5日00:58:35，joachim schiele（@joschelboschel）因reverse-engineer-anything出现，询问能否用它做不常崩溃、正常管理功耗的NVIDIA和AMD Linux显卡驱动，最好支持144Hz和驱动重启。这扩展了同一驱动研究idea的厂商范围和具体功能目标，没有分别提供两个独立驱动成果。REA只在这条新愿望中被提出，旧帖不追认使用。

三条都无GPU型号、驱动版本、二进制、模型、代码、日志或成功报告。Rust不自动保证稳定，也不能据提问认定已恢复电源管理或刷新率支持。保留unverified；未下载或分析驱动。

早期来源2026-10-24 01:40:46北京时间；11月4日候选1赞、21浏览、0转发。
Linux／Rust来自11月4日新读者，仍为无版本、无运行结果的idea。
11月5日候选1赞、45浏览、0转发；144Hz、电源管理与重启均为要求，非测得能力。

## 来源

- [@_fluk3_的NVIDIA反编译提问，2026-10-24](https://x.com/i/status/2113687087862215057)
- [Linux驱动Rust重写与稳定性提案，2026-11-04](https://x.com/i/status/2117694614056657158)
- [joachim的NVIDIA／AMD、功耗与144Hz愿望，2026-11-05](https://x.com/i/status/2118025124549132624)

[English](en/nvidia-video-driver-ai-decompilation-idea.md) | [返回目录](../README.zh-CN.md)
