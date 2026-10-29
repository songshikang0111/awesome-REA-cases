# Moon-Buggy: Florian BURNEL uses REA and Claude to read a binary and rebuild a browser game

Category: Games and preservation · REA
Record date: 2026-10-30
Stage: Analysis test

Two candidates at 01:01:38 and 01:30:29 Beijing time on October 30, 2026 share Florian BURNEL's IT-Connect article. The full article is dated October 29, 2026, so it is earlier supplementary evidence, not an in-window original publication. He selects Moon-Buggy, Jochen Voss's 1998 GPL ASCII game, and uses the stripped x86-64 ELF installed through APT in a Linux Mint VM, saying he analyzes it without consulting source. This is a teaching test with public source available for later comparison, not cracking a closed-source game.

He asks Claude Code with Opus 5.5 to use REA to recover scrolling, jumping, obstacle, scoring and collision rules, provide addresses, instructions or constants and unresolved items, and then generate a standalone index.html. He reports 97 unnamed functions. The agent follows references from strings including score_crater and level_start, invokes Ghidra, and identifies structures including 13 buggy sprites and an eight-level table. Analysis through browser implementation reportedly takes 12 minutes 29 seconds. Listed rules include scrolling one column per 0.08 seconds; a five-state jump lasting 1.08 seconds, with 0.88 seconds airborne and a maximum height of two lines; craters one to six columns wide; obstacles requiring three laser hits; and +20 for passing an obstacle, +13 for destroying it and -1 per shot.

BURNEL says his checks found these rules correct, except that objects the model calls rocks are meteorites in source. The browser game is keyboard-playable, and a separate ANALYSE.md is said to retain address-level evidence. This collection read the article and its displayed process, but did not obtain the full analysis report, run the HTML, independently time the work, verify every address or recompute the rules. The article says similar work is possible without REA but supplies no controlled timing comparison, so no speedup is calculated. DX-Ball, ReaCut and VSL-DSP are background examples of existing projects, not parts of BURNEL's Moon-Buggy experiment.

The two candidate snapshots are respectively 0 likes/11 views/0 reposts and 5 likes/460 views/0 reposts.
12m29s and rule correctness are author reports. No independent rerun or full ANALYSE.md was obtained here.

## Sources

- [Candidate shares the IT-Connect test article, October 30, 2026](https://x.com/i/status/2115851565202382949)
- [Same-window share explicitly naming Florian BURNEL, October 30, 2026](https://x.com/i/status/2115858824032596199)
- [Supplementary: Florian BURNEL's full Moon-Buggy tutorial test, article dated October 29, 2026](https://www.it-connect.fr/rea-retro-ingenierie-ia-ghidra/)

[中文](../it-connect-moon-buggy-rea-claude-web-rebuild.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
