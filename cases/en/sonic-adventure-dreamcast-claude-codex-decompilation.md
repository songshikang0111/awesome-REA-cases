# Japanese Sonic Adventure: Claude/Codex-assisted Dreamcast matching decompilation and GCC port

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-01
Stage: Analysis test

At 03:49:53 Beijing time on November 1, 2026, Kyle Mayer (@kylemayer) reports four weeks of continuous Claude Code/Codex work on a byte-matching decompilation of the original Japanese Dreamcast Sonic Adventure, around one million lines of C and hundreds of hours of human polishing, followed by porting the SuperH C to modern GCC. He credits Falco Girgis's SH4ZAM hand-tuned SH-4 math library. The first-complete-Dreamcast claim, line count and labor are the author's statements, not measurements by this collection.

Supplementary public reshaped/sonic-adventure documentation is pinned to commit 25a3d3154dbe657325e97dbe8c5291086f6af5c0, dated October 31, 2026, 17:16:28 UTC, before the candidate. Its target is HDR-0001 version 1.007. The README reports 247 binaries and 5,820,458 code bytes, 97.7% C and 2.3% assembly; 14 C sources require shckit patches to compiler assembly. Matching builds use Hitachi SHC, disc data and address tables, comparing every rebuilt output with the original disc. Disc-free make check only checks recorded hashes for linkable sources and produces no complete binary. The GCC 16.2 path relinks the images and offers 16:9, 60 fps and a frame counter, all off by default; it is not evidence of a native Windows/Linux game port.

Byte matching does not establish recovery of the original source text or build settings. Users must supply a legally obtained Japanese disc. The README assigns MIT only to parts including build tools and tests; the rest of the repository has no license. Only the post and pinned documentation were read here: no disc download, toolchain installation, project execution or recomputation of matches.

Candidate snapshot: 0 likes, 32 views; no independent build.
247 binaries / 5,820,458 code bytes are project reports; matching and GCC builds are separate paths.

## Sources

- [Kyle Mayer's Claude/Codex decompilation report, November 1, 2026](https://x.com/i/status/2116618684773158965)
- [Supplementary first-party pre-candidate pinned README: matching scope, GCC path and licensing](https://github.com/reshaped/sonic-adventure/blob/25a3d3154dbe657325e97dbe8c5291086f6af5c0/README.md)

[中文](../sonic-adventure-dreamcast-claude-codex-decompilation.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
