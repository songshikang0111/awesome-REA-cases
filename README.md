<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

**English (default)** | [简体中文](README.zh-CN.md)

### Explore software and hardware with AI.

A curated collection of **AI-assisted reverse-engineering projects, experiments, and ideas** for device interoperability, behavior-preserving app rebuilding and game preservation—including failed attempts and author corrections.

# 2971 cases & projects

**Latest case update:** November 29, 2026, 00:13 · **Last maintained:** November 29, 2026, 00:13 · Beijing time (UTC+8). Counts as of this maintenance; source dates and the continuous evidence cutoff are separate.

Updates **6× daily** · [Full index](INDEX.en.md) · [Browse categories](#browse-by-category)

Covers [REA](https://github.com/morluto/rea) and other AI-assisted work. REA connects coding agents to local reverse-engineering tools through CLI and MCP.

*Based on author and project reports; not independently reproduced here. Evidence and project status are recorded in each case.*

![Cumulative case collection growth, by day](assets/case-growth.en.svg)

## Recent picks

**10 worth reading**: recover a compiler, replace a decompiler's core or rebuild a racing simulation against recorded behavior. These picks favor concrete work and readable evidence over claims of full automation. Byte matches, interface checks and trace comparisons answer different questions; dates identify sources or author updates, not collection dates.

1. **[borland-reborn: recover a 1991 compiler](cases/en/borland-reborn-bcc20-exhume-byte-matching.md)** · `2026-11-14` report and pinned docs — Exhume's Claude Code skills support **reportedly byte-identical BCC.EXE/CPP.EXE rebuilds**. A separate modding build has 1,836 compile comparisons and 83% coverage, not every path or uniquely recovered original source. Not rebuilt here. `Unverified here`
2. **[OpenGlass Go: reopen a glasses-free 3D display](cases/en/openglass-go-kimi-gemini-armbian-firmware.md)** · `2026-11-22` author thread and pinned builder docs — Megabits credits **Kimi for reversing and early code, Gemini Neon for finishing Armbian firmware**. Public docs describe 3D media playback, file transfer and STM32 control. Hardware testing is project-reported; the kernel bug awaits submission. Not built or flashed here. `In progress`
3. **[FreeCAD: build an interface instead of clicking](cases/en/aoqu-agent-native-freecad-binary-mcp-computer-use.md)** · `2026-11-26` author update and pinned study — **DeepSeek/REA exposes FreeCAD through MCP**; five tasks, three runs per setup reportedly pass every check. The 55× speed/35× token demo excludes 30–85-minute server builds, not a universal CAD speedup. Methods read, tests not rerun. `Analysis test`
4. **[Forza Motorsport 4: an Xbox racer on Windows and Mac](cases/en/i2kiselev-forza4-ai-static-recompilation.md)** · `2026-11-27` report; `2026-11-15` pinned docs — **AI-assisted static recompilation adds an Apple Silicon preview**, with contributor-reported M1 Max/M3 Free Play tests. Windows 5K at 102 fps is one PC's benchmark, not 5K at 240 fps or Mac performance. Own disc required; macOS 14 and some Mac features remain untested. Not built here. `In progress`
5. **[MiniMax: put a rewritten core inside the original app](cases/en/minimax-internal-decompiler-rust-core-replacement-report.md)** · `2026-11-28` company report — An unreleased model reportedly rebuilds an unnamed decompiler core in Rust; **the original GUI still loads files and decompiles with replacement libraries**. CLI/API and a separate UI are also project-checked. Two million lines are experimental code, not a finished product; samples and logs are unavailable. Report read, not reproduced. `Internal evaluation`
6. **[Capcom vs. SNK 2: matching code, then porting the game](cases/en/cvs2-naomi-dc-claude-decompilation-native-ports.md)** · `2026-11-26` report and pinned docs — gibletto discloses **Claude-assisted reconstruction of three arcade/Dreamcast programs**, with reported byte matches and five-platform ports. Disc assets and many SDK modules are reused; matching originals does not verify port visuals or sound. Network features remain unavailable. Docs read, no builds rerun. `Unverified here`
7. **[Elecbrakes: audit a trailer's Bluetooth brakes](cases/en/elecbrakes-claude-android-brake-audit-report.md)** · `2026-11-19` researcher account; `2026-11-20` CVE record — Forck and McCarthy credit **Claude with bytecode analysis and research tooling**, then report tests on their own hardware. EB2/VM1 fixes are documented; older ELBC 2000 had no fix at publication. Static firmware analysis did not demonstrate malicious flashing. Not reproduced here. `Unverified here`
8. **[rust-anything: rebuild Prettier without guessing its output](cases/en/rust-anything-claude-behavior-capture-rust-migration.md)** · `2026-11-22` report and pinned docs — Agents write Rust against recorded behavior. Updated project docs report **17,224 byte-identical runs, 15,861 fully in Rust**; the rest fall back. The earlier M4 benchmark's roughly 19× CLI gain includes process startup, versus 4.2× warmed in-process. Recording runs real side effects; use isolated copies. Not rerun here. `Unverified here`
9. **[DRIG: rebuild GRID's racing behavior](cases/en/drig-grid-rust-bevy-ai-behavior-reimplementation.md)** · `2026-11-28` introduction; `2026-11-27` pinned docs — PipeKnight credits **AI agents and Claude with a Rust/Bevy engine**, compared against original driving, AI and audio traces and individual routines. Racing is project-reported; crashes, physics and visual differences remain. Headless checks do not verify full races; Linux testing is WSLg-only. Own game required, not built here. `In progress`
10. **[nvdriver: take control of a V100 driver](cases/en/quixiai-nvdriver-v100-rea-rust-driver-research.md)** · `2026-11-28` author report and pinned docs — Eric Hartford credits **REA for a Rust reconstruction of NVIDIA 580.178.04**. The project reports eight-V100 comparisons; a four-card PyTorch/NCCL record was read, not rerun. Other architectures remain offline-checked, not hardware-proven. Vendor-motive claims are the author's interpretation. `In progress`

## Classic cases

- **[Universal Modder](cases/en/universal-modder.md)** — AI-assisted cross-game mods, including Minecraft content in GTA V.
- **[Firefighter](cases/en/firefighter-rust.md)** — Recover Pascal logic from a DOS binary, then rewrite it in Rust, according to the author.
- **[Underworld Exhumed](cases/en/underworld-exhumed-ultima-claude-skills-byte-matching.md)** — Project-reported byte-identical rebuilds of two DOS games with Claude skills; native/web ports use recorded-behavior checks, not independently rerun here.
- **[Modern Warfare 2](cases/en/mw2-decompilation.md)** — Author-reported multi-agent reconstruction; **83% function byte matches**, no public code or independent reproduction here.
- **[Smart toilet from the Mac menu bar](cases/en/smart-toilet.md)** — Author-reported Bluetooth research and home-device control.
- **[Apple TV remote on Linux](cases/en/siri-remote-linux.md)** — Bluetooth interoperability with a public implementation; REA use unconfirmed.
- **[Plustek scanner & ThinkPad camera](cases/en/schaller-opticfilm-thinkpad-linux.md)** — Windows reference behavior informs Linux drivers; published measurements retain low-light and exposure defects.
- **[Fireface UCX on Linux](cases/en/johan-fireface-ucx-linux-rea-claude-driver.md)** — Johan reports REA/Claude driver work, a terminal mixer and **3.5 ms round-trip audio at 48 kHz** on one first-generation unit; not reproduced here.
- **[LG PlxNative](cases/en/lg-plxnative.md)** — Native Plex client; user-selection time reportedly falls from **30 seconds to 3 seconds**.

## Browse by category

| Category | Entries |
| :--- | ---: |
| [Games & preservation](categories/en/games.md) | **583** |
| [Hardware & interoperability](categories/en/hardware.md) | **778** |
| [Applications & clients](categories/en/apps.md) | **1230** |
| [Algorithms & feature recovery](categories/en/algorithms.md) | **380** |

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
