# reverse-skill: investigation workflows for coding agents

Category: Applications and clients · REA use unconfirmed
Record date: 2026-11-04
Stage: Related project

An earlier post introduces reverse-skill for Codex, Cursor and Claude Code to choose tools for APK, frontend and firmware investigations. Four candidates at 12:19 Beijing time on October 20 explain that root AGENTS.md and RULES.md first require listing commands, writes, networking and global-configuration impacts for approval, then master-route selects one PRIMARY, case-init records authorization scope, and the specialized skill loads. Reading files, installing a plugin or supplying a sample path is not authorization; copying only the skills directory misses these entry rules. This orchestrates agent investigations rather than adding a decompilation engine or guaranteeing compliance.

Routing uses must, mustAll and exclude regular-expression rules, selecting PRIMARY by match count and priority, falling back to R0 without matches. Chinese and English jailbreak terms are disambiguated using mobile versus LLM context. Candidates report 178 bilingual routing cases and Windows/Ubuntu checks. Reading zhaoxuya520/reverse-skill's public README, AGENTS, benchmark JSON and bootstrap source confirms inspectable implementation and 178 cases, but this collection ran neither scripts nor CI. That count is not 178 successful reverse-engineering tasks. A local tool index records paths and versions; bootstrap prepares manifest-listed dependencies and does not register MCP by default. Writing Codex or Claude global configuration requires explicit selection. Version pinning and journal redaction are project designs, not this collection auditing all dependencies or secret removal.

The candidate proposes a purely offline trial with an owned APK, requiring scope creation and case-guard before touching the target, without a complete target-analysis acceptance record. Windows is the full main path, Kali has dedicated scripts, and macOS, Ubuntu and Debian have general support; IDA keep-alive scripts are Windows-only. No dependencies were installed, configuration changed or targets executed here. Platform parity and reliable handling of every format are not established. Repository identification resolves the earlier missing-implementation-link limitation. This remains a related workflow project, distinct from apk-reverse, with REA use unconfirmed.

A new post at 21:29:30 Beijing time on November 4, 2026 emphasizes choosing a methodology before invoking jadx, Frida or IDA, preserving experience for reuse, and reports 44 routing rules and 175 regression cases for Claude Code, Codex and Cursor. This is a new promotional count, without reading its corresponding pinned revision or running regression tests. It does not replace the 178-case benchmark observed in October or establish three deletions, regression in quality or 175 successfully reversed targets.

October 20's four candidate snapshots each have 0 likes and respectively 86, 118, 39 and 139 views. Public files were read statically; no target or workflow was executed.
New November 4 sealed post: 2 likes, 83 views, 0 reposts. The 44 rules/175 cases are new self-reports, not rerun, distinct from the earlier 178-case benchmark.

## Sources

- [Earlier project introduction](https://x.com/i/status/2110680583634366777)
- [October 20, 12:19: routing rules and 178 benchmark cases](https://x.com/i/status/2112398152686829612)
- [Same thread: authorization, PRIMARY and plugin boundaries](https://x.com/i/status/2112398151613100171)
- [Same thread: tool index and explicit MCP registration](https://x.com/i/status/2112398154788213150)
- [Same thread: offline samples and unequal platform support](https://x.com/i/status/2112398155400552729)
- [Public repository: read-only inspection of documentation, benchmarks and bootstrap](https://github.com/zhaoxuya520/reverse-skill)
- [New post: 44 rules, 175 regression cases and experience reuse, November 4, 2026](https://x.com/i/status/2117972508905459981)

[中文](../reverse-skill-agent-workflows.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
