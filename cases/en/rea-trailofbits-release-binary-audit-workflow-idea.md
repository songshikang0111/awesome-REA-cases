# REA plus Trail of Bits skills: Archive proposes seven audit roles for release binaries

Category: Applications and clients · REA
Record date: 2026-11-25
Stage: Needs verification

At 01:37:34 Beijing time on November 25, 2026, Archive (@ArchiveExplorer) proposes putting REA before Trail of Bits skills in Claude Code to inspect one's own release binary and closed SDKs. Seven roles are named: dwarf-expert for DWARF information, zeroize-audit for secret zeroization, firebase-apk-scanner for Firebase configuration, burpsuite-project-parser for existing Burp records, constant-time-analysis for timing issues, audit-context-building for function assumptions, and yara-authoring for detection rules. This is a concrete owned-build audit idea, not seven discovered vulnerability classes.

Supplementary reading of trailofbits/skills' public main README confirms these plugin names, the Claude Code marketplace entry and their stated purposes. It is a mutable document read after this window, not a pinned candidate-time revision. The README limits zeroization work to C/C++ and Rust; DWARF analysis needs relevant target information and Burp parsing needs captured projects. This cannot be generalized to fully automatic, source-free auditing of any stripped application. The document does not validate the REA combination; 99 skills, five-minute setup and entirely free operation were not checked. No skills, build or findings were tested. Model/API costs are separate, and replacing a security team is promotion rather than an experimental conclusion.

Sealed candidate: 19 likes, 1,346 views, 5 reposts, 0 replies. The 99 skills, zero cost and five minutes are promotional figures, not checked counts or timings.

## Sources

- [Archive's REA/Trail of Bits release-build audit idea, November 25, 2026 at 01:37:34 Beijing time](https://x.com/i/status/2125282694372180094)
- [Supplement: Trail of Bits Skills public main README read after this window; neither a pinned revision nor combined-workflow verification](https://github.com/trailofbits/skills/blob/main/README.md)

[中文](../rea-trailofbits-release-binary-audit-workflow-idea.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
