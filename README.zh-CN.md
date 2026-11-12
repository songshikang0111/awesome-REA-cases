<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

[English](README.md) | **简体中文**

### 用 AI 读懂软件与硬件。

精选 **AI 辅助逆向的项目、实验与具体想法**：让设备互通，重建应用，保存游戏，也记录失败尝试与作者对旧结论的更正。

# 2156 个案例与项目

**最近案例更新：**2026 年 11 月 13 日 00:15 · **最近维护：**2026 年 11 月 13 日 00:15 · 北京时间（UTC+8）；数量统计截至此次维护，来源日期与连续证据截止另行标明。

**每天更新 6 次** · [完整目录](INDEX.md) · [按分类浏览](#分类浏览)

覆盖 [REA](https://github.com/morluto/rea) 与其他 AI 辅助逆向。REA 通过 CLI / MCP，让编程 Agent 调用本地逆向工具。

*据作者与项目报告整理，未经本合集独立复现；证据与项目状态见各案例详情。*

![案例每日累计收录量](assets/case-growth.zh.svg)

## 近期精选

**10 个值得读的案例**：让设备互通，读懂不透明应用，也保存游戏；还看一块手表如何绕开部分限制、又留下哪些共用问题。下列日期为来源或作者更新日期，不是收录日期。

1. **[富士X half：不用手机，照片直达Mac](cases/fujifilm-x-half-opus-wireless-mac-import-report.md)** · `2026-11-12`作者报告 — **Opus据报找到蓝牙／Wi-Fi协议差异**，做出JPEG导入和Google Photos上传。逐步实机试验，不是无迭代生成；代码与抓包未审。`未独立核验`
2. **[Anker录音豆：让Agent找回上周的对话](cases/berryxia-anker-recorder-rea-mcp-knowledge-app.md)** · `2026-11-12`作者报告 — **REA蓝牙研究与MCP录音检索**，可选千问本地ASR或在线转写。Berryxia计划调整测试后开源；代码与设备链路未核。`进行中`
3. **[Windows95旅鼠：匹配函数，不夸大整包](cases/lemmings-win95-human-led-ai-reconstruction-report.md)** · `2026-11-12`介绍；`2026-11-09`固定文档 — 人类定架构，REA／Claude／Codex辅助，项目自报**八模块696／696函数匹配**。整EXE／DLL仍有差异，现代可移植构建与原编译器匹配分开；自备游戏资产，本合集未构建。`进行中`
4. **[hexgrab：研究PowerToys，再做小取色器](cases/hexgrab-powertoys-colorpicker-rea-study.md)** · `2026-10-29`报道；`2026-10-12`研究 — Claude／REA调查二进制，作者对照源码得出**九项八项正确、一项部分正确**。另一个二进制负责热键注册，暴露盲点。公开.NET10实现，只测单屏，本合集未重跑。`分析测试`
5. **[REA检查自己的应用：发布前看暴露面](cases/phosphen-rea69-own-app-exposure-gate-test.md)** · `2026-11-12`作者自测 — Phosphen报告source map源码和Stripe键，以及发布门禁**修复前退出3、修复后0**。样本与日志未审；不证明键可用或每项发现都是泄漏。`分析测试`
6. **[MousePods：AirPods在Linux当鼠标与头追](cases/airpods3-claude-remotehid-linux-head-mouse-report.md)** · `2026-11-11`报道；`2026-11-10`固定文档 — **Claude辅助RemoteHID研究与自报AirPods 3／Pro 2实机检查。**不刷耳机，但Proton接入会改前缀。MTU／设备身份影响未隔离，本合集未运行。`未独立核验`
7. **[Garmin Profile2：共用手表，不是双系统档案](cases/garmin-forerunner955-claude-profile2-workaround.md)** · `2026-11-12`作者报告 — Claude研究Forerunner955限制后，改走官方应用平台，**自报心率、计时、GPS可用**。没有修改固件，步数、睡眠与全天心率仍混合；代码与隔离效果未核。`进行中`
8. **[NEAR Signer：让iPhone说Ledger协议](cases/near-signer-ios-ledger-ble-ai-report.md)** · `2026-11-12`报道与固定文档 — AI协作开发，自报**128个Swift、14个Python测试通过**。BLE只测模拟器，真实iPhone配对、相机和Xcode构建未核；应用中加密私钥不等同Ledger安全芯片。`进行中`
9. **[TimeSplitters 2：把PS2行为追进PC版](cases/destinity-timesplitters2-claude-native-pc-recompile.md)** · `2026-11-10`作者报告；`2026-11-09`固定文档 — **Claude辅助MIPS到C++，以PCSX2画面／状态对照**，自报Linux／Steam Deck首关通关。仍用PCSX2图形／音频，后续关卡与互联网联机待测；自备光盘，本合集未构建。`进行中`
10. **[Empire Earth：重建引擎与原版一起联机](cases/empire-earth-ai-trailers-compatible-engine-report.md)** · `2026-11-12`介绍；`2026-11-08`固定文档 — 提交有Claude署名，项目报告**逐tick对照及原版／重建端TCP混合对局无失步**。整文件仍不同，WON服务、音频与物理输入未测；源码无通用许可授权，本合集未运行。`进行中`

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
| [游戏与游戏保存](categories/games.md) | **435** |
| [硬件与设备互通](categories/hardware.md) | **579** |
| [应用与客户端](categories/apps.md) | **886** |
| [算法与功能重建](categories/algorithms.md) | **256** |

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
