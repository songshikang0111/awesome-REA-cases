<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

**English (default)** | [简体中文](README.zh-CN.md)

### Explore software and hardware with AI.

A curated collection of **reverse-engineering projects, experiments, and ideas**: revive old devices, rebuild apps, preserve games, and understand hidden behavior.

# 1464 cases & projects

**Latest case update:** November 2, 2026, 08:09 · **Last maintained:** November 2, 2026, 08:09 · Beijing time (UTC+8). Counts as of this maintenance.

Updates **6× daily** · [Full index](INDEX.en.md) · [Browse categories](#browse-by-category)

Covers [REA](https://github.com/morluto/rea) and other AI-assisted work. REA connects coding agents to local reverse-engineering tools through CLI and MCP.

*Based on author and project reports; not independently reproduced here. Evidence and project status are recorded in each case.*

![Cumulative case collection growth, by day](assets/case-growth.en.svg)

## Recent picks

**10 worth reading** for device interoperability, useful replacements, game preservation and binary analysis. These picks favor inspectable implementations, clear human/AI attribution and explicit test limits; a popular claim alone does not establish a working replacement. Dates below are source or author-update dates, not collection dates.

1. **[tolpo: a live 3D view of your Tapo home](cases/en/tolpo-tapo-claude-lan-3d-home-report.md)** · `2026-10-29` — A Claude-assisted protocol-research report leads to **public LAN/MCP control and a human-corrected floor plan**. Reuses python-kasa; earlier project tests cover nine rooms and 18 devices, not every write or model. Local device traffic does not mean local AI. `In progress`
2. **[hexgrab: learn from PowerToys, then build a smaller picker](cases/en/hexgrab-powertoys-colorpicker-rea-study.md)** · `2026-10-29` report; `2026-10-12` investigation — Claude/REA studies shipped binaries; the author's source scorecard gives **8 of 9 claims fully correct, one partial**. Public .NET 10 implementation; hotkey registration in an unexamined runner exposed a blind spot. One monitor tested, not independently rerun. `Analysis test`
3. **[scapectl: control a Fractal Scape headset without the web app](cases/en/scapectl-fractal-scape-claude-usb-hid.md)** · `2026-10-29` — **Claude Code-assisted USB HID research and a public Go tray app/CLI** for status, EQ presets and device events. Documents hardware corrections to source labels; macOS/Windows project-tested, Linux untested. Unsigned/unnotarized; not run here. `In progress`
4. **[Pokémon Bank: keep transfers local on a 3DS](cases/en/wokann-pokemon-bank-mover-codex-offline-patch.md)** · `2026-11-01` report and project record — Wokann explicitly credits Codex for decompilation analysis and patch work. A **public local-server patch preserves Bank/Mover workflows**, not the official backend; **no HOME transfer**. Requires your own supported titles and save backups; not run here. `In progress`
5. **[DX-Ball: from one audio function to a Windows rebuild](cases/en/dx-ball-sound-pan.md)** · `2026-11-01` report; `2026-10-31` project record — Codex/REA/Ghidra reconstruction reports **270 matching game functions and 84,968 bytes**, plus a native VC4 build. Timestamp-only image differences are against an earlier rebuild, not the retail EXE. Original 50-board campaign and full native audio remain unverified; bring your own files. Not rebuilt here. `Project-tested reconstruction`
6. **[Sonic Adventure: matching Dreamcast code, then a GCC port](cases/en/sonic-adventure-dreamcast-claude-codex-decompilation.md)** · `2026-11-01` — Kyle Mayer credits Claude Code/Codex and hundreds of hours of human polishing; the public project reports **247 matching binaries, 97.7% C / 2.3% assembly**. Some C needs compiler-assembly patches. The GCC build is separate, not a PC port; bring your own Japanese disc. Not rebuilt here. `Analysis test`
7. **[RETROGRADE: test what an agent actually understands](cases/en/retrograde-generated-reverse-engineering-agent-benchmark.md)** · `2026-11-01` — celeste proposes **freshly generated programs and execution-based scoring**, with confidence and evidence addresses attached to claims. Reports 15 workloads, four languages and six ISAs; example scores illustrate the method, not a model leaderboard. Round 0 results pending; not run here. `In progress`
8. **[Claude writes proofs; Rocq checks the binaries](cases/en/anthropic-theorem-claude-binary-formal-verification.md)** · `2026-10-22` — Anthropic/Theorem report machine-code no-crash proofs for **239 entry points across 123 libraries**. Single-threaded static RISC-V/Linux, inputs below 64MB; **not bug-free whole libraries**, and the checker was not independently rerun here. `Analysis test`
9. **[OKOK Libre: keep your scale, replace the ad-heavy app](cases/en/okok-libre-rea-glm-scale-android.md)** · `2026-10-31` — JYunth credits REA/GLM with APK research and Opus with UI work; **public Android code covers three OKOK Bluetooth protocols**. The pinned main manifest has no internet permission, not a final-APK audit. Some scale families remain unsupported; formula equivalence and health estimates are unverified. `In progress`
10. **[PE2PC: Parasite Eve II without a console emulator](cases/en/parasite-eve2-pe2pc-claude-native-port.md)** · `2026-11-02` report; `2026-11-01` project record — Snaity credits Claude Code and builds on **GabeRealB's existing decompilation**, with a C/Rust PC runtime and human play-testing. Project-reported two-disc support; **60-fps presentation still uses 30-fps game logic**. Experimental mods, your own USA discs, no independent rebuild here. `In progress`

## Classic cases

- **[Universal Modder](cases/en/universal-modder.md)** — AI-assisted cross-game mods, including Minecraft content in GTA V.
- **[Firefighter](cases/en/firefighter-rust.md)** — Recover Pascal logic from a DOS binary, then rewrite it in Rust, according to the author.
- **[Modern Warfare 2](cases/en/mw2-decompilation.md)** — Author-reported multi-agent reconstruction; **83% function byte matches**, no public code or independent reproduction here.
- **[Smart toilet from the Mac menu bar](cases/en/smart-toilet.md)** — Author-reported Bluetooth research and home-device control.
- **[Apple TV remote on Linux](cases/en/siri-remote-linux.md)** — Bluetooth interoperability with a public implementation; REA use unconfirmed.
- **[Plustek scanner & ThinkPad camera](cases/en/schaller-opticfilm-thinkpad-linux.md)** — Windows reference behavior informs Linux drivers; published measurements retain low-light and exposure defects.
- **[LG PlxNative](cases/en/lg-plxnative.md)** — Native Plex client; user-selection time reportedly falls from **30 seconds to 3 seconds**.

## Browse by category

| Category | Entries |
| :--- | ---: |
| [Games & preservation](categories/en/games.md) | **318** |
| [Hardware & interoperability](categories/en/hardware.md) | **387** |
| [Applications & clients](categories/en/apps.md) | **600** |
| [Algorithms & feature recovery](categories/en/algorithms.md) | **159** |

[**View all cases →**](INDEX.en.md) · [Contribute (中文)](CONTRIBUTING.md) · [Maintenance (中文)](MAINTENANCE.md)

<details>
<summary><strong>Update & evidence notes</strong></summary>

- **Continuous resolved-material cutoff:** October 15, 2026, 16:00, Beijing time. Older unresolved sources can hold this cutoff back while newer entries are added; it is not a verification date for every project.
- Searches run six times daily with keyword and pagination limits; coverage is bounded, not exhaustive, and some linked evidence remains unresolved. Source dates, evidence boundaries, and engagement snapshots are recorded in case details.
- Full descriptions, sources, and language switching are available on every case page.

</details>

## Scope & license

**Unofficial collection.** Original summaries and public links only; no proprietary software, game assets, keys, or private material.

Original curation and code: **[MIT](LICENSE)**. Linked work retains its own rights; use legally obtained targets and check the relevant permissions.
