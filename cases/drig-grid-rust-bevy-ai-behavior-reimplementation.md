# DRIG：AI辅助把Race Driver: GRID行为重建到Rust与Bevy

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-28
阶段：进行中

2026年11月28日16:30:09（北京时间），yibie在列表更新中介绍DRIG：研究Codemasters的2008年赛车游戏Race Driver: GRID，以Rust和Bevy重建引擎，游戏数据由玩家自己的PC安装提供。候选同时介绍另一个Sonic 2006项目，两者是不同目标。

补读PipeKnight/drig-race-driver固定8b360088b4f250871d8380d564613ef0231e1fc2 README，提交2026年11月27日20:50:23 UTC、早于窗口。作者明确多数代码由AI编程Agent编写，并提到Claude订阅；研究grid.exe使用Ghidra等工具，再将行为写成Rust，以原版驾驶、AI、音频录制轨迹及个别例程的bit-exact对照检查。文档报告驾驶、赛事、损伤、职业与回放等已可用，但称仍是早期实验，可能崩溃、物理失控、缺功能或画面不同；部分回放音效仍缺。Linux仅报告WSLg测试，不等于原生Linux真机已测。

目标是一比一行为，不是已证明整游戏字节匹配。backlog完成比例和固定无头场景通过比例不涵盖全部画面、音频或交互赛事，文档亦保留未自动化驾驶场景。本合集只读文档，未构建、运行或重放测试。新版本文档称GPL-3.0-or-later，旧Apache 2.0版本保留旧条款；原游戏数据须合法自备，不由本合集分发。

候选快照0赞、176浏览、0转发、0回复；4005文件为介绍口径，不代表完成度。

## 来源

- [yibie介绍DRIG与Sonic 2006，2026-11-28 16:30:09北京时间](https://x.com/i/status/2126594483777323455)
- [窗口前固定README：AI归因、轨迹对照、状态与平台限制，2026-11-27 20:50:23 UTC](https://github.com/PipeKnight/drig-race-driver/blob/8b360088b4f250871d8380d564613ef0231e1fc2/README.md)

[English](en/drig-grid-rust-bevy-ai-behavior-reimplementation.md) | [返回目录](../README.zh-CN.md)
