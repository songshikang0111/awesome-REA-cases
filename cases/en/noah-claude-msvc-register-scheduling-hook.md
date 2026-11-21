# An MSVC decision observer: Noah credits Claude with a hook used for Fallout matching decompilation

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-21
Stage: Needs verification

At 23:27:02 Beijing time on November 21, 2026, Noah (@Noah64165746) introduces a hook into Microsoft's C++ compiler and credits Claude with its implementation. Rather than directly translating a game into source, it reports why the compiler selects registers and how it schedules instructions, providing information for matching decompilation that must reproduce original compiler output. The author says the Fallout matching decompilation team has made good use of it, but supplies no count of additional matched functions or project completion attributable to the tool.

The same author's 23:31:59 reply says it supports MSVC 2003, 2005, 2008 and now 2012, with helper tools modeling the behavior at 97% accuracy for register selection and 98% for instruction scheduling order. These are author reports, not measurements by this collection. Sample size, test set, compiler flags, accuracy definitions and per-case results were not obtained; the numbers cannot be extended to all compiler versions or the entire Fallout reconstruction.

The thread includes a shortened link, but no identifiable repository or source was obtained and neither hook nor compiler was run. Claude attribution is explicit, while model, human edits and development time are unspecified. REA is unmentioned. Retained as an unverified report of a concrete matching-decompilation aid. The supplementary reply is not a new candidate.

November 21 candidate snapshot: 0 likes, 6 views, 0 reposts, 1 reply. The thread's 97%/98% figures are self-reported, not independently verified.

## Sources

- [Noah introduces the Claude compiler hook, November 21, 2026 at 23:27 Beijing time](https://x.com/i/status/2124162678688289138)
- [Same-author reply on MSVC versions and accuracy, November 21, 2026 at 23:31 Beijing time](https://x.com/i/status/2124163926539559412)

[中文](../noah-claude-msvc-register-scheduling-hook.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
