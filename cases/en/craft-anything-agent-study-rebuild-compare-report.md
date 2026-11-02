# Craft Anything: a Rust study-and-rebuild workbench with explicit limits on project-reported checks

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-02
Stage: In progress

At 09:51:48 Beijing time on November 2, 2026, Smartpig (@Smartpigai) introduces Craft Anything as studying a website, app or game, building a new project and comparing/refining it. At 11:15:23, mingzi206 promotes comprehensive automatic hooking, symbolic-execution architecture graphs and completion in minutes. A name lookup found the public storytold/craft-anything repository. This review read README and STATUS pinned to 32b80be89061896921d370e8f4f952ab707e2270, committed at 11:40:37 Beijing time that day. STATUS is dated November 2; its October 18 live runs and October 23 audit are earlier project records, not new experiments in this window.

The project describes a pure-Rust engine with 314 CLI/MCP tools, 298 in the engine itself, sharing a study/build/check/refine workflow between the desktop app and agents. Default Clean room mode uses visitor-visible UI, user pictures and descriptions and refuses internal reads; Deep permits code, files, website JavaScript and optional Ghidra. Building primarily invokes the user's own Claude Code; analysis can use APIs or local compatible services. A Codex adapter exists but is not verified on a real installation. Clean room is the project's mode name, not this collection's legal or clean-room-compliance certification.

STATUS reports October 18 Windows headless runs: a website at 96% likeness in 1.5 minutes; a small desktop app in 9 minutes, checked only by building; and a Rust game stopped at Build before Check. Website likeness is a project metric, not functional equivalence. Game self-tests are the generated build's own reports, not independently observed gameplay or measured values. Runtime study starts the original once to capture its window and UI tree rather than driving it over time; Frida sessions are partly simulated and no live full Clean room build has been run. These limits do not substantiate candidate generalizations about recording every syscall/memory transition or cloning arbitrary software in minutes.

The README labels the project early alpha and distinguishes working from partial components. Installer descriptions are not downloads or cross-platform tests by this collection. Only public documentation and commit metadata were read; no target or repository code, dependencies or author tests were executed. This entry is distinct from the ArtCraft app suite's Adobe-attribution dispute: common organizational ownership does not establish that those apps reverse-engineered Adobe.

Sealed candidate snapshots: Smartpig, 8 likes, 692 views, 2 reposts; mingzi206, 2 likes, 59 views, 0 reposts.
314 tools, 96%, 1.5 minutes, 9 minutes and audit tests are project reports, not independently reproduced. Real Codex installation, live Clean room builds and some dynamic analysis remain unverified.

## Sources

- [Candidate: Smartpig introduces the Craft Anything workflow, November 2, 2026](https://x.com/i/status/2117072151476080832)
- [Supporting candidate: mingzi206's Rust/dynamic-observation promotion, November 2, 2026](https://x.com/i/status/2117093182441972165)
- [Supplementary project README at a pinned November 2, 2026 commit](https://github.com/storytold/craft-anything/blob/32b80be89061896921d370e8f4f952ab707e2270/README.md)
- [Supplementary pinned STATUS, including October live runs and November 2 limitations](https://github.com/storytold/craft-anything/blob/32b80be89061896921d370e8f4f952ab707e2270/docs/STATUS.md)

[中文](../craft-anything-agent-study-rebuild-compare-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
