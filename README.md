<img src="assets/rea-banner.png" alt="REA Cases — AI + Reverse Engineering" width="1280">

# Awesome REA Cases

**English (default)** | [简体中文](README.zh-CN.md)

### Explore software and hardware with AI.

A curated collection of **AI-assisted reverse-engineering projects, experiments, and ideas** for device interoperability, app rebuilding and game preservation—including failed attempts and author corrections.

# 2213 cases & projects

**Latest case update:** November 14, 2026, 00:10 · **Last maintained:** November 14, 2026, 00:10 · Beijing time (UTC+8). Counts as of this maintenance; source dates and the continuous evidence cutoff are separate.

Updates **6× daily** · [Full index](INDEX.en.md) · [Browse categories](#browse-by-category)

Covers [REA](https://github.com/morluto/rea) and other AI-assisted work. REA connects coding agents to local reverse-engineering tools through CLI and MCP.

*Based on author and project reports; not independently reproduced here. Evidence and project status are recorded in each case.*

![Cumulative case collection growth, by day](assets/case-growth.en.svg)

## Recent picks

**10 worth reading**: connect devices, preserve games and test what reconstructed behavior actually matches. Protocol attribution and the limits of traffic-based inference matter as much as a working demo. Dates identify sources or author updates, not collection dates.

1. **[Fujifilm X half: camera to Mac without the phone](cases/en/fujifilm-x-half-opus-wireless-mac-import-report.md)** · `2026-11-12` author report — **Opus reportedly identifies Bluetooth/Wi-Fi protocol differences** for JPEG imports and Google Photos uploads. Incremental camera tests, not an iteration-free build; code and traces unchecked here. `Unverified here`
2. **[Anker recorder: ask an agent for last week's conversation](cases/en/berryxia-anker-recorder-rea-mcp-knowledge-app.md)** · `2026-11-12` author report — **REA Bluetooth research and MCP recording retrieval**, with local Qwen ASR or online transcription. Berryxia plans source release after refinement/testing; code and device path unchecked here. `In progress`
3. **[Lemmings for Windows 95: match functions, not headlines](cases/en/lemmings-win95-human-led-ai-reconstruction-report.md)** · `2026-11-12` report; `2026-11-09` pinned docs — Human-led REA/Claude/Codex work reports **696/696 matched functions across eight modules**. Whole EXE/DLL files still differ; portable builds and original-compiler matching are separate. Bring your own game assets; not built here. `In progress`
4. **[hexgrab: study PowerToys, build a smaller picker](cases/en/hexgrab-powertoys-colorpicker-rea-study.md)** · `2026-10-29` report; `2026-10-12` investigation — Claude/REA studies binaries; an author/source comparison finds **8 of 9 claims correct, one partial**. Hotkey registration in another binary exposed a blind spot. Public .NET 10 implementation, one monitor tested; not rerun here. `Analysis test`
5. **[ZigZag: from SVG to a Brother embroidery machine](cases/en/kath-korevec-brother-chatgpt-embroidery-report.md)** · `2026-11-13` report and pinned docs — **Skitch PP1 Bluetooth upload and MCP-assisted design**, with project-reported hardware tests. NOTICE credits the protocol to Respira; the earlier ChatGPT origin story remains secondary, not independent discovery. Not run here. `Unverified here`
6. **[MousePods: AirPods as a Linux mouse and head tracker](cases/en/airpods3-claude-remotehid-linux-head-mouse-report.md)** · `2026-11-11` reports; `2026-11-10` pinned docs — **Claude-assisted RemoteHID research and reported AirPods 3/Pro 2 hardware checks.** No earbud flash, but Proton integration changes prefixes. MTU/device-identity effects were not isolated; not run here. `Unverified here`
7. **[Fable animation: what browser traffic can—and cannot—show](cases/en/ganesh-fable-animation-rea-traffic-teardown.md)** · `2026-11-13` report, author clarification and pinned skill — **Claude/REA studies a story-generation run, retaining field names.** Ganesh explicitly says character-model training was inferred, not observed. Public workflow; raw traffic unchecked here. `Analysis test`
8. **[Ziliu: no detected keys is not a security proof](cases/en/ziliu-workbuddy-rea-client-exposure-self-test.md)** · `2026-11-13` author self-test — WorkBuddy/REA reportedly finds **178 channels and 337 calls**, leaving 42,352 unknown items and detecting no keys or core prompts. A bounded static-analysis account, not proof that client or server is safe; full report unchecked. `Analysis test`
9. **[TimeSplitters 2: PS2 behavior to a PC port](cases/en/destinity-timesplitters2-claude-native-pc-recompile.md)** · `2026-11-10` author report; `2026-11-09` pinned docs — **Claude-assisted MIPS-to-C++ with PCSX2 frame/state comparisons** and a reported Linux/Steam Deck first-level playthrough. Still uses PCSX2 graphics/audio; later levels and internet play need checks. Self-supplied disc; not built here. `In progress`
10. **[Empire Earth: a rebuilt engine playing the original](cases/en/empire-earth-ai-trailers-compatible-engine-report.md)** · `2026-11-12` report; `2026-11-08` pinned docs — Claude-credited history and project-reported **tick-by-tick comparisons plus mixed original/rebuilt TCP games without desync**. Whole images differ; WON services, audio and physical input are untested. No general source-license grant; not run here. `In progress`

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
| [Games & preservation](categories/en/games.md) | **439** |
| [Hardware & interoperability](categories/en/hardware.md) | **590** |
| [Applications & clients](categories/en/apps.md) | **920** |
| [Algorithms & feature recovery](categories/en/algorithms.md) | **264** |

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
