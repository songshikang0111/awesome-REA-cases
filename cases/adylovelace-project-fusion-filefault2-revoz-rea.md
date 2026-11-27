# Project Fusion：AdyLovelace报告REA／Ghidra研究与FileFault 2 REVoz PoC

分类：应用与客户端 · REA
记录日期：2026-11-28
阶段：待验证

2026年11月27日08:51:03（北京时间），Qυεεn Λδγ Lονεlαcε（@AdyLovelace）发布Project Fusion，称用REA、Ghidra、AI Agents研究Abyss与MysticalCore，在macOS 27.3 AArch64得到FileFault 2 REVoz PoC。旧帖还提到借Craft Anything、Cláudio dos Códigos、ChatzinGePeTo开发自定义本地分析流程；保留昵称，不擅自对应商业模型。

11月28日00:57:11的新帖补足原先不明的FileVault 2背景。作者称2021年6月29日为Roland UA-25EX在macOS Big Sur上的兼容测试偶然发现方法，2025年9月2日在macOS 26 Tahoe x86-64测试中调整为阻止启用FileVault 2，11月4日分享给Universo Hackintosh以整合进EFI Base。又称2026年9月2日建MysticalCore，迁至自有MacBook Air M5 Midnight的macOS 27 Golden Gate AArch64环境，11月26日在27.3合并Abyss与MysticalCore为PoC。她将Abyss描述为造成KernelKit／KASAN fatal crash的阶段，明确不公开实现，材料限Kira's Lab内部研究与自有硬件。系统、组件和日期均为作者原文口径，不是本合集核实的系统发布史或机制。

新帖确实明确提到FileVault，故不能继续将其背景写成完全未知；但“再次打破FileVault”的自述不等于成功解密、绕过已加密磁盘、提权或已登记漏洞。阻止启用加密和破解已有加密也不同。未得到源码、样本、哈希、权限条件、调用日志、成功标准或修复信息；未审图片、运行PoC、下载目标或改变系统保护。保留未核验报告，不提供可执行攻击步骤。

旧帖2026-11-27封存1赞、53浏览、0转发、0回复；新帖2026-11-28封存0赞、44浏览、0转发、0回复。PoC名称与作者成功措辞均不是独立验证。

## 来源

- [AdyLovelace的Project Fusion与REA／Ghidra归因，2026-11-27 08:51:03北京时间](https://x.com/i/status/2126116558028108138)
- [同一作者补述FileVault背景、时间线和不公开计划，2026-11-28 00:57:11北京时间](https://x.com/i/status/2126359694402781459)

[English](en/adylovelace-project-fusion-filefault2-revoz-rea.md) | [返回目录](../README.zh-CN.md)
