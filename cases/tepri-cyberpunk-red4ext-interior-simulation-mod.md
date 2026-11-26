# 用Claude梳理Cyberpunk工具链：Tepri的室内空间与C++模拟Mod

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-26
阶段：进行中

2026年11月26日05:30:25（北京时间），Tepri（@tepri_x）解释一个第一人称游戏Mod的实现，性能敏感部分除redscript包装／钩子外主要用C++。其引用Claude的说明涉及WolvenKit资源编辑、redscript反编译脚本、Cyber Engine Tweaks、TweakXL／ArchiveXL，以及RED4ext与RTTI；据工具生态定位为Cyberpunk 2077相关Mod，不自行给Mod起产品名。作者称实际使用redscript游戏钩子、TweakXL记录、WolvenKit任务归档和RED4ext C++模拟。

补充同串05:03:47父帖称，以前会伪造任务触发、玩钩子和裁剪对话，现在AI让他能更完整控制世界状态，几乎所有室内空间已可进入。该父帖不是额外候选。Claude解释区分可读脚本、社区SDK已暴露接口与未反射／内联代码才需原生逆向；没有证据说明这个Mod具体执行过哪些原生反汇编，不能把社区工具的既有成果全部归给AI。未审代码、运行录像、地图覆盖或性能数据；开放范围和工作进展均为作者自述，本合集未运行游戏。

候选封存1赞、23浏览、0转发、2回复；性能是设计动机，非跑分结果。

## 来源

- [Tepri的Claude工具链说明与Mod实现，2026-11-26 05:30:25北京时间](https://x.com/i/status/2125703678841782607)
- [补充同串：AI帮助控制世界状态与开放室内空间，2026-11-26 05:03:47北京时间](https://x.com/i/status/2125696977069580721)

[English](en/tepri-cyberpunk-red4ext-interior-simulation-mod.md) | [返回目录](../README.zh-CN.md)
