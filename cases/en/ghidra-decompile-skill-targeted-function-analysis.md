# ghidra-decompile: import once, then let agents investigate exact function addresses

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-23
Stage: Related project

At 16:05:06 Beijing time on November 23, 2026, Laurent Cheylus (@lcheylus) introduces the ghidra-decompile agent skill and 22 Ghidra scripts. Supplementary lookup found ioma8/ghidra-decompile-skill. It aims to avoid hours of full automatic analysis just to read one function: import with -noanalysis, keep the project, then decompile exact addresses. The skill also covers image-base alignment and output validation; scripts include cross-references, vtable/RTTI inspection and PACIASP entry scanning. The introducing poster is not established as the project author.

The README was read at commit 0a7ed092d2ce78d710d4f91a960c2d6a78ccf8d3, dated 2026-11-18T22:44:27Z, before the candidate window and used only as supplementary documentation. It reports 3.3 seconds for one targeted function after importing a 114 MB stripped AArch64 image. Hardware and full test logs are absent; this is not whole-image recovery or a general speedup ratio. Documentation claims verification on Ghidra 12.2 and warns that the GhidraMCP 7.0.0 release targets 12.1.4 and has compatibility problems with 12.2. The headless path needs no MCP. Only the introduction and README were read: no scripts were installed, images analyzed or measurements repeated. REA use is unconfirmed.

Sealed snapshot: 1 like, 38 views, 1 repost, 0 replies. The project's 3.3-second figure concerns a single function.

## Sources

- [Laurent Cheylus introduces the skill, November 23, 2026 at 16:05 Beijing time](https://x.com/i/status/2124776238636003682)
- [Supplementary README pinned to a 2026-11-18T22:44:27Z commit](https://github.com/ioma8/ghidra-decompile-skill/blob/0a7ed092d2ce78d710d4f91a960c2d6a78ccf8d3/README.md)

[中文](../ghidra-decompile-skill-targeted-function-analysis.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
