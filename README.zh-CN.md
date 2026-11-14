<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

[English](README.md) | **简体中文**

### 用 AI 读懂软件与硬件。

精选 **AI 辅助逆向的项目、实验与具体想法**：让设备互通，重建应用，保存游戏，也记录失败尝试与作者对旧结论的更正。

# 2236 个案例与项目

**最近案例更新：**2026 年 11 月 14 日 12:08 · **最近维护：**2026 年 11 月 14 日 12:08 · 北京时间（UTC+8）；数量统计截至此次维护，来源日期与连续证据截止另行标明。

**每天更新 6 次** · [完整目录](INDEX.md) · [按分类浏览](#分类浏览)

覆盖 [REA](https://github.com/morluto/rea) 与其他 AI 辅助逆向。REA 通过 CLI / MCP，让编程 Agent 调用本地逆向工具。

*据作者与项目报告整理，未经本合集独立复现；证据与项目状态见各案例详情。*

![案例每日累计收录量](assets/case-growth.zh.svg)

## 近期精选

**10 个值得读的案例**：探测设备，恢复游戏行为，把主张与项目测试放在一起看。优先看具体用途与可见的证据边界，不靠泛泛的能力承诺。下列日期为来源或作者更新日期，不是收录日期。

1. **[Ember恒温杯：探测蓝牙，做自己的控制端](cases/dmitriy-ember-mug-codex-bluetooth-probing-report.md)** · `2026-11-14`作者报告 — Dmitriy称**Codex探测特征并与iOS应用对照**，约一小时做出温度／灯控制。禁止查网是作者要求，不是独立隔离证明；杯量精度与代码未核。`未独立核验`
2. **[富士X half：不用手机，照片直达Mac](cases/fujifilm-x-half-opus-wireless-mac-import-report.md)** · `2026-11-12`作者报告 — **Opus据报找到蓝牙／Wi-Fi协议差异**，做出JPEG导入和Google Photos上传。逐步实机试验，不是无迭代生成；代码与抓包未审。`未独立核验`
3. **[Anker录音豆：让Agent找回上周的对话](cases/berryxia-anker-recorder-rea-mcp-knowledge-app.md)** · `2026-11-12`作者报告 — **REA蓝牙研究与MCP录音检索**，可选千问本地ASR或在线转写。Berryxia计划调整测试后开源；代码与设备链路未核。`进行中`
4. **[Fallout Van Buren：把六年研究交给REA](cases/fallout-van-buren-kran-rea-human-guided-reconstruction.md)** · `2026-11-14`作者串 — Kran明确归功于**人工研究、shenmarukai初始反编译与IDA数据库**，不是Agent从零发现。Adam报告DX9迁移，64位仍是目标；研究对象是技术演示，不是完整游戏。本合集未构建。`进行中`
5. **[Windows95旅鼠：匹配函数，不夸大整包](cases/lemmings-win95-human-led-ai-reconstruction-report.md)** · `2026-11-12`介绍；`2026-11-09`固定文档 — 人类定架构，REA／Claude／Codex辅助，项目自报**八模块696／696函数匹配**。整EXE／DLL仍有差异，现代可移植构建与原编译器匹配分开；自备游戏资产，本合集未构建。`进行中`
6. **[decompdecomp：字节匹配，也保留汇编兜底](cases/decompdecomp-local-agent-byte-matching-workbench.md)** · `2026-11-14`介绍；`2026-11-13`固定文档 — **Agent写C／C++，原编译器按字节判定。**独立续接decomp.wtf，文档明确尚无整款游戏完成；导出保留汇编，所选云模型可能收到游戏材料。本合集未运行。`进行中`
7. **[ZigZag：把SVG送进Brother刺绣机](cases/kath-korevec-brother-chatgpt-embroidery-report.md)** · `2026-11-13`介绍与固定文档 — **Skitch PP1蓝牙上传与MCP辅助设计**，项目报告实机测试。NOTICE把协议归于Respira；早先ChatGPT起源故事仍是二手转述，不是独立发现。未运行。`未独立核验`
8. **[MousePods：AirPods在Linux当鼠标与头追](cases/airpods3-claude-remotehid-linux-head-mouse-report.md)** · `2026-11-11`报道；`2026-11-10`固定文档 — **Claude辅助RemoteHID研究与自报AirPods 3／Pro 2实机检查。**不刷耳机，但Proton接入会改前缀。MTU／设备身份影响未隔离，本合集未运行。`未独立核验`
9. **[智能拼豆板：从APK到树莓派控制端](cases/smart-bead-board-claude-raspberry-pi-mcp-control-report.md)** · `2026-11-14`作者报告与澄清 — Labelray称**Claude反编译官方APK找协议**，再写MCP工具按需点亮位置，不用原App。板子型号、连接方式与代码未披露，本合集未实机测试。`未独立核验`
10. **[TimeSplitters 2：把PS2行为追进PC版](cases/destinity-timesplitters2-claude-native-pc-recompile.md)** · `2026-11-10`作者报告；`2026-11-09`固定文档 — **Claude辅助MIPS到C++，以PCSX2画面／状态对照**，自报Linux／Steam Deck首关通关。仍用PCSX2图形／音频，后续关卡与互联网联机待测；自备光盘，本合集未构建。`进行中`

## 经典案例

- **[Universal Modder](cases/universal-modder.md)** — AI 辅助跨游戏 Mod，把 Minecraft 内容放进 GTA V 等游戏。
- **[Firefighter：DOS 二进制到 Rust](cases/firefighter-rust.md)** — 作者报告先恢复 Pascal 逻辑，再转写为 Rust。
- **[《现代战争 2》](cases/mw2-decompilation.md)** — 作者报告多 Agent 重建，**83% 函数字节级匹配**；代码未公开，未独立复现。
- **[Mac 菜单栏控制智能马桶](cases/smart-toilet.md)** — 作者报告研究蓝牙通信，并扩展到其他家居设备。
- **[Apple TV 遥控器接入 Linux](cases/siri-remote-linux.md)** — 蓝牙互通与公开实现，未确认使用 REA。
- **[Plustek 扫描仪与 ThinkPad 相机](cases/schaller-opticfilm-thinkpad-linux.md)** — 用Windows参考行为改善Linux驱动，公开测量仍保留低光与曝光缺陷。
- **[LG PlxNative](cases/lg-plxnative.md)** — 原生 Plex 客户端；作者报告用户选择时间从 **30 秒降到 3 秒**。

## 分类浏览

| 分类 | 数量 |
| :--- | ---: |
| [游戏与游戏保存](categories/games.md) | **444** |
| [硬件与设备互通](categories/hardware.md) | **596** |
| [应用与客户端](categories/apps.md) | **930** |
| [算法与功能重建](categories/algorithms.md) | **266** |

[**查看全部案例 →**](INDEX.md) · [贡献案例](CONTRIBUTING.md) · [维护方法](MAINTENANCE.md)

<details>
<summary><strong>更新时间与证据说明</strong></summary>

- **连续已解决材料的证据截止：**2026 年 10 月 15 日 16:00，北京时间。往期未解决来源会使截止时间暂缓，较新的案例仍可收录；这不是每个项目的验证日期。
- 每天检索 6 次，受关键词和分页限制，属于有界覆盖，不代表全网全量，部分链接证据仍待核实。来源日期、证据边界与热度快照见各案例详情。
- 每个案例均提供完整介绍、公开来源及中英文切换。

</details>

## 范围与许可

**非 REA 官方项目。**只整理原创摘要与公开链接，不分发原软件、游戏资产、密钥或私人材料。

原创整理与代码采用 **[MIT](LICENSE)**。链接内容保留各自权利；研究和复现请使用合法取得的目标，并确认相应授权。
