# xmen2-pc: Claude Code-assisted X-Men 2 reconstruction adds four-player rollback multiplayer

Category: Games and preservation · Other AI-assisted work
Record date: 2026-10-31
Stage: In progress

At 02:36:57 Beijing time on October 31, 2026, The Gaming Emporium (@McGroin83) presents crabsmack's xmen2-pc, a native Windows/Linux port of the 1995 Sega Mega Drive/Genesis game X-Men 2: Clone Wars, adding four-player local/online co-op, rollback networking, widescreen and high refresh rates. The post explicitly discloses that the developer credits Claude Code agents with almost the entire project. The README was read at commit 06783ee115f1e374d35bf088ce432cfa962d5739, dated 2026-10-28T01:40:12Z. This earlier project evidence is supplementary, not another window candidate.

The README separates byte-matching disassembly, static recompilation using segagenesisrecomp, identification of the original Apple MPW C 3.3 compiler, readable C reconstruction, a native port without 68000 emulation, and subsequent enhancements/netplay. It says that of 3,164 functions, the 3,047 originally written in C compile to the cartridge's exact machine code with the original compiler. The remaining 117 were originally assembly and cannot byte-match through a C compiler; their C is compared instruction by instruction against recompiled cartridge code, reporting no differences. With options off, test runs reportedly match state and pictures each frame, except deliberately not reproducing cartridge slowdown. These are project reports, not a match rate recomputed here or proof of equivalence over all inputs.

The project credits Claude Code with almost all work in nine days under measurable completion criteria; REA is unspecified. The 16:9 view is separate from widescreen_gameplay, which changes enemy activation. high_fps interpolates between game frames for 61–1000Hz rather than accelerating logic. full_rate_2p restores two-player logic from the original's halved rate to 60 frames. New three/four-player modes explicitly have less playtesting. Online players need their own ROM and the same release; v1.1.0 rejects v1.0.x. Network performance was not tested here.

Only the compatible USA/Europe ROM is accepted, with assets read from the user's file at startup and no cartridge content distributed. Original work is MIT, but segagenesisrecomp uses PolyForm Noncommercial and the README forbids commercial use of port builds; the entire artifact is not simply commercially usable MIT. This collection downloaded no ROM, executed no target, installed no dependencies and reran neither compilation nor differential tests. Included for its public implementation and explicit self-test limits.

Candidate snapshot: 1 like, 194 views, 0 reposts. Nine days, 3,047/3,164 and the 117-function zero-difference result are project reports.
Pinned commit predates the window. Four-player additions are less tested; neither gameplay nor matching was independently checked.

## Sources

- [The Gaming Emporium presents xmen2-pc; full original includes Claude Code disclosure, October 31, 2026 at 02:36:57](https://x.com/i/status/2116237941227843747)
- [Supplementary: October 28 pinned README, byte matching, networking and license limits](https://github.com/crabsmack/xmen2-pc/blob/06783ee115f1e374d35bf088ce432cfa962d5739/README.md)
- [Supplementary: October 28 documentation commit with Claude Opus co-author credit](https://github.com/crabsmack/xmen2-pc/commit/06783ee115f1e374d35bf088ce432cfa962d5739)

[中文](../xmen2-pc-claude-genesis-native-port.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
