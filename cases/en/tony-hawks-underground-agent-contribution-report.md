# Tony Hawk's Underground: agents contribute functions, deterministic gates merge them without AI

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-12
Stage: In progress

At 16:30:18 Beijing time on November 12, 2026, yibie (@yibie) introduces andrewnakas/thug-decomp: humans and AI can contribute, but AI is not involved in merging. Supplementary README and START_HERE reading is pinned to dba7457cf8ea3bad7af718db46c2876863e1f36b, committed November 7 at 12:09:30 Beijing time before the candidate. The target is the NTSC-U SLUS-20731 release of Neversoft/Activision's 2003 PS2 game Tony Hawk's Underground, reconstructing matching C++ function by function for preservation and study.

The docs specify SN Systems ee-gcc 2.95.3, SN BUILD 1.36, and 11,438 functions split using splat/spimdisasm. The complete ELF reportedly rebuilds byte-identically from C++ plus assembly; this does not mean all 11,438 functions are C++. Current C++ progress is delegated to a live tracker whose percentage was not retrieved here. The candidate's 9,252 files is the roundup author's count, not matched functions, and the tree total was not checked.

START_HERE supplies an agent protocol: read rules, avoid leaked source, bring a disc, claim unoccupied addresses, draft/compare/fix functions, and submit PRs containing at most 20 functions. A first PR needs the maintainer's judge-ok label; a local Decompathon Steward then judges and merges automatically. No AI in merging therefore does not mean a person clicks every merge. README lists five deterministic gates: pinned-toolchain validation, scanning against shortcuts such as inline assembly, split integrity, instruction matching, and whole-ELF hash plus objdiff comparison. Public CI only runs checks that do not require the disc.

This is a concrete bounded collaboration design for agent contributions, not a cloud model inventing a whole game or unreviewed code acceptance. Only documentation was read; actual PRs, Steward implementation, agent logs and gates were not audited or run. No disc, compiler or game files were obtained. REA is not identified. Work remains in progress with project-reported matching limits.

Sealed whole post: 3 likes, 275 views, 0 reposts, 1 reply. The candidate's 9,252 files is not completion progress. No independent build result.

## Sources

- [yibie on THUG human/agent contributions and non-AI merging, November 12, 2026 at 16:30:18 Beijing time](https://x.com/i/status/2120796315898777815)
- [Supplementary pinned THUG README committed November 7, 2026 at 12:09:30 Beijing time, before the candidate](https://github.com/andrewnakas/thug-decomp/blob/dba7457cf8ea3bad7af718db46c2876863e1f36b/README.md)
- [START_HERE at the same pinned commit: bring a disc, agent contributions and first-PR approval](https://github.com/andrewnakas/thug-decomp/blob/dba7457cf8ea3bad7af718db46c2876863e1f36b/START_HERE.md)

[中文](../tony-hawks-underground-agent-contribution-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
