# Educator 64 KERNAL：Scientific Brad称REA识别8KB ROM并重组哈希一致

分类：硬件与设备互通 · REA
记录日期：2026-11-08
阶段：分析测试

2026年11月8日00:20:38（北京时间），Scientific Brad（@ScientificBrad）报告把标为901246-01的8KB ROM dump交给REA与Ghidra，识别为1983年Commodore 4064（Educator 64）的KERNAL，继而反汇编、重组，并称SHA-256完全一致。作者还称重建了可在PowerShell中运行的原生可执行文件，帖带antigravity标签，未据此确定具体模型。

目标是理解并重现老机器ROM行为。重组哈希相同即使属实，也仅针对输入ROM与重组字节，不证明原生程序同样字节匹配、完整操作系统移植或Educator 64硬件兼容。补取有两张图片，alt文字分别描述代码和PowerShell中的C64概念验证；未观看图片、取得ROM、哈希值、源码、可执行文件、测试向量或外设验证。

8KB、1983年和匹配结论均为作者口径，没有独立查验ROM身份或复现。只保留文字与附件描述，不分发ROM，未执行目标代码。

候选封存0赞、25浏览、0转发；SHA256匹配为自述，未取得哈希或文件。

## 来源

- [Scientific Brad的8KB Educator64 ROM识别、重组与原生概念版报告，2026-11-08 00:20:38北京时间](https://x.com/i/status/2119102738021928969)

[English](en/scientificbrad-educator64-kernal-rea-rom-reassembly.md) | [返回目录](../README.zh-CN.md)
