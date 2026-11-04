<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

[English](README.md) | **简体中文**

### 用 AI 读懂软件与硬件。

精选 **AI 逆向的项目、实验与具体想法**：让旧设备继续工作，重建应用功能，保存游戏，理解隐藏的实现。

# 1652 个案例与项目

**最近案例更新：**2026 年 11 月 4 日 16:15 · **最近维护：**2026 年 11 月 4 日 16:15 · 北京时间（UTC+8）；数量统计截至此次维护，连续证据截止见下方说明。

**每天更新 6 次** · [完整目录](INDEX.md) · [按分类浏览](#分类浏览)

覆盖 [REA](https://github.com/morluto/rea) 与其他 AI 辅助逆向。REA 通过 CLI / MCP，让编程 Agent 调用本地逆向工具。

*据作者与项目报告整理，未经本合集独立复现；证据与项目状态见各案例详情。*

![案例每日累计收录量](assets/case-growth.zh.svg)

## 近期精选

**10 个值得读的案例**，覆盖设备互通、实用替代品、游戏保存与二进制分析，也保留一次区分参数发现与实测行为的更正。下列日期为来源或作者更新日期，不是收录日期。

1. **[tolpo：Tapo住宅的实时3D视图](cases/tolpo-tapo-claude-lan-3d-home-report.md)** · `2026-10-29` — 转述Claude辅助协议研究，公开**LAN/MCP控制与人工校正户型**。复用python-kasa；较早项目自测覆盖九房间、18设备，不代表所有写操作与型号。设备本地通信不等于AI本地运行。`进行中`
2. **[hexgrab：研究PowerToys，再做小取色器](cases/hexgrab-powertoys-colorpicker-rea-study.md)** · `2026-10-29`报道；`2026-10-12`研究 — Claude/REA调查发布二进制，作者对照源码得出**九项中八项完全正确、一项部分正确**。公开.NET10实现；未分析的runner负责注册热键，暴露跨二进制盲点。只测单屏，本合集未重跑。`分析测试`
3. **[scapectl：不用网页也能控制Fractal Scape耳机](cases/scapectl-fractal-scape-claude-usb-hid.md)** · `2026-10-29` — **Claude Code辅助USB HID研究，公开Go托盘应用与CLI**，查看状态、切EQ预设、响应设备事件。文档保留实机纠正源码标注的过程；项目只测macOS/Windows，Linux未测。未经签名／公证，本合集未运行。`进行中`
4. **[REA Launcher SDK：让自有旧游戏重新跑起来](cases/makita-rea-launcher-sdk-retro-games.md)** · `2026-11-03`作者报告与项目记录 — Fabio Makita公开**从旧赛车启动器提炼的Rust、Wine与打包机制**，让Agent研究、人在检查点决策。项目要求原游戏目录只读、修复逐游戏验证；须自备游戏，所谓90%是估计，不是兼容覆盖率。本合集未构建。`进行中`
5. **[Pokémon Bank：把传输留在3DS本地](cases/wokann-pokemon-bank-mover-codex-offline-patch.md)** · `2026-11-01`报道与项目记录 — Wokann明确披露Codex辅助反编译分析和补丁工作，公开**本地服务器补丁保留Bank／Mover流程**，不是官方后端复刻；**不支持HOME传输**。须自备受支持原作并备份存档，本合集未运行。`进行中`
6. **[DX-Ball：从声像函数走到Windows重建](cases/dx-ball-sound-pan.md)** · `2026-11-01`报道；`2026-10-31`项目记录 — Codex／REA／Ghidra重建报告**270个游戏函数、84968字节匹配**，另有原生VC4构建。仅时间戳不同的比较对象是较早重建版，不是原版EXE；原版50关通关与完整原生音频仍待测。须自备文件，本合集未重建。`项目自测重建`
7. **[MechWarrior 3：让1999年的机甲游戏跑上现代电脑](cases/mechwarrior3-rea-ghidra-modern-cpp-rebuild.md)** · `2026-11-04`报道与固定项目记录 — Owen Morgan披露**REA／Ghidra研究、逐函数C++重建**，报告以Unicorn对照原版。公开原生后端、宽屏与八人UDP联机；报道明确Linux未试玩，Pirate's Moon未支持。须自备原游戏，本合集未构建。`进行中`
8. **[CS2声音：参数值不等于实测延迟](cases/cs2-claude-sound-delay-hardware-correction.md)** · `2026-11-04`作者更正 — Thour称Claude找到了**23ms声音偏移参数**，但换耳机复测后撤回步枪普遍多20ms延迟的说法。AK-47与M4A4结果不同；无原始测量，本合集未独立重跑。`分析测试`
9. **[OKOK Libre：留下体脂秤，换掉广告App](cases/okok-libre-rea-glm-scale-android.md)** · `2026-10-31` — JYunth称REA／GLM研究APK、Opus制作UI，**公开Android代码覆盖三种OKOK蓝牙协议**。固定主Manifest无联网权限，不等于最终APK审计；部分秤家族未支持，公式等价与健康估计未核验。`进行中`
10. **[121GW：把万用表固件重建为C](cases/eevblog-121gw-claude-c-firmware-reconstruction.md)** · `2026-11-04`作者更新 — Dave Jones报告**Claude Code不到24小时重建且能工作**；EEVblog1784目录列Ghidra、bootloader研究与人类实机测试。本合集未观看视频或核对源码，蓝牙、校准与全功能等价仍未确认。`作者报告结果`

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
| [游戏与游戏保存](categories/games.md) | **342** |
| [硬件与设备互通](categories/hardware.md) | **449** |
| [应用与客户端](categories/apps.md) | **681** |
| [算法与功能重建](categories/algorithms.md) | **180** |

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
