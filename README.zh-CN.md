<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

[English](README.md) | **简体中文**

### 用 AI 读懂软件与硬件。

精选 **AI 辅助逆向的项目、实验与具体想法**：让设备互通，保留旧行为重建应用，保存游戏，也记录失败尝试与作者对旧结论的更正。

# 2528 个案例与项目

**最近案例更新：**2026 年 11 月 20 日 16:08 · **最近维护：**2026 年 11 月 20 日 16:08 · 北京时间（UTC+8）；数量统计截至此次维护，来源日期与连续证据截止另行标明。

**每天更新 6 次** · [完整目录](INDEX.md) · [按分类浏览](#分类浏览)

覆盖 [REA](https://github.com/morluto/rea) 与其他 AI 辅助逆向。REA 通过 CLI / MCP，让编程 Agent 调用本地逆向工具。

*据作者与项目报告整理，未经本合集独立复现；证据与项目状态见各案例详情。*

![案例每日累计收录量](assets/case-growth.zh.svg)

## 近期精选

**10 个值得读的案例**：重建旧二进制，查询已有电路，分享游戏，让设备更好用。精选优先展示具体方法与可检验的主张，而非宽泛承诺；完整目录也保留早期 idea 与失败尝试。下列日期为来源或作者更新日期，不是收录日期。

1. **[borland-reborn：重建1991年的编译器](cases/borland-reborn-bcc20-exhume-byte-matching.md)** · `2026-11-14`介绍与固定文档 — Exhume的Claude Code skills辅助，项目报告**BCC.EXE／CPP.EXE整文件字节一致**。另有改版构建的1836次编译对照、83%覆盖，不代表所有路径或唯一原始源码。本合集未重建。`未独立核验`
2. **[Proteus：让Claude回答已有电路的问题](cases/arpit-proteus-pdsprj-mcp-project-research.md)** · `2026-11-17`作者串 — Arpit研究**未文档化.pdsprj，制作MCP桥接**，报告可查原理图、追连线、改参数与生成物料清单。放元件和布线仍待做，无头仿真不返回波形。已读串文，未测代码与电路。`进行中`
3. **[Darmoshark TOP75：在Mac控制键盘](cases/darmoshark-top75-macos-ai-protocol-report.md)** · `2026-11-18`作者回复与固定文档 — **AI辅助研究Windows工具，再用IOKit实机检查**，支持蓝牙RGB、改键、宏与定时熄灯。项目文档记录读回、回退和丢写；显示上传走USB，GIF机上播放仍待验证。本合集未测试。`未独立核验`
4. **[Horizon：用Rust重建Minecraft Java行为](cases/horizon-minecraft-java-rust-ai-differential-reimplementation.md)** · `2026-11-16`介绍与固定文档 — **AI辅助重建，自报281套差分测试**，可读旧存档、连原版服务器。已读公开文档与Codex署名提交，未审完整测试结果；性能宣称有硬件条件。自备游戏，本合集未构建。`进行中`
5. **[Underworld Exhumed：保存两部DOS地下世界](cases/underworld-exhumed-ultima-claude-skills-byte-matching.md)** · `2026-11-20`介绍；`2026-11-17`固定文档 — Exhume的Claude Code技能辅助，项目报告**UW.EXE／UW2.EXE整文件字节一致**，原生与Web移植以17／13段DOS录制回放检查。均为项目报告，本合集未重跑；原生版自备游戏数据。`未独立核验`
6. **[rust-anything：重建Prettier，不猜输出](cases/rust-anything-claude-behavior-capture-rust-migration.md)** · `2026-11-20`介绍与固定文档 — Agent按录制行为写Rust，项目报告**17224次字节一致，仅15837次全在Rust**，其余回退Prettier。所列M4测试中CLI约19倍含进程启动优势，预热进程内为4.2倍；本合集未重跑。`未独立核验`
7. **[DecBench：反编译的“精确”究竟测什么？](cases/decbench-llm-decompiler-exactness-benchmark.md)** · `2026-11-19`介绍；`2026-11-11`固定文档 — 分别比较**控制流、类型与归一化重编译**。Union是任一指标完美，不是三项同时正确或整文件字节一致；还有fixup修正，未核实时榜单或运行基准。`分析测试`
8. **[X6200：更新电台，不必换回原厂系统](cases/x6200-claude-base-firmware-upgrade-reimplementation.md)** · `2026-11-16`介绍与PR合并 — **Claude辅助重建Xiegu升级流程**，已进入OpenX6X00。项目CI通过，作者报告单台升级与回退；无法读回flash，恢复未实机测试，本合集未复现。`未独立核验`
9. **[NotTheInstagram：给无限刷加一点阻力](cases/nottheinstagram-rea-codex-flex-friction-hooks.md)** · `2026-11-15`作者文章与固定代码 — **FLEX给Codex地图，REA连接Hopper**找hook，实现每三帖等待与Reels入口两分钟暂停的自述。源码可见签名检查，实机细项仍未全确认；仅报告测试Instagram455.0.0，修改客户端有风险。`未独立核验`
10. **[Kirby到PPSSPP：让homebrew复用GameShare](cases/xitrix-kirby-rea-gameshare-ppsspp-homebrew.md)** · `2026-11-20`作者串 — XITRIX称**REA找出Kirby启动系统SDK的调用**，再用于把第二个PPSSPP实例分享给另一台Switch。是具体互通报告，不是找回整部Kirby源码；未核验API代码、演示与主机。`未独立核验`

## 经典案例

- **[Universal Modder](cases/universal-modder.md)** — AI 辅助跨游戏 Mod，把 Minecraft 内容放进 GTA V 等游戏。
- **[Firefighter：DOS 二进制到 Rust](cases/firefighter-rust.md)** — 作者报告先恢复 Pascal 逻辑，再转写为 Rust。
- **[《现代战争 2》](cases/mw2-decompilation.md)** — 作者报告多 Agent 重建，**83% 函数字节级匹配**；代码未公开，未独立复现。
- **[Mac 菜单栏控制智能马桶](cases/smart-toilet.md)** — 作者报告研究蓝牙通信，并扩展到其他家居设备。
- **[Apple TV 遥控器接入 Linux](cases/siri-remote-linux.md)** — 蓝牙互通与公开实现，未确认使用 REA。
- **[Plustek 扫描仪与 ThinkPad 相机](cases/schaller-opticfilm-thinkpad-linux.md)** — 用Windows参考行为改善Linux驱动，公开测量仍保留低光与曝光缺陷。
- **[Fireface UCX接Linux](cases/johan-fireface-ucx-linux-rea-claude-driver.md)** — Johan报告REA／Claude研究驱动、终端混音器与**48kHz往返3.5ms**，仅一台第一代设备，本合集未复现。
- **[LG PlxNative](cases/lg-plxnative.md)** — 原生 Plex 客户端；作者报告用户选择时间从 **30 秒降到 3 秒**。

## 分类浏览

| 分类 | 数量 |
| :--- | ---: |
| [游戏与游戏保存](categories/games.md) | **495** |
| [硬件与设备互通](categories/hardware.md) | **668** |
| [应用与客户端](categories/apps.md) | **1056** |
| [算法与功能重建](categories/algorithms.md) | **309** |

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
