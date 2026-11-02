# The House of the Dead ReWrithe: Claude-assisted arcade/PC logic merger, with platform-testing limits

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-02
Stage: In progress

At 18:14:38 Beijing time on November 2, 2026, the candidate introduces TawhidI-602 (Tawhid)'s The House of the Dead: ReWrithe, a C++ rewrite combining SEGA's 1996 arcade game and 1998 PC release. It advertises widescreen, four-player co-op, controllers and light guns, with Windows/Linux/Steam Deck/macOS builds. The goal is preserving the original for modern hardware; users need their own Revision A arcade ROMs and 1998 PC files.

Supplementary public README reading pins commit 081fe6a651dbc4c43779f5ced65e705f853466ab, dated 2026-11-01T16:23:10Z, or November 2 at 00:23:10 Beijing time, before the candidate. The project explicitly credits Claude with reverse engineering, rewriting and combining existing code under the author's direction and testing. Translations are machine-made; it does not claim AI-generated game artwork. Version 1.0.0 is still a first release. Many routines without capture proofs remain marked UNVERIFIED, with 45 listed, while the PC prologue and route-map walker remain partial.

The README reports zero differing frames in one/two-player MAME replays through all four arcade chapters, the final boss and ending; it also reports 17,289 equal frames for PC Mode Chapter 1 and no differences in 321 THOTD.EXE routines. These are project-run automated comparisons, not reruns here. A human completed the arcade campaign on a Surface Pro 7 on October 21, 2026. The matrix explicitly limits networking to multiple copies on one PC: two real PCs and internet play are untested. Light guns and many pads have simulated-input tests only. Linux has WSL headless testing, not a real Steam Deck. Although macOS has a listed CI build path, the matrix also says never built or run and the roadmap remains unchecked; the candidate's all-platform language is not compatibility proof.

Four-player support is experimental. Most AMD/Intel and old GPUs need testing. Initial DualSense aiming was described as clunky, with revised feel untested, and machine translations await native readers. The public implementation and layered testing are worth retaining, but zero-difference figures do not establish whole-game, all-mode or all-platform equivalence. No assets were downloaded and no game was compiled or executed.

Candidate snapshot: 0 likes, 225 views, 0 reposts. No independent rebuild; project-reported replay results are not whole-game proofs.
The supporting README predates the candidate and includes historical tests such as October 21 and 27, 2026, not additional new candidates.
Platform support, real light guns, two-device networking and macOS builds/execution have explicit evidence gaps.

## Sources

- [Candidate: ReWrithe and Claude-assisted development report, November 2, 2026](https://x.com/i/status/2117198692591575352)
- [Supplementary pinned README: AI roles, replays and human/automated/untested matrix, November 2, 2026 at 00:23:10 Beijing time](https://github.com/TawhidI-602/The-House-of-the-Dead-ReWrithe/blob/081fe6a651dbc4c43779f5ced65e705f853466ab/README.md)

[中文](../house-of-the-dead-rewrithe-claude-cpp-rewrite.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
