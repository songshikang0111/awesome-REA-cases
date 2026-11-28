# Open Ultima 8 v0.5.8：Claude辅助Rust重建《创世纪VIII》引擎的转述

分类：游戏与游戏保存 · 其他 AI 逆向
记录日期：2026-11-28
阶段：待验证

2026年11月28日08:56:55（北京时间），The Gaming Emporium（@TheEmporium83）介绍fswolf（Beerus）的Open Ultima 8 v0.5.8：以Rust重建Origin Systems于1994年推出的RPG Ultima VIII: Pagan引擎，让旧DOS游戏在Windows、Linux、macOS与Steam Deck原生运行。帖子明确将开发与逆向归为Claude辅助；Claude具体模型与参与比例仍未核实，REA未提及。

介绍称新引擎使用原地图、资产、脚本与玩法逻辑而不依赖DOS模拟，支持宽屏、分辨率调整、1至8倍缩放、xBR／xBRZ／CRT滤镜和平滑镜头，输入包括键鼠、手柄、触屏及Steam Deck／ROG Ally控制。还称原DOS与新引擎存档互通，保留任务、谜题、对话、战斗、四系魔法和过场，另有书卷阅读、环境音量、快速存读、生命／法力显示、Discord整合与可选开发者作弊功能。发帖者将整部游戏可玩归因开发者，同时明确仍需测试差异；这些不是本合集实玩结果。

补读窗口前11月27日16:48:22北京时间提交683a91f01eed78e353c567153ed1990a732b3fb1的README，确认fswolf/open-ultima8公开项目及上述多数功能的文档。它将已知文件格式与引擎知识明确归功Pentagram、ScummVM，不是AI独立从零发现。原游戏数据不分发，须自备GOG或原CD；U8.EXE仍需保留以读取武器表。存档使用原格式并备份首次覆盖的原槽位，但成长进度、饥饿、挂在边缘等原格式无处存的状态放在.ou8 sidecar，不能把“互通”扩成全部状态双向等价。音乐需要另备SoundFont，缺少时无音乐；Mac应用未公证。

文档说nearly the whole game，列有意改变镜头、字体、环境音、跨楼层声音等；可选恢复遗失内容默认关闭，部分剧情时限为新引擎选择。它列无游戏数据测试及需U8_DATA的原数据测试命令，但没有本合集读过的逐项运行结果。这里只读固定文档，未审完整源码、发布包或开发轨迹，未运行游戏或存档往返测试，不确认v0.5.8全部内容、无模拟、全平台可用或行为完全等价，保持unverified。

候选封存20赞、524浏览、2转发、0回复；可玩性和功能为二手项目报告，不是独立复现。

## 来源

- [The Gaming Emporium的Open Ultima 8 v0.5.8与Claude参与介绍，2026-11-28 08:56:55北京时间](https://x.com/i/status/2126480423610187950)
- [补充固定README：上游归属、原数据、存档与差异；提交2026-11-27 16:48:22北京时间，早于候选窗口](https://github.com/fswolf/open-ultima8/blob/683a91f01eed78e353c567153ed1990a732b3fb1/README.md)

[English](en/open-ultima8-rust-claude-engine-v058.md) | [返回目录](../README.zh-CN.md)
