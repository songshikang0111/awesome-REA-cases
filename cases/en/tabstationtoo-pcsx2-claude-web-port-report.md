# TabStationToo: Claude-assisted work brings PCSX2 and four JITs into the browser

Category: Games and preservation · Other AI-assisted work
Record date: 2026-10-30
Stage: In progress

At 08:24:51 Beijing time on October 30, 2026, Bù Chī Pào Miàn (@paomiange1) introduces TabStationToo, saying two developers used Claude to move the open-source PS2 emulator PCSX2 into a browser: humans set architecture and run tests while the model replaces code. This adapts an existing emulator across platforms, not PS2 reversing from scratch, and retains credit for more than twenty years of PCSX2 work. The two-person division of labor remains secondary reporting without a complete development record.

Supplementary reading pins the README to c53f021af984438cd1fe07114f9710af77f5f4bd, committed at 04:36:17 Beijing time on October 30, before this window. That commit reports Tekken Tag Tournament increasing from 50% to 87% in Chrome and credits Claude Opus 5.5 as co-author, supporting AI involvement rather than sole authorship of the entire engineering effort. The README explicitly says early and experimental. It describes an Emscripten-compiled PCSX2 core, SharedArrayBuffer threads and runtime WebAssembly JITs for EE, IOP, VU0 and VU1, reportedly checked bit for bit against interpreters. WebGPU hardware rendering has a software fallback; audio uses Web Audio.

The project reports about 99% average emulation speed on foot in GTA San Andreas, 100% for Final Fantasy XII cutscenes and a Guitar Hero song at 100% with occasional dips in Chrome. These are bounded scene speeds, not full-speed compatibility for every game or a common frame rate. A heavy WWE scene needs a Ryzen 7 7840U at full power; Linux power management previously caused a 50–60% misreading, and most Linux Chromium GPUs lack WebGPU by default. Gamepads, browser memory cards and up to ten save states per game are documented, while phones, parent-dependent CHDs and multi-file BIN/CUE remain unsupported. JIT differential checks and benchmarks were not independently rerun.

Users must legally provide their own PS2 BIOS and game images. The README says those files stay local, but covers make external requests to ps2-covers, so the page is not wholly network-free. Deployment requires cross-origin isolation; opening HTML from disk is not supported. This collection only read public documentation and commit metadata, without downloading BIOS/game files, installing dependencies or running the port. Project validation is not independent reproduction.

Candidate snapshot: 1 like, 36 views, 0 reposts. Promotional engagement is not technical validation.
Pinned commit: 2026-10-29T20:36:17Z. The 99%/100% figures describe project-reported emulation speeds in selected scenes, not independent measurements.

## Sources

- [Secondary account of TabStationToo and Claude's role, October 30, 2026](https://x.com/i/status/2115963106681909434)
- [Pre-window pinned README: experimental status, architecture, test scope and local-file limits](https://github.com/TabStationToo/TabStationToo/blob/c53f021af984438cd1fe07114f9710af77f5f4bd/README.md)
- [Pre-window commit: Tekken performance claim and Claude Opus co-author credit](https://github.com/TabStationToo/TabStationToo/commit/c53f021af984438cd1fe07114f9710af77f5f4bd)

[中文](../tabstationtoo-pcsx2-claude-web-port-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
