# Fireface UCX完整控制上Linux：Johan用REA与Claude研究Windows驱动，逐项接线实测

分类：硬件与设备互通 · REA
记录日期：2026-11-15
阶段：待验证

2026年11月15日20:42:10（北京时间），Choblin（@choblin29）转述RME Fireface UCX的Linux驱动项目，随后回复给出Johan Yngman同日文章。UCX本来能在Class Compliant模式下提供18路输入输出，问题不是Linux完全不能用它，而是DSP混音、EQ、动态和混响等设置仍依赖Windows TotalMix FX。

补读作者日期为11月15日的原文：Johan称让Claude Code通过REA调用Ghidra与rizin，阅读Windows驱动、追USB请求、音频流设置和推子指令；发现混音指令沿用社区早已记录的RME FireWire格式，明确感谢snd-firewire-ctl-services与oscmix，不把全部协议发现归给AI。作者说代码全由Claude写，但自己决定声明式配置设计、推动fuzz、clang-tidy与sanitizer，并花约一周移动线缆、低音量回环测试、观察设备电平、断电与睡眠恢复。这不是无人干预的一次生成。

文章报告snd-fireface-ucx内核驱动、ucxtui终端混音器和ucxcfg JSON配置工具，声称18通道、32—192kHz、两个MIDI口、路由、EQ、动态、混响与回声，以及48kHz经PipeWire往返3.5ms。以上均为作者结果，未读取原始延迟测量日志；文章明确仅测试一台第一代UCX，不推广到UCX II或全系列。作者链接realbogart/fireface-ucx-linux并称MIT；本合集未审完整源码或许可、安装驱动、运行目标或连接硬件，保持unverified。

主候选封存2赞、499浏览、0转发、4回复；回复0赞、165浏览。约一周为作者开发／测试经历，不是纯AI工时。
3.5ms是48kHz经PipeWire的作者往返测量；测试样本为一台第一代UCX。

## 来源

- [Choblin转述UCX驱动与人工测试，2026-11-15 20:42:10北京时间](https://x.com/i/status/2121946863523987476)
- [同串候选回复给出的作者原文链接，20:42:12](https://x.com/i/status/2121946868976660569)
- [补读Johan Yngman原文，页面日期2026-11-15：REA方法、单台测试与3.5ms自报](https://johanyngman.com/fireface-ucx-on-linux-reverse-engineered-and-built-with-claude-code.html)

[English](en/johan-fireface-ucx-linux-rea-claude-driver.md) | [返回目录](../README.zh-CN.md)
