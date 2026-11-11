<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

[English](README.md) | **简体中文**

### 用 AI 读懂软件与硬件。

精选 **AI 辅助逆向的项目、实验与具体想法**：让设备互通，重建应用，保存游戏，也记录失败尝试与作者对旧结论的更正。

# 2094 个案例与项目

**最近案例更新：**2026 年 11 月 12 日 00:14 · **最近维护：**2026 年 11 月 12 日 00:14 · 北京时间（UTC+8）；数量统计截至此次维护，来源日期与连续证据截止另行标明。

**每天更新 6 次** · [完整目录](INDEX.md) · [按分类浏览](#分类浏览)

覆盖 [REA](https://github.com/morluto/rea) 与其他 AI 辅助逆向。REA 通过 CLI / MCP，让编程 Agent 调用本地逆向工具。

*据作者与项目报告整理，未经本合集独立复现；证据与项目状态见各案例详情。*

![案例每日累计收录量](assets/case-growth.zh.svg)

## 近期精选

**10 个值得读的案例**：核对Agent究竟发现了什么，让设备继续可用，保存游戏。新增小实验探测记忆与指令冲突；Mac游戏移植和驱动争议提醒我们，技术说法要连同边界一起读。下列日期为来源或作者更新日期，不是收录日期。

1. **[微型Electron：接线正确，证据却太大](cases/rea-tiny-electron-ipc-evidence-output-test.md)** · `2026-11-11`作者自测 — **五文件、846字节样本中，REA据报正确配对渲染端到主进程IPC**，却输出316kb JSON并略过inline脚本。约10秒含冷启，本合集未核源码或完整输出。`分析测试`
2. **[hexgrab：研究PowerToys，再做小取色器](cases/hexgrab-powertoys-colorpicker-rea-study.md)** · `2026-10-29`报道；`2026-10-12`研究 — Claude/REA调查发布二进制，作者对照源码得出**九项中八项完全正确、一项部分正确**。公开.NET10实现；未分析的runner负责注册热键，暴露跨二进制盲点。只测单屏，本合集未重跑。`分析测试`
3. **[记忆与AGENTS.md冲突时，Agent听谁的](cases/sparsamp-agent-memory-agents-md-conflict-probes.md)** · `2026-11-11`作者实验 — **每设置五次，探测格式、时效与付费许可。**Sparshith称Codex依文件，Claude会考虑较新或更安全的指令。小样本行为自测，不是通用优先级规则，harness／模型影响未区分。`分析测试`
4. **[MousePods：AirPods在Linux当鼠标与游戏头追](cases/airpods3-claude-remotehid-linux-head-mouse-report.md)** · `2026-11-11`报道；`2026-11-10`固定项目文档 — **Claude辅助RemoteHID研究、公开实现与项目自报AirPods 3／Pro 2实机检查。**不刷耳机固件，但Proton游戏接入会改前缀。MTU与设备身份变化未隔离，部分模式仍实验。本合集未运行。`未独立核验`
5. **[1994 Jeep：别急着信读出的数字，先核固件](cases/zulali-32year-jeep-claude-control-report.md)** · `2026-11-11`作者与读者报告 — **Claude／Codex辅助SCI诊断，转述燃油修正方向纠错。**fly报告NOx从702降到13，但最终改写内容不清；过检不证明合规，执行器命令不等于自动驾驶。本合集未审仓库或实车测试。`未独立核验`
6. **[TimeSplitters 2：把PS2行为追进原生PC版](cases/destinity-timesplitters2-claude-native-pc-recompile.md)** · `2026-11-10`作者报告；`2026-11-09`固定文档 — **Claude辅助MIPS到C++，以PCSX2画面与状态追查差异。**项目自报Linux／Steam Deck首关通关，仍用PCSX2图形／音频。内部测试工具未公开，后续关卡、部分VU1状态与互联网联机待测，Windows／在线版待发布。须自备光盘，本合集未构建。`进行中`
7. **[bo2-mac：Black Ops II移到ARM64](cases/bo2-mac-claude-arm64-static-translation-report.md)** · `2026-11-11`同串转述 — **Claude辅助Ghidra／Remill／LLVM翻译，单M1战役据报51–60fps。**部分代码仍进小型x86 VM；beta、无在线，报告111–116°C。本合集未核仓库与测试日志，须自备Steam游戏。`未核验转述`
8. **[DX-Ball：从声像函数走到Windows重建](cases/dx-ball-sound-pan.md)** · `2026-11-01`报道；`2026-10-31`项目记录 — Codex／REA／Ghidra重建报告**270个游戏函数、84968字节匹配**，另有原生VC4构建。仅时间戳不同的比较对象是较早重建版，不是原版EXE；原版50关通关与完整原生音频仍待测。须自备文件，本合集未重建。`项目自测重建`
9. **[日聪蓄电池：回成功不等于执行](cases/gemini-echonet-lite-code-copy-analysis-report.md)** · `2026-11-11`作者文章，回顾8至9月工作 — **Gemini辅助HEX对照，据报定位电力与排程字段。**作者也记录成功应答却设置不变、待机死锁、粘贴修复丢保护逻辑；硬件安全与长期运行未经本合集核验。`进行中`
10. **[Vino：AI辅助驱动遇上专利争议](cases/vino-displaylink-rust-ai-driver-cease-desist-report.md)** · `2026-11-11`转述 — **Rust／Claude研究Linux DisplayLink互通。**传播较广的新帖列出英国专利与按周索费说法，原法律文件和驱动测试仍未核；威胁收费不等于已判赔偿。`未核验转述`


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
| [游戏与游戏保存](categories/games.md) | **425** |
| [硬件与设备互通](categories/hardware.md) | **562** |
| [应用与客户端](categories/apps.md) | **856** |
| [算法与功能重建](categories/algorithms.md) | **251** |

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
