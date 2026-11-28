# Codex 0.169.0 computer use: separating source observations from closed-executor reports

Category: Applications and clients · REA use unconfirmed
Record date: 2026-11-28
Stage: Analysis test

A long post at 10:08:18 Beijing time on November 28, 2026 reports inspecting a local Codex 0.169.0 source mirror at d32063f9 to understand its alternative to repeated screenshot-and-click operations. The author's source observations are that Rust tool handlers contain no low-level screenshot, click or keyboard executor; models.json uses code_mode_only and flags such as node_repl_disabled for newer models except the older gpt-5.5; and connectors recognize a persistent cua_repl/node_repl by name. Screenshots pass through nodeRepl.emitImage to a cloud model rather than JavaScript interpreting them locally. Batched asynchronous JavaScript with screenshots only at checkpoints is the author's explanation for fewer round trips, not a measured speedup.

The post describes the open Rust side as a safety shell: Windows application allow/deny rules by AUMID or publisher/product/binary name; a separate Guardian review model for login, sensitive data and permission actions, with about 11KB of risk-classification prompts; and separation of screenshots and review context. SkyComputerUseService, persistent JavaScript, combined macOS Accessibility/Windows UI Automation and screenshot channels, and Mac-background versus Windows-foreground operation are separately attributed to community analysis and documentation feedback, not directly proven by that source tree.

The reuse idea is wrapping an existing desktop driver with persistent JavaScript, accessibility trees, app allowlists and independent high-risk-action review, not copying a closed binary or GPT's native trained capability. No public mirror, file/line references, original community sources, execution traces or benchmarks were supplied. This collection did not independently inspect that revision, audit the closed service or run a client. Model names, flags and platform differences remain author reports. Included as AI-tool architecture research, without establishing AI-assisted source reading. REA is unknown.

Sealed candidate: 16 likes, 358 views, 8 reposts, 7 replies. No reproducible performance comparison was supplied.

## Sources

- [Codex 0.169.0 d32063f9 source and closed computer-use architecture analysis, November 28, 2026 at 10:08:18 Beijing time](https://x.com/i/status/2126498386732056717)

[中文](../codex-01690-cua-repl-source-architecture-analysis.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
