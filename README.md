<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

**English (default)** | [简体中文](README.zh-CN.md)

### Explore software and hardware with AI.

A curated collection of **reverse-engineering projects, experiments, and ideas**: revive old devices, rebuild apps, preserve games, and understand hidden behavior.

# 1384 cases & projects

**Latest case update:** November 1, 2026, 00:16 · **Last maintained:** November 1, 2026, 00:16 · Beijing time (UTC+8). Counts as of this maintenance.

Updates **6× daily** · [Full index](INDEX.en.md) · [Browse categories](#browse-by-category)

Covers [REA](https://github.com/morluto/rea) and other AI-assisted work. REA connects coding agents to local reverse-engineering tools through CLI and MCP.

*Based on author and project reports; not independently reproduced here. Evidence and project status are recorded in each case.*

![Cumulative case collection growth, by day](assets/case-growth.en.svg)

## Recent picks

**10 worth reading** for device interoperability, useful replacements, game preservation and binary analysis. These picks favor inspectable implementations and explicit test limits; a widely shared claim alone does not establish a working replacement. Dates below are source or author-update dates, not collection dates.

1. **[tolpo: a live 3D view of your Tapo home](cases/en/tolpo-tapo-claude-lan-3d-home-report.md)** · `2026-10-29` — A Claude-assisted protocol-research report leads to **public LAN/MCP control and a human-corrected floor plan**. Reuses python-kasa; earlier project tests cover nine rooms and 18 devices, not every write or model. Local device traffic does not mean local AI. `In progress`
2. **[hexgrab: learn from PowerToys, then build a smaller picker](cases/en/hexgrab-powertoys-colorpicker-rea-study.md)** · `2026-10-29` report; `2026-10-12` investigation — Claude/REA studies shipped binaries; the author's source scorecard gives **8 of 9 claims fully correct, one partial**. Public .NET 10 implementation; hotkey registration in an unexamined runner exposed a blind spot. One monitor tested, not independently rerun. `Analysis test`
3. **[scapectl: control a Fractal Scape headset without the web app](cases/en/scapectl-fractal-scape-claude-usb-hid.md)** · `2026-10-29` — **Claude Code-assisted USB HID research and a public Go tray app/CLI** for status, EQ presets and device events. Documents hardware corrections to source labels; macOS/Windows project-tested, Linux untested. Unsigned/unnotarized; not run here. `In progress`
4. **[Where NIST curve seeds came from](cases/en/nist-ecdsa-origin-claude-report.md)** · `2026-10-16` — Anthropic reports Claude traced public parameters to **lrand48 and timestamps**, publishing code and unresolved questions. **Not an ECDSA break**; not independently recomputed here. `Research report`
5. **[LG UltraFine: repair the updater, not the firmware](cases/en/lg-ultrafine-codex-updater-patch.md)** · `2026-10-19` — Codex-assisted diagnosis and a **public, exact-build memory patch**; the author reports a scaler update reaching **100% with CRC passing**. Credits an earlier bug report; one Apple Silicon setup, not independently flashed here. `Author-tested patch`
6. **[Brother: scan straight to your NAS](cases/en/brother-scan-button-claude-rea-server.md)** · `2026-10-18` — Replace the PC button app with a **public Claude/REA-assisted Go service for SMB, FTP, S3 and local storage**, building on prior protocol work. A server is still required; only MFC-L2800DW firmware 1.32 is project-tested. `Public implementation`
7. **[Claude writes proofs; Rocq checks the binaries](cases/en/anthropic-theorem-claude-binary-formal-verification.md)** · `2026-10-22` — Anthropic/Theorem report machine-code no-crash proofs for **239 entry points across 123 libraries**. Single-threaded static RISC-V/Linux, inputs below 64MB; **not bug-free whole libraries**, and the checker was not independently rerun here. `Analysis test`
8. **[OKOK Libre: keep your scale, replace the ad-heavy app](cases/en/okok-libre-rea-glm-scale-android.md)** · `2026-10-31` — JYunth credits REA/GLM with APK research and Opus with UI work; **public Android code covers three OKOK Bluetooth protocols**. The pinned main manifest has no internet permission, not a final-APK audit. Some scale families remain unsupported; formula equivalence and health estimates are unverified. `In progress`
9. **[X-Men 2: from Genesis to four-player PC co-op](cases/en/xmen2-pc-claude-genesis-native-port.md)** · `2026-10-31` report; `2026-10-28` project documentation — crabsmack credits Claude Code with a native Windows/Linux port, reporting **3,047 byte-matching C functions** plus instruction-level checks for 117 assembly functions. Adds rollback and widescreen; four-player modes are less tested. Bring your own ROM; not rerun here. `Public implementation`
10. **[Harvest Moon: readable C that also plays](cases/en/rodoly-harvest-moon-snes-ai-native-report.md)** · `2026-10-31` report; `2026-10-30` project documentation — RodoLy credits **human-supervised AI** and reports **778 routines / 45,176 instructions verified**, comparing memory and registers. Native-C beta adds optional widescreen and endless farming; picture/sound chips still run in software. Bring your own USA ROM and build locally; checks not rerun here. `Analysis test`

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
| [Games & preservation](categories/en/games.md) | **295** |
| [Hardware & interoperability](categories/en/hardware.md) | **370** |
| [Applications & clients](categories/en/apps.md) | **571** |
| [Algorithms & feature recovery](categories/en/algorithms.md) | **148** |

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
