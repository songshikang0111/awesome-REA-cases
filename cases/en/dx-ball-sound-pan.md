# DX-Ball: from a panning function to 270 matching game functions and a native Windows build record

Category: Games and preservation · REA
Record date: 2026-11-01

DX-Ball is a 1990s Windows brick-breaking game. An early REA contribution recovered its horizontal-position stereo-panning algorithm by following playback calls and using assembly, constants and callers to reconstruct C. The evidence records 3,205 differential tests against original x86 and recompilation matching the complete 63-byte function. This was one-function validation, not a complete game reconstruction at that time.

Japanese commentary at 14:10 Beijing time on October 19 cites October 7 progress: 528 Ghidra candidates included library code and were not the denominator for game completion; 55 functions were rewritten and 33 matched, with no complete playable build yet. This is a third-party account of earlier progress, no longer the current stage. Its separate Berman/Mario discussion is unrelated to DX-Ball validation.

At 12:48:33 on November 1, 2026, Tuoba Shu (@qwerty__cs) reports Codex using REA to call Ghidra, reconstructing typed C/C++ function by function from the English DX-Ball 1.07 EXE. Visual C++ 4.0 compilation and complete-function comparison guide corrections to types, control flow and memory layout, mapping relocated calls and data references back to original addresses. The report gives 270 non-runtime game functions and 84,968 matching bytes, with source recovery complete October 22 and native Windows build work added October 31.

Supplementary reading inspected N0zoM1z0/dx-ball's README and PLAYABILITY_20261031 at 36856cb0ab246e8727bed5ae9d58bf5ab5a72de7. Its commit is October 31 at 18:31:16 UTC, or November 1 at 02:31:16 Beijing time, before this window and supplementary only. The project reports 141 compiled C/C++ units and 270 matching functions across 53 closures. The native rebuild and October 22 tested executable are both 166,400 bytes, differing in 18 bytes across six PE/resource timestamp fields. This is not whole-EXE identity with the original retail file. Nineteen original CRT members are still linked and game assets must be supplied separately; MIT source licensing does not authorize redistribution of original files.

The October 31 report uses Europe/Berlin (UTC+1), so its 20261101 directory labels are not new-window experiments. New Wine/Xvfb checks cover basic play, editor save/reload, cnc-ddraw windowed operation and ranking persistence across restart. Windows 11 play without major problems is scoped manual user feedback, not another launch acceptance test of the newly rebuilt EXE. A fifteen-minute original-bank episode reaching board three, fifty editor-created one-brick boards and stereo results come from the retained October 22 record and were not repeated October 31. The original fifty-board campaign, every power-up in live play, exclusive-mode focus/surface recovery and complete native audio/MIDI/frame-pacing coverage remain unverified. The windowed wrapper fails the exclusive focus fixture; windowed play does not erase that limit. A limited sample records about 44.57 timer updates per second, median 17ms and 95th percentile 54ms, not GPU FPS or a fixed frame-pacing problem.

The older function-level finding and newer game-wide progress coexist with dates. These are project records and reporting, not this collection's independent reproduction. Only documents were read; no game acquisition, VC4 compilation, differential-test rerun or play occurred here.

New candidate snapshot: 0 likes, 124 views, 0 reposts. The game-function denominator excludes runtime code.
270 functions and 84,968 bytes are project matching results. The original fifty-board campaign and other checks remain pending; no independent rerun.
Supplementary project material predates this window. The 18-byte timestamp-only comparison is against the October 22 reconstructed test executable, not the original EXE.

## Sources

- [Case PR](https://github.com/morluto/rea/pull/876)
- [Evidence record](https://github.com/morluto/rea/blob/main/website/evidence/dx-ball-sound-pan.md)
- [October 19 commentary: single-function versus full-game verification, citing October 7 progress](https://x.com/i/status/2112063745824616946)
- [Tuoba Shu reports 270 matching functions and a native Windows build, November 1, 2026](https://x.com/i/status/2116754242870645169)
- [Supplementary: pinned README, commit October 31 at 18:31:16 UTC, before this window](https://github.com/N0zoM1z0/dx-ball/blob/36856cb0ab246e8727bed5ae9d58bf5ab5a72de7/README.md)
- [Supplementary: October 31 Europe/Berlin build and windowed-play report, pinned commit](https://github.com/N0zoM1z0/dx-ball/blob/36856cb0ab246e8727bed5ae9d58bf5ab5a72de7/docs/research/PLAYABILITY_20261031.md)

[中文](../dx-ball-sound-pan.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
