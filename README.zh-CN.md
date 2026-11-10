<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

[English](README.md) | **简体中文**

### 用 AI 读懂软件与硬件。

精选 **AI 辅助逆向的项目、实验与具体想法**：让设备互通，重建应用，保存游戏，也记录失败尝试与作者对旧结论的更正。

# 1995 个案例与项目

**最近案例更新：**2026 年 11 月 10 日 08:11 · **最近维护：**2026 年 11 月 10 日 08:11 · 北京时间（UTC+8）；数量统计截至此次维护，连续证据截止见下方说明。

**每天更新 6 次** · [完整目录](INDEX.md) · [按分类浏览](#分类浏览)

覆盖 [REA](https://github.com/morluto/rea) 与其他 AI 辅助逆向。REA 通过 CLI / MCP，让编程 Agent 调用本地逆向工具。

*据作者与项目报告整理，未经本合集独立复现；证据与项目状态见各案例详情。*

![案例每日累计收录量](assets/case-growth.zh.svg)

## 近期精选

**10 个值得读的案例**：追查二进制证据，让乐高机构动起来，让设备继续可用，保存游戏。可追查的方法与坦诚的测试边界，比发布宣传或单次模型排名更重要。收录不等于成功；下列日期为来源或作者更新日期，不是收录日期。

1. **[XRef：究竟谁写了这个二进制字段？](cases/alex09x-xref-serialized-status-writer-walkthrough.md)** · `2026-11-07`作者帖；`2026-11-06`固定文档 — **从序列化键追到候选writer与指令证据**，公开Rust／JSON／MCP工具供分析者和Agent使用。排名是启发式，x86-64输入支持有边界，live探针可能扰动目标。本合集未运行。`相关项目`
2. **[hexgrab：研究PowerToys，再做小取色器](cases/hexgrab-powertoys-colorpicker-rea-study.md)** · `2026-10-29`报道；`2026-10-12`研究 — Claude/REA调查发布二进制，作者对照源码得出**九项中八项完全正确、一项部分正确**。公开.NET10实现；未分析的runner负责注册热键，暴露跨二进制盲点。只测单屏，本合集未重跑。`分析测试`
3. **[LDraw Mecha：让静态乐高机构动起来](cases/ldraw-mecha-semantic-parts-blender-motion.md)** · `2026-11-08`报道与固定v0.5.0文档（北京时间） — **从带注释零件文本推机构，再映射同名节点生成Blender rig。**公开运动与间隙检查也保留边界：看起来能动不等于物理可行，42043只做起重机，Linux／WSL2路径未测。本合集未运行。`相关项目`
4. **[scapectl：不用网页也能控制Fractal Scape耳机](cases/scapectl-fractal-scape-claude-usb-hid.md)** · `2026-10-29` — **Claude Code辅助USB HID研究，公开Go托盘应用与CLI**，查看状态、切EQ预设、响应设备事件。文档保留实机纠正源码标注的过程；项目只测macOS/Windows，Linux未测。未经签名／公证，本合集未运行。`进行中`
5. **[TimeSplitters 2：把PS2行为追进原生PC版](cases/destinity-timesplitters2-claude-native-pc-recompile.md)** · `2026-11-10`作者报告；`2026-11-09`固定文档 — **Claude辅助MIPS到C++，以PCSX2画面与状态追查差异。**项目自报Linux／Steam Deck首关通关，仍用PCSX2图形／音频。内部测试工具未公开，后续关卡、部分VU1状态与互联网联机待测，Windows／在线版待发布。须自备光盘，本合集未构建。`进行中`
6. **[Project Avalanche：让SSX滑上现代PC](cases/project-avalanche-ssx2012-claude-bevy-reimplementation.md)** · `2026-11-09`报道与固定项目文档（北京时间） — **Claude辅助光盘格式与行为研究，再以Rust／Bevy重实现**，文档提供Windows／Linux构建、滑雪、存档与专用服务器。无人完整通关，未解码行为仍有近似；须自备Xbox 360光盘镜像，本合集未构建或试玩。`进行中`
7. **[DX-Ball：从声像函数走到Windows重建](cases/dx-ball-sound-pan.md)** · `2026-11-01`报道；`2026-10-31`项目记录 — Codex／REA／Ghidra重建报告**270个游戏函数、84968字节匹配**，另有原生VC4构建。仅时间戳不同的比较对象是较早重建版，不是原版EXE；原版50关通关与完整原生音频仍待测。须自备文件，本合集未重建。`项目自测重建`
8. **[MechWarrior 3：让1999年的机甲游戏跑上现代电脑](cases/mechwarrior3-rea-ghidra-modern-cpp-rebuild.md)** · `2026-11-04`报道与固定项目记录 — Owen Morgan披露**REA／Ghidra研究、逐函数C++重建**，报告以Unicorn对照原版。公开原生后端、宽屏与八人UDP联机；报道明确Linux未试玩，Pirate's Moon未支持。须自备原游戏，本合集未构建。`进行中`
9. **[SoftProtect：REA逆向了，还是找到源码了？](cases/softprotect-ai-adversarial-rea-test.md)** · `2026-11-09`作者纠错 — **首轮看似还原，实为循Debug路径读到本地源码。**删源码后仍部分恢复，但VM保护没开，也没有启用后的结果。值得读的实验设计纠错，不证明保护通破或普遍有效。本合集未复跑。`分析测试`
10. **[Redivivus：用审阅过的数据库提案恢复暗黑II](cases/redivivus-diablo2-ghidra-agent-proposals.md)** · `2026-11-08`报道与固定项目文档 — **Claude／MCP Agent只读调查Ghidra数据库，再按证据提修正。**项目自报单人通关、地址归一比较下**7772／14626函数匹配**，不是整EXE相同。仍有崩溃，x64编译通过不等于可玩，须自备原游戏。本合集未重建。`进行中`


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
| [游戏与游戏保存](categories/games.md) | **408** |
| [硬件与设备互通](categories/hardware.md) | **534** |
| [应用与客户端](categories/apps.md) | **813** |
| [算法与功能重建](categories/algorithms.md) | **240** |

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
