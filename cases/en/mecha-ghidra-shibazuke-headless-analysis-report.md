# mecha_ghidra: shibazuke reports Docker/MCP binary analysis, with documentation clarifying its limits

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-26
Stage: Needs verification

At 22:06:49 Beijing time on November 26, 2026, the second project in shibazuke's (@shibazukesec) two-tool introduction is mecha_ghidra. The author says a personal Docker/MCP trial let an agent load, decompile and analyze a binary without opening a GUI. The post lists multiple-target switching, BSim similar-function search and handling long outputs. This is a personal trial on an unnamed target, not independently accepted code recovery, and it is separate from Binary Ninja MCP in the same post.

Supplementary reading pins ghidra-user-jp/mecha_ghidra's README to 7ff4264d07c52572b2c555a82044d38ad7877558, committed October 26, 2026 at 12:19:58 UTC (20:19:58 Beijing time), before this window. This is project documentation, not another candidate. It describes a standalone MCP server accessing Ghidra APIs through PyGhidra while the agent chooses the analysis steps. Names, types and comments can be edited, changes undone and programs exported; Ghidra Server shares results for humans to continue in the GUI, while BSim finds similar functions in registered binaries. Large results use pagination/search for selective retrieval, not proven lossless semantic compression.

Local analysis needs neither Server nor BSim. Shared editing uses checkout/check-in and does not support headless conflict merging. Starting the server does not create a project or import a file, and loading never analyzes: unanalyzed programs need a separate analyze_program call. The README lists Python 3.10+, uv, a compatible JDK and Ghidra, with native builds currently targeting 12.2. These are dependency descriptions, not installations performed here. It names Apache 2.0; LICENSE was not separately reviewed. The trial's sample hash, model, call logs, accuracy and analysis results are absent. Only documentation was read; Docker, full source review and reruns were not performed. Correct automatic analysis, no side effects and vulnerability detection are not certified. REA is unmentioned.

Shared sealed post: 2 likes, 93 views, 1 repost, 0 replies. Docker trial is author-reported, not rerun by this collection.

## Sources

- [Second project in shibazuke's post: personal mecha_ghidra trial, November 26, 2026 at 22:06:49 Beijing time](https://x.com/i/status/2125954431783145732)
- [Supplementary pinned README: PyGhidra, BSim and loading/analysis boundaries; committed October 26, 2026 at 12:19:58 UTC, before the window](https://github.com/ghidra-user-jp/mecha_ghidra/blob/7ff4264d07c52572b2c555a82044d38ad7877558/README.md)

[中文](../mecha-ghidra-shibazuke-headless-analysis-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
