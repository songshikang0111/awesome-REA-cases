<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

**English (default)** | [简体中文](README.zh-CN.md)

### Explore software and hardware with AI.

A curated collection of **reverse-engineering projects, experiments, and ideas**: revive old devices, rebuild apps, preserve games, and understand hidden behavior.

# 1729 cases & projects

**Latest case update:** November 5, 2026, 20:11 · **Last maintained:** November 5, 2026, 20:11 · Beijing time (UTC+8). Counts as of this maintenance; the continuous evidence cutoff is recorded below.

Updates **6× daily** · [Full index](INDEX.en.md) · [Browse categories](#browse-by-category)

Covers [REA](https://github.com/morluto/rea) and other AI-assisted work. REA connects coding agents to local reverse-engineering tools through CLI and MCP.

*Based on author and project reports; not independently reproduced here. Evidence and project status are recorded in each case.*

![Cumulative case collection growth, by day](assets/case-growth.en.svg)

## Recent picks

**10 worth reading**: control your devices, preserve games, and turn observed behavior into reusable tools. Recovery can mean erasing data, not saving it; reported success still needs its limits. Dates are source or author-update dates, not collection dates.

1. **[tolpo: a live 3D view of your Tapo home](cases/en/tolpo-tapo-claude-lan-3d-home-report.md)** · `2026-10-29` — A Claude-assisted protocol-research report leads to **public LAN/MCP control and a human-corrected floor plan**. Reuses python-kasa; earlier project tests cover nine rooms and 18 devices, not every write or model. Local device traffic does not mean local AI. `In progress`
2. **[hexgrab: learn from PowerToys, then build a smaller picker](cases/en/hexgrab-powertoys-colorpicker-rea-study.md)** · `2026-10-29` report; `2026-10-12` investigation — Claude/REA studies shipped binaries; the author's source scorecard gives **8 of 9 claims fully correct, one partial**. Public .NET 10 implementation; hotkey registration in an unexamined runner exposed a blind spot. One monitor tested, not independently rerun. `Analysis test`
3. **[scapectl: control a Fractal Scape headset without the web app](cases/en/scapectl-fractal-scape-claude-usb-hid.md)** · `2026-10-29` — **Claude Code-assisted USB HID research and a public Go tray app/CLI** for status, EQ presets and device events. Documents hardware corrections to source labels; macOS/Windows project-tested, Linux untested. Unsigned/unnotarized; not run here. `In progress`
4. **[REA Launcher SDK: help your own old games run again](cases/en/makita-rea-launcher-sdk-retro-games.md)** · `2026-11-03` author report and project record — Fabio Makita shares **Rust, Wine and packaging mechanisms from retro-racing launchers**, with agent research and human checkpoints. Original game folders stay read-only by project policy; fixes need per-game verification. Bring your own games; the claimed 90% is an estimate, not compatibility coverage. Not built here. `In progress`
5. **[Pokémon Bank: keep transfers local on a 3DS](cases/en/wokann-pokemon-bank-mover-codex-offline-patch.md)** · `2026-11-01` report and project record — Wokann explicitly credits Codex for decompilation analysis and patch work. A **public local-server patch preserves Bank/Mover workflows**, not the official backend; **no HOME transfer**. Requires your own supported titles and save backups; not run here. `In progress`
6. **[DX-Ball: from one audio function to a Windows rebuild](cases/en/dx-ball-sound-pan.md)** · `2026-11-01` report; `2026-10-31` project record — Codex/REA/Ghidra reconstruction reports **270 matching game functions and 84,968 bytes**, plus a native VC4 build. Timestamp-only image differences are against an earlier rebuild, not the retail EXE. Original 50-board campaign and full native audio remain unverified; bring your own files. Not rebuilt here. `Project-tested reconstruction`
7. **[MechWarrior 3: bring the 1999 mech game to modern PCs](cases/en/mechwarrior3-rea-ghidra-modern-cpp-rebuild.md)** · `2026-11-04` report and pinned project record — Owen Morgan credits **REA/Ghidra research and function-by-function C++ reconstruction**, with reported Unicorn comparisons. Public native backends, widescreen and eight-player UDP networking; Linux was not play-tested in the report, Pirate's Moon is unsupported. Bring your own game; not built here. `In progress`
8. **[Anthropic-style diagrams: study the web app, keep a local Skill](cases/en/anthropic-style-diagram-claude-web-js-skill.md)** · `2026-11-05` author report; `2026-07-26` pinned project update — Erduo studies Claude's drawing-time JavaScript and publishes **an SVG/PNG workflow with layout checks and explicit semantic review**. Public docs do not prove verbatim recovery of official prompts; rendering was not run here. `In progress`
9. **[BeanScribe: choose your recorder's transcription service](cases/en/gengdaj-feishu-recorder-custom-transcription-app.md)** · `2026-11-04` author updates and project record — Yichen credits REA; **public H5/Python code connects a D3200 to Feishu**, reusing tacshi's protocol research. Single-user deployment; the first 2–4 seconds may be lost, and official quotas/firmware are unchanged. Source-available, not OSI open source; not run here. `In progress`
10. **[iPad mini 7: recover without a forced wired upgrade](cases/en/zhuoli-codex-ipad-mini7-wifi-recovery-erase-report.md)** · `2026-11-05` author report and clarifications — Zhuoli Li credits Codex with studying **WiFi recovery transport and sending an erase command** to recover a boot-looping iOS 18 iPad. **Erasing clears data**; one-device report, not lossless repair, downgrading or a compatibility guarantee. Code and protocol traces were not reviewed here. `Unverified`

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
| [Games & preservation](categories/en/games.md) | **356** |
| [Hardware & interoperability](categories/en/hardware.md) | **467** |
| [Applications & clients](categories/en/apps.md) | **719** |
| [Algorithms & feature recovery](categories/en/algorithms.md) | **187** |

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
