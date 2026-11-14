<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

[English](README.md) | **简体中文**

### 用 AI 读懂软件与硬件。

精选 **AI 辅助逆向的项目、实验与具体想法**：让设备互通，重建应用，保存游戏，也记录失败尝试与作者对旧结论的更正。

# 2249 个案例与项目

**最近案例更新：**2026 年 11 月 14 日 20:15 · **最近维护：**2026 年 11 月 14 日 20:15 · 北京时间（UTC+8）；数量统计截至此次维护，来源日期与连续证据截止另行标明。

**每天更新 6 次** · [完整目录](INDEX.md) · [按分类浏览](#分类浏览)

覆盖 [REA](https://github.com/morluto/rea) 与其他 AI 辅助逆向。REA 通过 CLI / MCP，让编程 Agent 调用本地逆向工具。

*据作者与项目报告整理，未经本合集独立复现；证据与项目状态见各案例详情。*

![案例每日累计收录量](assets/case-growth.zh.svg)

## 近期精选

**10 个值得读的案例**：控制自己的设备，保存老工具与游戏，也看清测试究竟证明了什么。下列日期为来源或作者更新日期，不是收录日期。

1. **[borland-reborn：重建1991年的编译器](cases/borland-reborn-bcc20-exhume-byte-matching.md)** · `2026-11-14`介绍与固定文档 — Exhume的Claude Code skills辅助，项目报告**BCC.EXE／CPP.EXE整文件字节一致**。另有改版构建的1836次编译对照、83%覆盖，不代表所有路径或唯一原始源码。本合集未重建。`未独立核验`
2. **[Ember恒温杯：探测蓝牙，做自己的控制端](cases/dmitriy-ember-mug-codex-bluetooth-probing-report.md)** · `2026-11-14`作者报告 — Dmitriy称**Codex探测特征并与iOS应用对照**，约一小时做出温度／灯控制。禁止查网是作者要求；杯量精度与代码未核。`未独立核验`
3. **[富士X half：不用手机，照片直达Mac](cases/fujifilm-x-half-opus-wireless-mac-import-report.md)** · `2026-11-12`作者报告 — **Opus据报找到蓝牙／Wi-Fi差异**，做出JPEG导入和Google Photos上传。逐步实机试验，不是无迭代生成；代码与抓包未审。`未独立核验`
4. **[Anker录音豆：让Agent找回上周的对话](cases/berryxia-anker-recorder-rea-mcp-knowledge-app.md)** · `2026-11-12`作者报告 — **REA蓝牙研究与MCP录音检索**，可选千问本地ASR或在线转写。计划调整测试后开源；代码与设备链路未核。`进行中`
5. **[Fallout Van Buren：把六年研究交给REA](cases/fallout-van-buren-kran-rea-human-guided-reconstruction.md)** · `2026-11-14`作者串 — Kran归功于**人工研究、shenmarukai反编译与IDA数据库**，不是Agent从零发现。已报告DX9迁移，64位仍是技术演示的目标，不是完整游戏。本合集未构建。`进行中`
6. **[Windows95旅鼠：匹配函数，不夸大整包](cases/lemmings-win95-human-led-ai-reconstruction-report.md)** · `2026-11-12`介绍；`2026-11-09`固定文档 — 人类定架构，REA／Claude／Codex辅助，自报**八模块696／696函数匹配**。整EXE／DLL仍有差异，现代构建与原编译器匹配分开；自备资产，本合集未构建。`进行中`
7. **[Mario Kart World：转译代码，也逐项测改动](cases/mkw-recomp-claude-aarch64-c-port.md)** · `2026-11-14`介绍与固定文档 — **Claude辅助AArch64转C、同次运行A/B与原机图对照**，项目报告PC比赛可跑。不是原始源码恢复；菜单、AMD挂起与无在线联机仍有限制。自备游戏，本合集未构建。`进行中`
8. **[Donkey Kong Bananza：把Switch2游戏带到PC](cases/dkb-pc-recomp-claude-switch2-port.md)** · `2026-11-14`介绍；`2026-11-13`固定文档 — **Claude Code工作以游戏运行和Unicorn对照检查**，建立于TotK Recomp及社区着色器研究。GPU崩溃、后段缺陷仍在，Linux／macOS为预览。自备游戏，本合集未构建。`进行中`
9. **[decompdecomp：字节匹配，也保留汇编兜底](cases/decompdecomp-local-agent-byte-matching-workbench.md)** · `2026-11-14`介绍；`2026-11-13`固定文档 — **Agent写C／C++，原编译器按字节判定。**尚无整款游戏完成的报告；导出保留汇编，云模型可能收到游戏材料。本合集未运行。`进行中`
10. **[智能拼豆板：从APK到树莓派控制端](cases/smart-bead-board-claude-raspberry-pi-mcp-control-report.md)** · `2026-11-14`作者报告与澄清 — Labelray称**Claude反编译官方APK找协议**，再写MCP工具按需点亮位置，不用原App。型号、连接方式与代码未披露，本合集未实机测试。`未独立核验`

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
| [游戏与游戏保存](categories/games.md) | **449** |
| [硬件与设备互通](categories/hardware.md) | **597** |
| [应用与客户端](categories/apps.md) | **936** |
| [算法与功能重建](categories/algorithms.md) | **267** |

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
