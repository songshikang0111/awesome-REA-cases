# PSP Dock：David复用FUSA，在存储／手柄间切换并同步PPSSPP存档

分类：硬件与设备互通 · 未确认使用 REA
记录日期：2026-11-04
阶段：相关项目

2026年11月4日07:08:48（北京时间），David（@bitcoinpendium）称想为AI逆向浪潮做点东西，拿出旧PSP做类似Switch的停靠体验，不再反复换线。补读同串07:08:49至07:08:56的作者说明：USB先同步游戏与存档，再把PSP变为PC上PPSSPP的手柄，结束后切回存储把存档传回；难点是免拔线切换USB存储和HID。项目复用FUSA及其他工程，PC端Next.js界面仿XMB，下层沿用PPSSPP，不是PSP原生视频输出升频。

作者称项目名PSP Dock、Windows已做，Linux、Android TV及其他模拟器是未来计划，并称开放源码但不授商业权利。本合集只读原串，未核对仓库、许可证或观看录像；不能将口语open source解释为已核查OSI许可。具体模型、提示与新增逆向方法未披露，REA未知，故列设备互通相关项目而非AI独立破解。没有同步可靠性、冲突恢复、性能或设备兼容测试，未连接掌机或运行游戏，须自备合法游戏。补充原串用于解释本候选，不另算候选。

11月4日候选快照1赞、201浏览、0转发；原串补充不是运行验收。

## 来源

- [David的PSP Dock原帖，2026-11-04](https://x.com/i/status/2117755905681076381)
- [同日作者补充：USB存储／HID切换和复用FUSA](https://x.com/i/status/2117755924601315532)
- [同日作者补充：名称、Windows及未来平台、非商业说法](https://x.com/i/status/2117755928825241825)

[English](en/david-psp-dock-usb-save-hid-ppsspp.md) | [返回目录](../README.zh-CN.md)
