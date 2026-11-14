# borland-reborn: Exhume-assisted Borland C++ 2.0 reconstruction, where matching bytes do not prove unique original source

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-14
Stage: Needs verification

At 18:32:55 Beijing time on November 14, 2026, a post in @huihoo's conversation introduces Abedegno's Exhume-assisted reconstruction of the 1991 Borland C++ 2.0 compiler. The target is preserving DOS command-line compiler BCC.EXE and standalone preprocessor CPP.EXE as readable C and assembly that rebuild with the original tools, and studying compiler internals. The candidate's claim of 100% recovery of all original source requires narrowing: byte identity supports an equivalent reconstruction, not recovery of the developers' original text, names or a unique source.

Public lookup found abedegno/borland-reborn. Its README was read at pinned commit 71530cb, timestamped November 14, 2026 at 11:10:44 UTC, later than the introduction but separately obtained supplementary documentation, not another candidate. It marks both BCC.EXE and CPP.EXE as whole-file byte-identical. The BCC section lists 298 sources: 265 C files and 33 handwritten TASM modules, preserving the original split rather than forcing existing assembly into C. About 3,100 functions/globals/labels, 300 fields, 40 layouts and about 10,000 comment lines describe the readability work, not independent proof of recovered original names.

The README describes a gate that recompiles, compares functions byte for byte, verifies relocations and names, then links the complete BCC.EXE. A separate modding build permits code growth and relocation, comparing outputs from 1,836 compiles with the original compiler and reporting 83% code coverage. Neither 1,836 independent user acceptance tests nor complete path coverage is established. The native bcc20-port has only started call recording, replay and initial runtime functions; it is not conflated with the reportedly matched DOS build as a finished native port.

Exhume's README explicitly identifies a toolkit plus Claude Code skills. Its pinned commit 1602022 is dated November 13, 2026 at 23:57:15 UTC, before this window, and only checks the AI-tool relationship. Borland's project distinguishes MIT scripts/documentation from recovered sources derived from Borland's copyrighted programs, with no rights claimed in those sources; users still supply original tools. No installation, target execution, compilation, 1,836-test comparison or hash check was performed here, and the technical findings were not exhaustively inspected. Included as a project report, not independent reproduction. REA is unmentioned.

Sealed candidate: 35 likes, 2,097 views, 6 reposts, 7 replies. The 298 sources, 1,836 compiles and 83% coverage are project statements, not rerun here.

## Sources

- [Borland C++ 2.0 and Exhume introduction, November 14, 2026 at 18:32:55 Beijing time](https://x.com/i/status/2121551947186704540)
- [Supplementary pinned borland-reborn README, commit November 14, 2026 at 11:10:44 UTC](https://github.com/abedegno/borland-reborn/blob/71530cbfe35cb6ed64892f7096b12da710939021/README.md)
- [Pre-window pinned Exhume README: Claude Code skills, commit November 13, 2026 at 23:57:15 UTC](https://github.com/abedegno/Exhume/blob/160202277647e7e97cca8a06e76184f88c573748/README.md)

[中文](../borland-reborn-bcc20-exhume-byte-matching.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
