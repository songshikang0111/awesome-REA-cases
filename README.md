<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

**English (default)** | [简体中文](README.zh-CN.md)

### Explore software and hardware with AI.

A curated collection of **AI-assisted reverse-engineering projects, experiments, and ideas** for device interoperability, app rebuilding and game preservation—including failed attempts and author corrections.

# 2249 cases & projects

**Latest case update:** November 14, 2026, 20:15 · **Last maintained:** November 14, 2026, 20:15 · Beijing time (UTC+8). Counts as of this maintenance; source dates and the continuous evidence cutoff are separate.

Updates **6× daily** · [Full index](INDEX.en.md) · [Browse categories](#browse-by-category)

Covers [REA](https://github.com/morluto/rea) and other AI-assisted work. REA connects coding agents to local reverse-engineering tools through CLI and MCP.

*Based on author and project reports; not independently reproduced here. Evidence and project status are recorded in each case.*

![Cumulative case collection growth, by day](assets/case-growth.en.svg)

## Recent picks

**10 worth reading**: control your devices, preserve old tools and games, and see what the tests actually establish. Dates identify sources or author updates, not collection dates.

1. **[borland-reborn: recover a 1991 compiler](cases/en/borland-reborn-bcc20-exhume-byte-matching.md)** · `2026-11-14` report and pinned docs — Exhume's Claude Code skills support **reportedly byte-identical BCC.EXE/CPP.EXE rebuilds**. A separate modding build has 1,836 compile comparisons and 83% coverage, not every path or uniquely recovered original source. Not rebuilt here. `Unverified here`
2. **[Ember mug: probe Bluetooth, build a personal controller](cases/en/dmitriy-ember-mug-codex-bluetooth-probing-report.md)** · `2026-11-14` author report — Dmitriy says **Codex probed characteristics against the iOS app** and built temperature/light controls in about an hour. The no-web rule was author-imposed; coffee-level accuracy and code unchecked. `Unverified here`
3. **[Fujifilm X half: camera to Mac without the phone](cases/en/fujifilm-x-half-opus-wireless-mac-import-report.md)** · `2026-11-12` author report — **Opus reportedly identifies Bluetooth/Wi-Fi differences** for JPEG imports and Google Photos uploads. Incremental camera tests, not an iteration-free build; code and traces unchecked here. `Unverified here`
4. **[Anker recorder: ask an agent for last week's conversation](cases/en/berryxia-anker-recorder-rea-mcp-knowledge-app.md)** · `2026-11-12` author report — **REA Bluetooth research and MCP recording retrieval**, with local Qwen ASR or online transcription. Source release is planned after refinement/testing; code and device path unchecked here. `In progress`
5. **[Fallout Van Buren: six years of research meet REA](cases/en/fallout-van-buren-kran-rea-human-guided-reconstruction.md)** · `2026-11-14` author thread — Kran credits **manual research, shenmarukai's decompilation and an IDA database**, not a from-zero agent. DX9 migration is reported; 64-bit remains a goal for this tech demo, not a complete game. Not built here. `In progress`
6. **[Lemmings for Windows 95: match functions, not headlines](cases/en/lemmings-win95-human-led-ai-reconstruction-report.md)** · `2026-11-12` report; `2026-11-09` pinned docs — Human-led REA/Claude/Codex work reports **696/696 functions matched across eight modules**. Whole EXE/DLL files still differ; portable builds and original-compiler matching are separate. Own assets required; not built here. `In progress`
7. **[Mario Kart World: translate code, measure each change](cases/en/mkw-recomp-claude-aarch64-c-port.md)** · `2026-11-14` report and pinned docs — **Claude-assisted AArch64-to-C, same-run A/B and console-image checks** bring reported PC racing. Not original-source recovery; menus, AMD hangs and no online play remain. Own game required; not built here. `In progress`
8. **[Donkey Kong Bananza: a Switch 2 game on PC](cases/en/dkb-pc-recomp-claude-switch2-port.md)** · `2026-11-14` report; `2026-11-13` pinned docs — **Claude Code work checked with game runs and Unicorn comparisons**, built on TotK Recomp and community shader research. GPU crashes and later-area defects remain; Linux/macOS are previews. Own game required; not built here. `In progress`
9. **[decompdecomp: byte matching with an assembly fallback](cases/en/decompdecomp-local-agent-byte-matching-workbench.md)** · `2026-11-14` report; `2026-11-13` pinned docs — **Agents write C/C++, original compilers judge the bytes.** No whole game is reported decompiled; exports retain assembly, and cloud models may receive game material. Not run here. `In progress`
10. **[Smart bead board: an APK to a Raspberry Pi controller](cases/en/smart-bead-board-claude-raspberry-pi-mcp-control-report.md)** · `2026-11-14` author report and clarification — Labelray says **Claude decompiled the official APK for the protocol**, then wrote MCP tooling to light selected positions without the app. Model, transport and code are undisclosed; no device test here. `Unverified here`

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
| [Games & preservation](categories/en/games.md) | **449** |
| [Hardware & interoperability](categories/en/hardware.md) | **597** |
| [Applications & clients](categories/en/apps.md) | **936** |
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
