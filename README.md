<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

[![Featured by Awesome REA](https://raw.githubusercontent.com/reacher-z/Awesome-REA/main/assets/featured-by-awesome-rea-inline.svg)](https://github.com/reacher-z/Awesome-REA)

**English (default)** | [简体中文](README.zh-CN.md)

### Explore software and hardware with AI.

A curated collection of **AI-assisted reverse-engineering projects, experiments, and ideas** for device interoperability, app rebuilding and game preservation—including failed attempts and author corrections.

# 2240 cases & projects

**Latest case update:** November 14, 2026, 16:07 · **Last maintained:** November 14, 2026, 16:07 · Beijing time (UTC+8). Counts as of this maintenance; source dates and the continuous evidence cutoff are separate.

Updates **6× daily** · [Full index](INDEX.en.md) · [Browse categories](#browse-by-category)

Covers [REA](https://github.com/morluto/rea) and other AI-assisted work. REA connects coding agents to local reverse-engineering tools through CLI and MCP.

*Based on author and project reports; not independently reproduced here. Evidence and project status are recorded in each case.*

![Cumulative case collection growth, by day](assets/case-growth.en.svg)

## Recent picks

**10 worth reading**: probe devices, recover game behavior and compare claims with documented tests. These picks favor concrete uses and visible evidence limits over broad capability promises. Dates identify sources or author updates, not collection dates.

1. **[Ember mug: probe Bluetooth, build a personal controller](cases/en/dmitriy-ember-mug-codex-bluetooth-probing-report.md)** · `2026-11-14` author report — Dmitriy says **Codex probed characteristics against the iOS app** and built temperature/light controls in about an hour. The author prohibited web lookup, not independently enforced; coffee-level accuracy and code unchecked. `Unverified here`
2. **[Fujifilm X half: camera to Mac without the phone](cases/en/fujifilm-x-half-opus-wireless-mac-import-report.md)** · `2026-11-12` author report — **Opus reportedly identifies Bluetooth/Wi-Fi protocol differences** for JPEG imports and Google Photos uploads. Incremental camera tests, not an iteration-free build; code and traces unchecked here. `Unverified here`
3. **[Anker recorder: ask an agent for last week's conversation](cases/en/berryxia-anker-recorder-rea-mcp-knowledge-app.md)** · `2026-11-12` author report — **REA Bluetooth research and MCP recording retrieval**, with local Qwen ASR or online transcription. Berryxia plans source release after refinement/testing; code and device path unchecked here. `In progress`
4. **[Fallout Van Buren: six years of research meet REA](cases/en/fallout-van-buren-kran-rea-human-guided-reconstruction.md)** · `2026-11-14` author thread — Kran credits **manual research, shenmarukai's initial decompilation and an IDA database**, not a from-zero agent. Adam reports a DX9 migration; 64-bit is a goal, and the target is a tech demo, not a complete game. Not built here. `In progress`
5. **[Lemmings for Windows 95: match functions, not headlines](cases/en/lemmings-win95-human-led-ai-reconstruction-report.md)** · `2026-11-12` report; `2026-11-09` pinned docs — Human-led REA/Claude/Codex work reports **696/696 matched functions across eight modules**. Whole EXE/DLL files still differ; portable builds and original-compiler matching are separate. Bring your own game assets; not built here. `In progress`
6. **[decompdecomp: byte matching with an assembly fallback](cases/en/decompdecomp-local-agent-byte-matching-workbench.md)** · `2026-11-14` report; `2026-11-13` pinned docs — **Agents write C/C++, original compilers judge the bytes.** This independent decomp.wtf continuation reports no whole game decompiled; exports retain assembly, and chosen cloud models may receive game material. Not run here. `In progress`
7. **[ZigZag: from SVG to a Brother embroidery machine](cases/en/kath-korevec-brother-chatgpt-embroidery-report.md)** · `2026-11-13` report and pinned docs — **Skitch PP1 Bluetooth upload and MCP-assisted design**, with project-reported hardware tests. NOTICE credits the protocol to Respira; the earlier ChatGPT origin story remains secondary, not independent discovery. Not run here. `Unverified here`
8. **[MousePods: AirPods as a Linux mouse and head tracker](cases/en/airpods3-claude-remotehid-linux-head-mouse-report.md)** · `2026-11-11` reports; `2026-11-10` pinned docs — **Claude-assisted RemoteHID research and reported AirPods 3/Pro 2 hardware checks.** No earbud flash, but Proton integration changes prefixes. MTU/device-identity effects were not isolated; not run here. `Unverified here`
9. **[Smart bead board: an APK to a Raspberry Pi controller](cases/en/smart-bead-board-claude-raspberry-pi-mcp-control-report.md)** · `2026-11-14` author report and clarification — Labelray says **Claude decompiled the official APK to find the protocol**, then wrote MCP tooling to light selected positions without the app. Board model, transport and code are undisclosed; no device test here. `Unverified here`
10. **[TimeSplitters 2: PS2 behavior to a PC port](cases/en/destinity-timesplitters2-claude-native-pc-recompile.md)** · `2026-11-10` author report; `2026-11-09` pinned docs — **Claude-assisted MIPS-to-C++ with PCSX2 frame/state comparisons** and a reported Linux/Steam Deck first-level playthrough. Still uses PCSX2 graphics/audio; later levels and internet play need checks. Self-supplied disc; not built here. `In progress`

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
| [Games & preservation](categories/en/games.md) | **445** |
| [Hardware & interoperability](categories/en/hardware.md) | **596** |
| [Applications & clients](categories/en/apps.md) | **932** |
| [Algorithms & feature recovery](categories/en/algorithms.md) | **267** |

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
