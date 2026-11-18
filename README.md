<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

**English (default)** | [简体中文](README.zh-CN.md)

### Explore software and hardware with AI.

A curated collection of **AI-assisted reverse-engineering projects, experiments, and ideas** for device interoperability, behavior-preserving app rebuilding and game preservation—including failed attempts and author corrections.

# 2425 cases & projects

**Latest case update:** November 18, 2026, 16:09 · **Last maintained:** November 18, 2026, 16:09 · Beijing time (UTC+8). Counts as of this maintenance; source dates and the continuous evidence cutoff are separate.

Updates **6× daily** · [Full index](INDEX.en.md) · [Browse categories](#browse-by-category)

Covers [REA](https://github.com/morluto/rea) and other AI-assisted work. REA connects coding agents to local reverse-engineering tools through CLI and MCP.

*Based on author and project reports; not independently reproduced here. Evidence and project status are recorded in each case.*

![Cumulative case collection growth, by day](assets/case-growth.en.svg)

## Recent picks

**10 worth reading**: recover a compiler, query an existing circuit, control a keyboard without its Windows utility—or learn from an unresolved video-analysis attempt. These picks favor concrete engineering and inspectable evidence over blanket replacement claims. Dates identify sources or author updates, not collection dates.

1. **[borland-reborn: recover a 1991 compiler](cases/en/borland-reborn-bcc20-exhume-byte-matching.md)** · `2026-11-14` report and pinned docs — Exhume's Claude Code skills support **reportedly byte-identical BCC.EXE/CPP.EXE rebuilds**. A separate modding build has 1,836 compile comparisons and 83% coverage, not every path or uniquely recovered original source. Not rebuilt here. `Unverified here`
2. **[Proteus: ask Claude about an existing circuit](cases/en/arpit-proteus-pdsprj-mcp-project-research.md)** · `2026-11-17` author thread — Arpit researches **undocumented .pdsprj files for an MCP bridge**, reporting schematic queries, connection tracing, value edits and bills of materials. Placement and wiring remain planned; headless simulation returns no waveforms. Thread read, code and circuits not tested here. `In progress`
3. **[Darmoshark TOP75: keyboard control on Mac](cases/en/darmoshark-top75-macos-ai-protocol-report.md)** · `2026-11-18` author reply and pinned docs — **AI-assisted Windows-utility research plus IOKit checks** support RGB, remapping, macros and lights-off scheduling over Bluetooth. Project docs record readback, rollback and failed writes; display uploads use USB and on-device GIF playback remains unvalidated. Not tested here. `Unverified here`
4. **[Horizon: Minecraft Java behavior, rebuilt in Rust](cases/en/horizon-minecraft-java-rust-ai-differential-reimplementation.md)** · `2026-11-16` report and pinned docs — **AI-assisted reconstruction with 281 reported differential harnesses**, existing saves and vanilla multiplayer. Public docs and a Codex-credited commit were read, not the full test results; performance claims are hardware-specific. Own game required; not built here. `In progress`
5. **[Fallout Van Buren: six years of research meet REA](cases/en/fallout-van-buren-kran-rea-human-guided-reconstruction.md)** · `2026-11-14` author thread — Kran credits **manual research, shenmarukai's decompilation and an IDA database**, not a from-zero agent. DX9 migration is reported; 64-bit remains a goal for this tech demo, not a complete game. Not built here. `In progress`
6. **[Lemmings for Windows 95: match functions, not headlines](cases/en/lemmings-win95-human-led-ai-reconstruction-report.md)** · `2026-11-12` report; `2026-11-09` pinned docs — Human-led REA/Claude/Codex work reports **696/696 functions matched across eight modules**. Whole EXE/DLL files still differ; portable builds and original-compiler matching are separate. Own assets required; not built here. `In progress`
7. **[Mario Kart World: translate code, measure each change](cases/en/mkw-recomp-claude-aarch64-c-port.md)** · `2026-11-14` report and pinned docs — **Claude-assisted AArch64-to-C, same-run A/B and console-image checks** bring reported PC racing. Not original-source recovery; menus, AMD hangs and no online play remain. Own game required; not built here. `In progress`
8. **[X6200: update the radio without swapping back to stock](cases/en/x6200-claude-base-firmware-upgrade-reimplementation.md)** · `2026-11-16` report and PR merge — **Claude-assisted reconstruction of Xiegu's updater** reaches OpenX6X00. The project CI passed; the author reports upgrades and rollback on one radio. No flash readback, recovery not hardware-tested, and no reproduction here. `Unverified here`
9. **[Fireface UCX: Linux control beyond basic USB audio](cases/en/johan-fireface-ucx-linux-rea-claude-driver.md)** · `2026-11-15` author article — Johan reports **REA/Claude driver research, a terminal mixer and 3.5 ms round-trip audio at 48 kHz**. Community command-format research and a week of hands-on checks matter; tested on one first-generation unit, not reproduced here. `Unverified here`
10. **[rea-video: a convincing explanation still did not explain the trick](cases/en/pamela-rea-video-codex-food-video-analysis-failure.md)** · `2026-11-17` author report — Pamela asks **Codex to decode seamless food-video edits**, then requests diagrams and more concrete images. Several rounds leave the filming method unresolved; she says the model also admits failure. One reported attempt, not a general verdict; video and session unchecked here. `Failed attempt`

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
| [Games & preservation](categories/en/games.md) | **474** |
| [Hardware & interoperability](categories/en/hardware.md) | **644** |
| [Applications & clients](categories/en/apps.md) | **1014** |
| [Algorithms & feature recovery](categories/en/algorithms.md) | **293** |

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
