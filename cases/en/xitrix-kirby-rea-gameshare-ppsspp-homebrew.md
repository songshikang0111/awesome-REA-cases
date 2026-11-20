# Kirby to PPSSPP: XITRIX uses REA to investigate GameShare startup calls

Category: Games and preservation · REA
Record date: 2026-11-20
Stage: Needs verification

At 05:03:05 Beijing time on November 20, 2026, XITRIX (@X1TRIX) explains how GameShare was added to their PPSSPP port for Switch 2. PPSSPP is a PSP emulator. The author says they used REA to investigate how a Kirby game starts the feature through the system SDK, then called the same APIs from homebrew. The goal is reuse of system sharing capabilities, not recovery of Kirby's entire source. The specific Kirby title is unnamed.

The same thread's introduction at 03:21:50 on November 20 says the port uses kaiHEN and GameShare creates a second PPSSPP instance controlled by a client Switch, allowing a friend to play PSP games from the same collection or join local multiplayer. This introduction predates the current 04:00 window and is supplementary context for purpose and reported results, not a candidate. Another participant says libounce already offers a GameShare API; XITRIX then says they also wrote an SDK. These statements do not independently validate either implementation.

Attribution and conversation context were checked, but API code, SDK and the complete REA session were not read, the demonstration was not watched and no console was tested. Compatible models, network limits and per-game multiplayer behavior remain unconfirmed. The older ongoing Kirby record belongs to another author and does not identify its title. Without evidence of a shared project, its progress and account concerns are not merged here. This remains a specific interoperability result reported by its author, not independently verified.

Sealed candidate: 1 like, 163 views, 0 reposts, 1 reply; not total project engagement.

## Sources

- [XITRIX explains REA investigation of Kirby's GameShare SDK calls, November 20, 2026 at 05:03:05 Beijing time](https://x.com/i/status/2123522473777885254)
- [Supplementary context: PPSSPP Switch 2 port and GameShare dual instances, November 20, 2026 at 03:21:50 Beijing time, before the current window](https://x.com/i/status/2123496993884660100)
- [Supplement: XITRIX says they also made an SDK, November 20, 2026 at 05:35:14 Beijing time](https://x.com/i/status/2123530566104703355)

[中文](../xitrix-kirby-rea-gameshare-ppsspp-homebrew.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
