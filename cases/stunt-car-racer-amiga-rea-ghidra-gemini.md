# Stunt Car Racer：REA遇m68k瓶颈，作者转用Ghidra与Gemini

分类：游戏与游戏保存 · REA
记录日期：2026-10-31
阶段：进行中

2026年10月31日22:59:29（北京时间），Scientific Brad（@ScientificBrad）报告把REA用于喜欢的1989年Amiga游戏Stunt Car Racer。它没有AmigaDOS，使用RNC raw-MFM加载器，作者提到XOR-$80代码、校验和及可疑68000 TRACE向量，称REA撞到m68k支持瓶颈；随后Ghidra反编译480函数，映射定点悬架与物理逻辑，现由Gemini继续。目标是理解旧赛车实现并尝试重建，不是另一个Stunts浏览器项目。

补查确认作者和完整文字；图片alt写Gemini重建经典Stunt Car Racer，但未看图或验证运行。没有镜像版本、反编译输出、物理公式、差分检查、帧率或公开代码；480函数不证明全部识别正确，TRACE也保持作者疑点而非确定反调试结论。没有给Gemini版本或可运行完成度，按进行中保存研究及工具失败边界。本合集未取得ROM、运行游戏或复现。

候选0赞、11浏览、0转发；480函数为作者报告，不是覆盖率。

## 来源

- [Scientific Brad的Amiga／REA／Ghidra／Gemini进度，2026-10-31](https://x.com/i/status/2116545601987096930)

[English](en/stunt-car-racer-amiga-rea-ghidra-gemini.md) | [返回目录](../README.zh-CN.md)
