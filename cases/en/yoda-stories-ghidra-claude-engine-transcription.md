# Yoda Stories: Ghidra and Claude transcribe the engine; byte matching pauses and SDL work continues

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-20
Stage: In progress

At 22:01:51 Beijing time on November 20, 2026, whyamas (@whyamas) introduces @ShinyQuagsire's Claude-led Yoda Stories engine decompilation from Ghidra and a plan file, reporting complete C++ transcription and an SDL port in progress. Supplementary reading used shinyquagsire23/Yodecomp at 850368bc1727dcf2f690d78b10fc1fcd1c09f453, committed September 9 at 11:36:13 Beijing time. This is pre-window project documentation, not a new November completion.

README reports 100% engine transcription into idiomatic C++ and building an EXE from source. Claude paused byte matching after spinning its wheels and is porting to SDL through microfx, replacing MFC and parts of GDI. The 100% is a claimed transcription scope, not 100% byte matching or validated complete behavioral equivalence. Builds require user-supplied game assets and toolchains; none were obtained or built here.

The author describes giving Opus game assets, Yodesk.exe loaded in Ghidra, decompiler access through MCP/curl, OpenJKDF2 and DesktopAdventures references and an initial CLAUDE.md plan. The quoted plan instead names YodaDemo.exe; the differing documented names are retained rather than silently normalized. Claude mostly steered, but the author corrected confidently wrong names, required structs documented in Ghidra rather than only Markdown and manually drove a phased pickup protocol allowing empty-context continuation, occasionally using Fable. This was not an unsupervised automatic loop. Only README was read, not all source, video or test logs; all-path usability of the transcription or SDL port is not confirmed. REA is not mentioned.

Candidate snapshot: 0 likes, 5 views, 0 reposts, 0 replies. 100% transcription is a project report, not byte matching; human supervision and matching stagnation are retained.

## Sources

- [whyamas introduces Yoda Stories/Claude, November 20, 2026 at 22:01:51 Beijing time](https://x.com/i/status/2123778852669554700)
- [Supplement: pinned Yodecomp README, September 9, 2026 at 11:36:13 Beijing time](https://github.com/shinyquagsire23/Yodecomp/blob/850368bc1727dcf2f690d78b10fc1fcd1c09f453/README.md)

[中文](../yoda-stories-ghidra-claude-engine-transcription.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
