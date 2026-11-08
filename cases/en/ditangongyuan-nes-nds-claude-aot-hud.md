# NES to NDS: ditangongyuan reports Claude-assisted 6502-to-C AOT conversion and a lower-screen HUD

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-08
Stage: In progress

At 23:58:34 Beijing time on November 8, 2026, ditangongyuan (@ditangongyuan) says Claude settled on rewriting disassembled 6502 logic in C while retaining the original memory layout, compiling a native program and implementing PPU graphics and APU audio in software. The author calls it an AOT emulator: CPU logic is converted ahead of time while related hardware behavior remains software-implemented. Claude also added a map and further status information to the lower-screen HUD.

The candidate literally writes DNS as the device name; that is not treated as a valid model identifier. A supplementary same-thread post dated November 8 at 18:53:58, before the window, explicitly names porting NES games to NDS: equal horizontal resolution, fewer vertical pixels, and the second screen available for status. It supplies platform identity and motivation, not a new-window candidate or a silent correction of the source token.

The author's done and correctness language is not backed by a game revision, complete source, build record, CPU/PPU/APU equivalence tests, frame rate or playthrough acceptance. Retaining memory layout does not establish full behavioral correctness. Later replies beyond the window, returned during retrieval, were not used as in-window results. No target was run, ROM downloaded or dual-screen handheld tested here. REA is unmentioned; retained as an in-progress porting self-report.

Candidate snapshot: 0 likes, 20 views, 0 reposts. Completion and correctness are the author's wording without whole-game or hardware acceptance.

## Sources

- [Candidate: ditangongyuan's Claude/6502-to-C and lower-screen HUD approach, November 8, 2026 at 23:58:34 Beijing time; original token DNS](https://x.com/i/status/2119459574440956403)
- [Supplementary pre-window thread post: NES-to-NDS goal and dual-screen motivation, November 8, 2026 at 18:53:58 Beijing time](https://x.com/i/status/2119382916904128863)

[中文](../ditangongyuan-nes-nds-claude-aot-hud.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
