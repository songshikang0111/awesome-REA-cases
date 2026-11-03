# ro-mono-303：Claude辅助TB-303电路与固件研究，ROM音序器接模拟声部

分类：硬件与设备互通 · 其他 AI 逆向
记录日期：2026-11-03
阶段：进行中

2026年11月3日22:08:52（北京时间），候选祝贺@lemusdev发布ro-mono-303的Mac／Windows AU/VST3 beta，称用Claude Code研究Roland TB-303的电路与固件。TB-303是带音序器的低音合成器；目标是在音乐宿主中保留原机音序行为与模拟声部，不是只仿面板。AI归因来自候选转述，文档不能单独证明Claude承担了哪些分析。

补读Lemus公开仓库固定提交32b3e4961fded5e5298bea45c1c8e19717de499c，提交于同日17:58:40北京时间，早于候选窗口，只作实现背景。文档说音序器将原NEC uPD650C-133固件跑在由MAME核心移植的uCOM-43 CPU模拟器上，保留pattern RAM、按键、LED和CV／gate／accent／slide锁存；声部按服务电路图逐元件建模。顶层README给出AU、VST3和独立版构建，标early，代码AGPL-3.0，MAME CPU核心BSD-3-Clause；不能把CPU仿真写成全由AI从零开发。

TB-303 README自报16／16服务检查通过，并以一台真机400个单音作拟合与比较：log-spectral distance为3.0dB，真机自身重录2.4dB、Roland软件3.3dB。这是项目文档的测试口径，不是本合集重测，也不是所有机器与声音等价。已知前100ms亮度仍约有25%误差；不模拟MIX IN、CV／GATE输出、耳放及电池LED。

仓库不分发ROM或商标图；完整音序器须用户自备合法ROM，没有ROM仅MIDI声部模式、无音序器。部分真机录音与研究参考材料不公开，不能独立核验其对照。只静态阅读公开文档，未安装JUCE、构建插件、取得ROM或渲染音频。另有TR-909在补读文档出现，但不是本候选目标，不据此新增另一案例。

11月3日候选快照1赞、13浏览、0转发；16／16、400音符及误差均为项目报告，本合集未运行。

## 来源

- [候选转述ro-mono-303与Claude Code，2026-11-03](https://x.com/i/status/2117620026895405083)
- [补充：Lemus顶层README，固定提交2026-11-03 17:58:40北京时间](https://github.com/lemus-dev/lemus/blob/32b3e4961fded5e5298bea45c1c8e19717de499c/README.md)
- [补充：TB-303实现、验证与已知差异，同一固定提交](https://github.com/lemus-dev/lemus/blob/32b3e4961fded5e5298bea45c1c8e19717de499c/machines/tb303/README.md)

[English](en/ro-mono-303-claude-circuit-firmware-emulator.md) | [返回目录](../README.zh-CN.md)
