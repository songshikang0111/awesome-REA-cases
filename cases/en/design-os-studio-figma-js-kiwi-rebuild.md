# DESIGN:OS Studio: reported REA research on Figma JS and .fig, with a public native Rust designer

Category: Applications and clients · REA
Record date: 2026-11-11
Stage: In progress

At 16:30:17 Beijing time on November 11, 2026, yibie (@yibie) introduces DESIGN:OS Studio in a daily roundup, saying it used REA to study Figma desktop JavaScript and the .fig v106 kiwi schema before reimplementing the desktop tool. The goal is local design-file ownership and a native designer agents can operate, not recovery of all Figma source. The same post also covers MK64 on PS3, a separate target with its own record.

Supplementary review covers the maintainer's PR #7 in yibie/awesome-rea and pinned E1-4 specification. The PR opened November 10 at 22:51:19 Beijing time and merged November 11 at 13:35:36, both before the window. The spec is pinned at df14c593e86edcc039adc2c67067bf8db64e9e84, committed November 10 at 21:44:10, with internal research dated October 18 and an October 19 revision. None is a new experiment in this window. It explicitly records REA 6.7.0 running analyze-javascript-application on extracted Figma cached JS. Without WABT or Ghidra, wasm analysis lanes were unavailable; a 40-line kiwi schema reader instead decoded the wasm data section. The author reports 653 definitions and a v106 .fig sample with 56,625 nodes, comparing style-variable bindings and separating observations from an inferred fontStyle string binding. Full raw REA reports were not obtained and fields were not recomputed. The spec's facts remain project research records, not proof REA alone performed all parsing.

Relevant README sections were also read at 1cc765bca900e187431d079f892f402cbaa200c7, dated November 11 at 19:45:34 Beijing time, after the candidate. They describe Rust/wgpu and tiny-skia, local .fig read/write with container-v106 output, a panel running the user's own agent CLI and stdio MCP. More than 6,000 macOS CI tests and large-file measurements are project claims; CI logs, implementation and reruns were not audited.

The README states there is no real-time cloud multiplayer or enterprise cloud administration. Known .fig save losses include numbered-list formatting and inherited or variable-bound instance paints becoming fixed values. Release notes and older issue lists are partly inconsistent; newer fix paragraphs do not establish that all save issues are resolved. Windows CI failed for v0.7.11 and Windows testing is advisory; pre-release verification centers on macOS. Built Linux packages do not establish interactive testing. Agents bill through their own plans; no extra Studio API key does not mean free model use. The current license is source-available PolyForm Shield 1.0.0, not generically OSI open source; the docs say releases through v0.5.0 retain MIT or Apache terms. No target was run, dependencies installed or Figma outputs compared here, and full functional equivalence is not established.

Whole-roundup sealed snapshot: 2 likes, 249 views, 0 reposts, not this project's engagement. PR state is a retrieval snapshot, not full functional validation.

## Sources

- [yibie's roundup on Figma JS, kiwi v106 and REA research, November 11, 2026 at 16:30:17 Beijing time](https://x.com/i/status/2120433924434452690)
- [Supplementary project README features and limitations, pinned to November 11, 2026 at 19:45:34 Beijing time](https://github.com/jangtrinh/design-os-studio/blob/1cc765bca900e187431d079f892f402cbaa200c7/README.md)
- [Supplementary E1-4 original specification: October 18–19 REA research, pinned to a pre-window November 10 commit](https://github.com/jangtrinh/design-os-studio/blob/df14c593e86edcc039adc2c67067bf8db64e9e84/docs/specs/v0.6/E1-4-styles-hold-variable-aliases.md)
- [Supplementary maintainer PR #7: opened November 10, 2026 and merged November 11 before the window](https://github.com/yibie/awesome-rea/pull/7)

[中文](../design-os-studio-figma-js-kiwi-rebuild.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
