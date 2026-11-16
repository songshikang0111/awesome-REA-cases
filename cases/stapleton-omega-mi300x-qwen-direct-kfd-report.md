# Omega在MI300X运行Qwen：Stapleton报告绕过AMD用户态运行时直连kfd

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-16
阶段：待验证

2026年11月16日07:07:59（北京时间），介绍Michael Drake Stapleton研究的公开信列出‘Omega running Qwen3.8-27B on an AMD Instinct MI300X’（Zenodo 24237047），称这是面向UXL Open Source Working Group的技术简报。本条目标是AMD MI300X上的模型执行路径，与同一信中的NVIDIA GB10／CUDA++目标分开，不是另一个CUDA兼容实现。

按信中描述，2026年11月13日，一个Omega语言程序在MI300X运行Qwen3.8-27B-FP8，进程不加载AMD用户态运行时，直接通过/dev/kfd通信，已公布的解码中位时间为26.7毫秒／token。11月14日后续会话达到16.226毫秒／token，但优化构建尚未进入公共克隆，信中特意区分证据状态。这些日期早于候选，只是本次报告引用的运行日期；不由此推断不需要内核驱动、任意AMD卡兼容、模型完全正确或端到端吞吐。

信中把总体工作放在人类指导Agent跨GPU栈与模型运行时的背景下，未给这个具体执行路径的模型、Agent分工、源码提交或测试配置。未读技术简报、克隆或测量记录；补取Zenodo API返回403，记录号只作为信中引用追溯。本合集未运行模型或接触GPU，保留作者归因与unverified，不将未公开的快速版写成可复现性能，也不评判公开信的法律主张。

封存候选1赞、71浏览、0转发、0回复；26.7与16.226毫秒／token均为信中数字，后者构建未公开。

## 来源

- [公开信中的Omega／MI300X运行与两个证据阶段，2026-11-16 07:07:59北京时间](https://x.com/i/status/2122104354140205554)
- [信中所引MI300X技术简报24237047；正文未取得，API返回403](https://zenodo.org/records/24237047)

[English](en/stapleton-omega-mi300x-qwen-direct-kfd-report.md) | [返回目录](../README.zh-CN.md)
