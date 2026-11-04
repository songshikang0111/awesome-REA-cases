# SMK-37固件：Sofia用Claude缩小Lean运行时并接杰理编译器

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-04
阶段：相关项目

2026年11月4日04:13:59（北京时间），Sofia（@algebraic_dev）称Claude主要帮助编写较小的Lean运行时，使用固定内存池，并写脚本调用杰理编译器。Genkigenki把fm-1固件felucca-bsp移植到SMK-37的项目让整合变得容易。用途是把语言运行时接到已有设备固件环境，不把上游移植归给Claude。

补取原帖确认账号与表述，未取得运行时源码、上游仓库、设备规格、编译输出或实测。原文未明说反编译或协议恢复，按设备互通相关项目收录；不推断内存用量、实时性能、机型覆盖或Lean证明正确性。REA未提及，未安装编译器或运行固件。

11月4日候选快照0赞、38浏览、0转发；无内存大小或性能数据。

## 来源

- [Sofia解释Claude与SMK-37整合分工，2026-11-04](https://x.com/i/status/2117711909260820979)

[English](en/smk37-claude-lean-runtime-firmware-port.md) | [返回目录](../README.zh-CN.md)
