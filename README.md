<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

**English (default)** | [简体中文](README.zh-CN.md)

### Explore software and hardware with AI.

A curated collection of **AI-assisted reverse-engineering projects, experiments, and ideas** for device interoperability, app rebuilding and game preservation—including failed attempts and author corrections.

# 2006 cases & projects

**Latest case update:** November 10, 2026, 12:18 · **Last maintained:** November 10, 2026, 12:18 · Beijing time (UTC+8). Counts as of this maintenance; the continuous evidence cutoff is recorded below.

Updates **6× daily** · [Full index](INDEX.en.md) · [Browse categories](#browse-by-category)

Covers [REA](https://github.com/morluto/rea) and other AI-assisted work. REA connects coding agents to local reverse-engineering tools through CLI and MCP.

*Based on author and project reports; not independently reproduced here. Evidence and project status are recorded in each case.*

![Cumulative case collection growth, by day](assets/case-growth.en.svg)

## Recent picks

**10 worth reading**: trace binary evidence, animate LEGO mechanisms, keep devices useful and preserve games. Inspectable methods and candid test limits matter more than launch claims or one-off model rankings. Inclusion is not proof of success; dates identify sources or author updates, not collection dates.

1. **[XRef: who writes this binary field?](cases/en/alex09x-xref-serialized-status-writer-walkthrough.md)** · `2026-11-07` author post; `2026-11-06` pinned docs — **Trace serialized keys to candidate writers and instruction evidence**, with public Rust/JSON/MCP tools for analysts and agents. Rankings are heuristic, x86-64 input support is bounded, and live probes can disturb the target. Not run here. `Related project`
2. **[hexgrab: learn from PowerToys, then build a smaller picker](cases/en/hexgrab-powertoys-colorpicker-rea-study.md)** · `2026-10-29` report; `2026-10-12` investigation — Claude/REA studies shipped binaries; the author's source scorecard gives **8 of 9 claims fully correct, one partial**. Public .NET 10 implementation; hotkey registration in an unexamined runner exposed a blind spot. One monitor tested, not independently rerun. `Analysis test`
3. **[LDraw Mecha: make a static LEGO mechanism move](cases/en/ldraw-mecha-semantic-parts-blender-motion.md)** · `2026-11-08` report and pinned v0.5.0 docs (Beijing time) — **Infer mechanisms from annotated parts text, then map matching nodes into Blender rigs.** Public motion and clearance checks retain their limits: plausible animation is not physical feasibility, the 42043 demo covers only the crane, and Linux/WSL2 paths are untested. Not run here. `Related project`
4. **[scapectl: control a Fractal Scape headset without the web app](cases/en/scapectl-fractal-scape-claude-usb-hid.md)** · `2026-10-29` — **Claude Code-assisted USB HID research and a public Go tray app/CLI** for status, EQ presets and device events. Documents hardware corrections to source labels; macOS/Windows project-tested, Linux untested. Unsigned/unnotarized; not run here. `In progress`
5. **[TimeSplitters 2: trace PS2 behavior into a native PC port](cases/en/destinity-timesplitters2-claude-native-pc-recompile.md)** · `2026-11-10` author report; `2026-11-09` pinned docs — **Claude-assisted MIPS-to-C++ work, with PCSX2 frame and state comparisons.** The project reports a Linux/Steam Deck first-level playthrough, still using PCSX2 graphics/audio. Internal test tooling is unpublished; later levels, some VU1 state and internet play need checks. Windows/online await release. Bring your own disc; not built here. `In progress`
6. **[Project Avalanche: rebuild SSX for modern PCs](cases/en/project-avalanche-ssx2012-claude-bevy-reimplementation.md)** · `2026-11-09` report and pinned project docs (Beijing time) — **Claude-assisted disc-format and behavior research becomes a Rust/Bevy reimplementation**, with documented Windows/Linux builds, snowboarding, saves and dedicated servers. Nobody has completed a full playthrough; undecoded behavior remains approximate. Bring your own Xbox 360 disc image; not built or played here. `In progress`
7. **[DX-Ball: from one audio function to a Windows rebuild](cases/en/dx-ball-sound-pan.md)** · `2026-11-01` report; `2026-10-31` project record — Codex/REA/Ghidra reconstruction reports **270 matching game functions and 84,968 bytes**, plus a native VC4 build. Timestamp-only image differences are against an earlier rebuild, not the retail EXE. Original 50-board campaign and full native audio remain unverified; bring your own files. Not rebuilt here. `Project-tested reconstruction`
8. **[MechWarrior 3: bring the 1999 mech game to modern PCs](cases/en/mechwarrior3-rea-ghidra-modern-cpp-rebuild.md)** · `2026-11-04` report and pinned project record — Owen Morgan credits **REA/Ghidra research and function-by-function C++ reconstruction**, with reported Unicorn comparisons. Public native backends, widescreen and eight-player UDP networking; Linux was not play-tested in the report, Pirate's Moon is unsupported. Bring your own game; not built here. `In progress`
9. **[SoftProtect: did REA reverse it—or find the source?](cases/en/softprotect-ai-adversarial-rea-test.md)** · `2026-11-09` author correction — **The first apparent recovery followed Debug paths to local source.** Deleting it still allowed partial recovery, but VM protection was off; no VM-enabled result is supplied. A useful test-design correction, not proof of universal defeat or protection. Not rerun here. `Analysis test`
10. **[Redivivus: recover Diablo II through reviewed database proposals](cases/en/redivivus-diablo2-ghidra-agent-proposals.md)** · `2026-11-08` report and pinned project docs — **Claude/MCP agents inspect read-only Ghidra databases and propose evidence-backed corrections.** The project reports a single-player playthrough and **7,772/14,626 matching functions** under its address-normalized comparison; not a whole-EXE match. Crashes remain, x64 compilation is not playable x64 support, and users need their own game. Not rebuilt here. `In progress`


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
| [Games & preservation](categories/en/games.md) | **409** |
| [Hardware & interoperability](categories/en/hardware.md) | **537** |
| [Applications & clients](categories/en/apps.md) | **820** |
| [Algorithms & feature recovery](categories/en/algorithms.md) | **240** |

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
