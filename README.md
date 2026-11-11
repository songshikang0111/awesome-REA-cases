<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

**English (default)** | [简体中文](README.zh-CN.md)

### Explore software and hardware with AI.

A curated collection of **AI-assisted reverse-engineering projects, experiments, and ideas** for device interoperability, app rebuilding and game preservation—including failed attempts and author corrections.

# 2086 cases & projects

**Latest case update:** November 11, 2026, 20:20 · **Last maintained:** November 11, 2026, 20:20 · Beijing time (UTC+8). Counts as of this maintenance; source dates and the continuous evidence cutoff are separate.

Updates **6× daily** · [Full index](INDEX.en.md) · [Browse categories](#browse-by-category)

Covers [REA](https://github.com/morluto/rea) and other AI-assisted work. REA connects coding agents to local reverse-engineering tools through CLI and MCP.

*Based on author and project reports; not independently reproduced here. Evidence and project status are recorded in each case.*

![Cumulative case collection growth, by day](assets/case-growth.en.svg)

## Recent picks

**10 worth reading**: check what an agent actually found, keep devices useful and preserve games. A tiny Electron test exposes output bloat; battery research shows why a successful protocol reply is not proof the device did what you wanted. Dates identify sources or author updates, not collection dates.

1. **[Tiny Electron app: correct wiring, oversized evidence](cases/en/rea-tiny-electron-ipc-evidence-output-test.md)** · `2026-11-11` author test — **REA reportedly pairs renderer-to-main IPC in a five-file, 846-byte sample**, but emits 316kb of JSON and skips an inline script. Roughly ten seconds includes cold startup; no source or full output checked here. `Analysis test`
2. **[hexgrab: learn from PowerToys, then build a smaller picker](cases/en/hexgrab-powertoys-colorpicker-rea-study.md)** · `2026-10-29` report; `2026-10-12` investigation — Claude/REA studies shipped binaries; the author's source scorecard gives **8 of 9 claims fully correct, one partial**. Public .NET 10 implementation; hotkey registration in an unexamined runner exposed a blind spot. One monitor tested, not independently rerun. `Analysis test`
3. **[AlphaProof Code: examine Signal's actual machine code](cases/en/alphaproof-code-signal-machine-code-security-verification.md)** · `2026-11-10` team announcement; `2026-11-11` reader report — **AI-written proofs against human-approved specifications**, with reported historical-bug counterexamples. DeepMind reports a month for key properties, not all of Signal being bug-free. Versions and proof-scale details are relayed; artifacts were not audited here. `Related project`
4. **[MousePods: AirPods become a Linux mouse and head tracker](cases/en/airpods3-claude-remotehid-linux-head-mouse-report.md)** · `2026-11-11` reports; `2026-11-10` pinned project docs — **Claude-assisted RemoteHID research, a public implementation and project-reported AirPods 3/Pro 2 hardware checks.** No earbud flashing; Proton game integration does modify prefixes. MTU and device-identity changes were not isolated; some modes remain experimental. Not run here. `Unverified here`
5. **[A 1994 Jeep: check the firmware before trusting the number](cases/en/zulali-32year-jeep-claude-control-report.md)** · `2026-11-11` author and reader reports — **Claude/Codex-assisted SCI diagnostics and a reported fuel-trim sign correction.** fly relays NOx falling from 702 to 13, but the final modification is unclear. Passing inspection is not proof of compliance; actuator commands are not autonomous driving. Repository and vehicle tests unchecked here. `Unverified here`
6. **[TimeSplitters 2: trace PS2 behavior into a native PC port](cases/en/destinity-timesplitters2-claude-native-pc-recompile.md)** · `2026-11-10` author report; `2026-11-09` pinned docs — **Claude-assisted MIPS-to-C++ work, with PCSX2 frame and state comparisons.** The project reports a Linux/Steam Deck first-level playthrough, still using PCSX2 graphics/audio. Internal test tooling is unpublished; later levels, some VU1 state and internet play need checks. Windows/online await release. Bring your own disc; not built here. `In progress`
7. **[DX-Ball: from one audio function to a Windows rebuild](cases/en/dx-ball-sound-pan.md)** · `2026-11-01` report; `2026-10-31` project record — Codex/REA/Ghidra reconstruction reports **270 matching game functions and 84,968 bytes**, plus a native VC4 build. Timestamp-only image differences are against an earlier rebuild, not the retail EXE. Original 50-board campaign and full native audio remain unverified; bring your own files. Not rebuilt here. `Project-tested reconstruction`
8. **[MechWarrior 3: bring the 1999 mech game to modern PCs](cases/en/mechwarrior3-rea-ghidra-modern-cpp-rebuild.md)** · `2026-11-04` report and pinned project record — Owen Morgan credits **REA/Ghidra research and function-by-function C++ reconstruction**, with reported Unicorn comparisons. Public native backends, widescreen and eight-player UDP networking; Linux was not play-tested in the report, Pirate's Moon is unsupported. Bring your own game; not built here. `In progress`
9. **[Nichicon battery: acknowledgment is not execution](cases/en/gemini-echonet-lite-code-copy-analysis-report.md)** · `2026-11-11` author article, recalling August–September work — **Gemini-assisted HEX comparisons identify reported power and schedule fields.** The author also records unchanged settings despite success replies, standby deadlock and copy-paste fixes losing safeguards. Hardware safety and long-term operation are not verified here. `In progress`
10. **[DESIGN:OS Studio: local Figma files, explicit limits](cases/en/design-os-studio-figma-js-kiwi-rebuild.md)** · `2026-11-11` report/docs; `2026-10-18–19` research notes — **REA studies cached JS; a separate kiwi reader handles the unavailable wasm route.** Public Rust designer with .fig read/write and agent interfaces, but save losses and Windows-test issues remain. Source-available, not OSI open source; not run here. `In progress`


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
| [Games & preservation](categories/en/games.md) | **421** |
| [Hardware & interoperability](categories/en/hardware.md) | **560** |
| [Applications & clients](categories/en/apps.md) | **856** |
| [Algorithms & feature recovery](categories/en/algorithms.md) | **249** |

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
