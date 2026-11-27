<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

**English (default)** | [简体中文](README.zh-CN.md)

### Explore software and hardware with AI.

A curated collection of **AI-assisted reverse-engineering projects, experiments, and ideas** for device interoperability, behavior-preserving app rebuilding and game preservation—including failed attempts and author corrections.

# 2899 cases & projects

**Latest case update:** November 27, 2026, 12:15 · **Last maintained:** November 27, 2026, 12:15 · Beijing time (UTC+8). Counts as of this maintenance; source dates and the continuous evidence cutoff are separate.

Updates **6× daily** · [Full index](INDEX.en.md) · [Browse categories](#browse-by-category)

Covers [REA](https://github.com/morluto/rea) and other AI-assisted work. REA connects coding agents to local reverse-engineering tools through CLI and MCP.

*Based on author and project reports; not independently reproduced here. Evidence and project status are recorded in each case.*

![Cumulative case collection growth, by day](assets/case-growth.en.svg)

## Recent picks

**10 worth reading**: recover a compiler, trace retry behavior, preserve a game or reopen a device. Start with the concrete methods and reported checks, not a headline's promise of a complete clone. Dates identify sources or author updates, not collection dates.

1. **[borland-reborn: recover a 1991 compiler](cases/en/borland-reborn-bcc20-exhume-byte-matching.md)** · `2026-11-14` report and pinned docs — Exhume's Claude Code skills support **reportedly byte-identical BCC.EXE/CPP.EXE rebuilds**. A separate modding build has 1,836 compile comparisons and 83% coverage, not every path or uniquely recovered original source. Not rebuilt here. `Unverified here`
2. **[OpenGlass Go: reopen a glasses-free 3D display](cases/en/openglass-go-kimi-gemini-armbian-firmware.md)** · `2026-11-22` author thread and pinned builder docs — Megabits credits **Kimi for reversing and early code, Gemini Neon for finishing Armbian firmware**. Public docs describe 3D media playback, file transfer and STM32 control. Hardware testing is project-reported; the kernel bug awaits submission. Not built or flashed here. `In progress`
3. **[FreeCAD: build an interface instead of clicking](cases/en/aoqu-agent-native-freecad-binary-mcp-computer-use.md)** · `2026-11-26` author update and pinned study — **DeepSeek/REA exposes FreeCAD through MCP**; five tasks, three runs per setup reportedly pass every check. The 55× speed/35× token demo excludes 30–85-minute server builds, not a universal CAD speedup. Methods read, tests not rerun. `Analysis test`
4. **[Forza Motorsport 4: an Xbox racer on Windows and Mac](cases/en/i2kiselev-forza4-ai-static-recompilation.md)** · `2026-11-27` report; `2026-11-15` pinned docs — **AI-assisted static recompilation adds an Apple Silicon preview**, with contributor-reported M1 Max/M3 Free Play tests. Windows 5K at 102 fps is one PC's benchmark, not 5K at 240 fps or Mac performance. Own disc required; macOS 14 and some Mac features remain untested. Not built here. `In progress`
5. **[Underworld Exhumed: preserve two DOS worlds](cases/en/underworld-exhumed-ultima-claude-skills-byte-matching.md)** · `2026-11-20` introduction; `2026-11-17` pinned docs — Exhume's Claude Code skills support **reported byte-identical UW.EXE/UW2.EXE rebuilds**, plus native/web ports checked against 17/13 DOS recordings. Project reports, not checks rerun here; native ports need your own game data. `Unverified here`
6. **[Capcom vs. SNK 2: matching code, then porting the game](cases/en/cvs2-naomi-dc-claude-decompilation-native-ports.md)** · `2026-11-26` report and pinned docs — gibletto discloses **Claude-assisted reconstruction of three arcade/Dreamcast programs**, with reported byte matches and five-platform ports. Disc assets and many SDK modules are reused; matching originals does not verify port visuals or sound. Network features remain unavailable. Docs read, no builds rerun. `Unverified here`
7. **[Elecbrakes: audit a trailer's Bluetooth brakes](cases/en/elecbrakes-claude-android-brake-audit-report.md)** · `2026-11-19` researcher account; `2026-11-20` CVE record — Forck and McCarthy credit **Claude with bytecode analysis and research tooling**, then report tests on their own hardware. EB2/VM1 fixes are documented; older ELBC 2000 had no fix at publication. Static firmware analysis did not demonstrate malicious flashing. Not reproduced here. `Unverified here`
8. **[rust-anything: rebuild Prettier without guessing its output](cases/en/rust-anything-claude-behavior-capture-rust-migration.md)** · `2026-11-22` report and pinned docs — Agents write Rust against recorded behavior. Updated project docs report **17,224 byte-identical runs, 15,861 fully in Rust**; the rest fall back. The earlier M4 benchmark's roughly 19× CLI gain includes process startup, versus 4.2× warmed in-process. Recording runs real side effects; use isolated copies. Not rerun here. `Unverified here`
9. **[echo-dot-assist: keep the microphones, replace Alexa](cases/en/echo-dot-assist-claude-hassmic-home-assistant.md)** · `2026-11-24` introduction and pinned README — **Claude-credited hassmic connects old Echos to Home Assistant**, keeping the original audio front end. Unlocking research belongs to R0rt1z2. Only one unit per model was tested by the project; code is unaudited and installation can wipe or brick a device. Network isolation is not verified here. `In progress`
10. **[curl.exe: explain exactly when a request retries](cases/en/nate-brooks-curl-retry-claude-rea-analysis.md)** · `2026-11-27` author thread — Nate reports **eight Claude/REA tool calls**, then matching eight HTTP codes and backoff constants against source and checking a local server. Target revision and full logs are absent; this is the author's comparison, not a test rerun here. `Analysis test`

## Classic cases

- **[Universal Modder](cases/en/universal-modder.md)** — AI-assisted cross-game mods, including Minecraft content in GTA V.
- **[Firefighter](cases/en/firefighter-rust.md)** — Recover Pascal logic from a DOS binary, then rewrite it in Rust, according to the author.
- **[Modern Warfare 2](cases/en/mw2-decompilation.md)** — Author-reported multi-agent reconstruction; **83% function byte matches**, no public code or independent reproduction here.
- **[Smart toilet from the Mac menu bar](cases/en/smart-toilet.md)** — Author-reported Bluetooth research and home-device control.
- **[Apple TV remote on Linux](cases/en/siri-remote-linux.md)** — Bluetooth interoperability with a public implementation; REA use unconfirmed.
- **[Plustek scanner & ThinkPad camera](cases/en/schaller-opticfilm-thinkpad-linux.md)** — Windows reference behavior informs Linux drivers; published measurements retain low-light and exposure defects.
- **[Fireface UCX on Linux](cases/en/johan-fireface-ucx-linux-rea-claude-driver.md)** — Johan reports REA/Claude driver work, a terminal mixer and **3.5 ms round-trip audio at 48 kHz** on one first-generation unit; not reproduced here.
- **[LG PlxNative](cases/en/lg-plxnative.md)** — Native Plex client; user-selection time reportedly falls from **30 seconds to 3 seconds**.

## Browse by category

| Category | Entries |
| :--- | ---: |
| [Games & preservation](categories/en/games.md) | **566** |
| [Hardware & interoperability](categories/en/hardware.md) | **762** |
| [Applications & clients](categories/en/apps.md) | **1202** |
| [Algorithms & feature recovery](categories/en/algorithms.md) | **369** |

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
