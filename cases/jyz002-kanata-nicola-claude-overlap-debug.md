# NICOLA拇指换挡输入：Claude辅助追查kanata宏交错，作者称608错误归零

分类：算法与功能重建 · 其他 AI 逆向
记录日期：2026-11-04
阶段：分析测试

2026年11月4日02:23:45（北京时间），@jyz002在Ubuntu26.04的MacBook9,1笔记中披露Claude Code辅助的NICOLA输入适配。NICOLA是日文拇指换挡输入方式；此处以kanata1.12.0和Mozc组合，Eisu／Kana轻触同时切kanata层并用Hangul_Hanja／Hangul单次启闭Mozc。作者将kanata置于专用加固systemd用户，而自己的用户不进input组。

作者称在kanata_simulated_input穷举双键对，识别两类乱码：误触Eisu层切换，以及最多四个宏并发使ka、ta交错为k t a。其修正分别限制为150ms内轻触且此前200ms无输出，以及只在紧接其他输出时延迟6ms，报告双键对608处错误降为0。测试范围不是所有真实打字情境，NICOLA三键规则仍不能用kanata配置表达。工具会看到所有按键，原帖明确警告风险；没有读取私人输入、运行配置或复测数字。与同帖声卡路径研究是独立目标，不将扬声器结果当输入测试证据。

1赞、25浏览、0转发的11月4日候选快照；608→0为作者双键对模拟测试。

## 来源

- [@jyz002的kanata／Mozc排错与未解三键规则，2026-11-04](https://x.com/i/status/2117684171720233121)

[English](en/jyz002-kanata-nicola-claude-overlap-debug.md) | [返回目录](../README.zh-CN.md)
