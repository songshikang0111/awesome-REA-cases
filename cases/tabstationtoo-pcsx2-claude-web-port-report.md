# TabStationToo：Claude协作把PCSX2与四类JIT带进浏览器

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-10-30
阶段：进行中

2026年10月30日08:24:51（北京时间），不吃泡面（@paomiange1）介绍TabStationToo，称两位开发者用Claude把开源PS2模拟器PCSX2移至浏览器，人工定架构与跑测试、模型承担替换代码。它是已有模拟器的跨平台适配，不是从零逆向PS2，也不能抹去PCSX2团队二十多年的工作。两人分工仍为转述，未取得完整开发记录。

补读固定提交c53f021af984438cd1fe07114f9710af77f5f4bd的README；提交时间10月30日04:36:17北京时间，早于本窗口，只作补证。该提交说明Tekken Tag Tournament在Chrome中从50%至87%的项目性能变化，并含Claude Opus 5.5协作署名；这支持AI参与，但不是其独自完成整套工程的证明。README明确early and experimental，描述Emscripten编译的PCSX2核心、SharedArrayBuffer线程，以及EE、IOP、VU0、VU1四类运行时WebAssembly JIT，声称与解释器逐位核对。WebGPU硬件渲染有软件回退，声音走Web Audio。

项目报告Chrome中GTA San Andreas步行平均约99%、Final Fantasy XII过场100%、Guitar Hero歌曲100%偶有下降；这些是特定场景的模拟速度，不是所有游戏满帧、也不是统一帧率。较重WWE场景需Ryzen7 7840U全功率；Linux省电策略曾造成50%至60%的误读，且多数Linux Chromium GPU默认不开WebGPU。支持手柄、浏览器记忆卡和每游戏最多十份即时存档，但手机、带parent的CHD和多文件BIN/CUE仍不支持。没有独立重跑JIT差分或性能测试。

用户须合法自备PS2 BIOS与游戏镜像；README说这些文件留本地，但封面会向ps2-covers发外部请求，因此不是页面绝无联网。需跨源隔离部署，不能把从磁盘打开HTML当可用方式。本合集只静态阅读公开文档与提交，没有下载BIOS/游戏、安装依赖或运行移植，不将项目验证升级为独立复现。

候选快照1赞、36浏览、0转发；未把宣传热度当技术验证。
固定提交2026-10-29T20:36:17Z；99%/100%为项目限定场景模拟速度，未独立测量。

## 来源

- [不吃泡面转述TabStationToo与Claude分工，2026-10-30](https://x.com/i/status/2115963106681909434)
- [窗口前固定README：实验状态、架构、测试范围与本地文件限制](https://github.com/TabStationToo/TabStationToo/blob/c53f021af984438cd1fe07114f9710af77f5f4bd/README.md)
- [窗口前提交：Tekken性能自述与Claude Opus协作署名](https://github.com/TabStationToo/TabStationToo/commit/c53f021af984438cd1fe07114f9710af77f5f4bd)

[English](en/tabstationtoo-pcsx2-claude-web-port-report.md) | [返回目录](../README.zh-CN.md)
