# sh4vita：Claude／Codex辅助把《寂静岭4》PC版静态重编译到PS Vita

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-10-31
阶段：进行中

2026年10月31日02:25:06（北京时间）的候选介绍sh4vita，将Konami的Silent Hill 4: The Room从GOG PC版带到PS Vita，称Claude和Codex协助逆向与编码、开发者在真实Vita上测试，并转述v1.0.1修复长局崩溃。补查找到vallfrr/sh4vita，阅读固定提交386541b726538a50f2e3cdf48d5ac24b553d6239的README；该提交为2026-10-30T09:57:00Z，早于候选，仅作项目背景与限制的补充，不另算窗口候选。

文档解释流程：Ghidra导出函数列表，recomp/x86rec.py将x86函数转为C，再与替代Win32、Direct3D8、DirectInput和DirectSound的运行时编译；D3D8建立在vitaGL上。Rust编写的独立sh4prep准备玩家自己的游戏文件。项目明确Claude与Codex用于研究和代码，设计决定及真实硬件验证由人完成；未称REA参与。

README报告实机从头到尾可玩，逻辑30fps，性能允许时插值渲染趋近60fps；敌人密集地铁、水牢和部分后期房间仍CPU受限、可低于30fps。首次进房可停约一秒，一小时以上长局仍可能内存不足、丢纹理甚至关闭；Continue灰显须用Load，光晕效果为性能关闭。因此不把候选的1.0.1修复写成所有长局崩溃已消失，也不称恒定60fps。

只支持GOG“1.0 gog v5”Windows文件，其他版本及PS2文件不行；需改机Vita、至少4GB空间和用户自己的shader编译模块。项目代码GPLv3，游戏和生成C不随仓库提供；GPL不授予Konami资产权利。这里只静态阅读公开文档，未下载游戏、运行准备器、安装VPK、实测帧率或独立通关。

候选快照0赞、80浏览、0转发；通关、帧率和修复均为项目／报道说法，未独立复现。
补充固定提交2026-10-30T09:57:00Z早于窗口；保留长局内存限制。

## 来源

- [候选转述sh4vita、AI协助及1.0.1修复，2026-10-31 02:25:06](https://x.com/i/status/2116234958109122747)
- [补充：10月30日固定README，方法、AI归因与尚存实机限制](https://github.com/vallfrr/sh4vita/blob/386541b726538a50f2e3cdf48d5ac24b553d6239/README.md)

[English](en/sh4vita-silent-hill4-claude-codex-static-port.md) | [返回目录](../README.zh-CN.md)
