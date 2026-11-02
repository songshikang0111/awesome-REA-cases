# knife: Dopax describes a Rust multi-format static-analysis toolkit for agents

Category: Applications and clients · REA use unconfirmed
Record date: 2026-11-02
Stage: Related project

At 09:24:17 Beijing time on November 2, 2026, Dopax (@tensorstaff) introduces knife in a five-project open-source roundup: a terminal-first Rust reverse-engineering toolkit exposing CLI, TUI and MCP interfaces for agents. Claimed capabilities include PE/ELF/Mach-O/Wasm static analysis, mitigation audits, dangerous-API tracing and pseudocode. Its concrete purpose is making binary research available to terminal users and agents, not a completed reconstruction of a particular app.

Original-post lookup confirmed attribution. A name search found bl4ckr0ss3/knife, and the README was read at f260b87ffc54ae5c8c56cc31351334d209228745, committed October 16 at 04:25:49 Beijing time: earlier documentation, not a November 2 experiment. It describes static target reading without execution, the same engine exposed through MCP, and an investigation desk for local or compatible-API models. It explicitly lacks a Wasm lifter and refuses code views there; indirect dispatch is outside its direct call graph, so empty results do not establish unreachability. Unmodeled pseudocode remains verbatim. Reading documentation is not an implementation, safety or recovery-accuracy audit.

The reported 384 stars are the writer's November 2 GitHub-API snapshot, not independently checked or live popularity. Neither repository nor sample was run; equal functionality across formats and effective vulnerability discovery are not guaranteed. REA is unspecified; MCP support does not establish AI authorship of all development. RDX is recorded separately; SkillOpt, Ethproofs and solOS are not this reverse-engineering project.

Candidate snapshot: 0 likes, 21 views, 0 reposts. The reported 384 stars are the writer's November 2 figure, not independently checked.

## Sources

- [knife in Dopax's five-project roundup, November 2, 2026](https://x.com/i/status/2117065226063667699)
- [Earlier supplementary knife README at a pinned commit, October 16, 2026 Beijing time](https://github.com/bl4ckr0ss3/knife/blob/f260b87ffc54ae5c8c56cc31351334d209228745/README.md)

[中文](../knife-rust-static-analysis-mcp-secondary-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
