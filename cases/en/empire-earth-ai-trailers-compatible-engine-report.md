# Empire Earth: The Art of Conquest: Claude-credited reconstruction, mixed multiplayer and testing limits

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-12
Stage: In progress

At 16:30:18 Beijing time on November 12, 2026, yibie (@yibie) introduces Protryon/empire_earth, describing mixed original/rebuilt hosts and clients and AI evidence in commit trailers rather than README. Supplementary reading uses README at 073017a6b1809735d2d586f633ce7b8ddc2b4584, committed November 8 at 15:31:23 Beijing time before the candidate. The actual target is Stainless Steel Studios/Sierra's 2002 Empire Earth: The Art of Conquest, reconstructing C++ with the original VC6 toolchain across the game and first-party DLLs.

Pinned docs report a November 7 measurement at source revision 698ba84314bf: 15,420/16,884 game-code functions (91.3%) and 1,820,263/2,736,250 code bytes (66.5%) matched, with separate WON-library, engine, network and renderer figures. Unmatched reconstructed functions still link, so whole images are not identical. The DCL compression library is explicitly a format-compatible reimplementation rather than original-library machine code. Linking every image from source does not mean every function matches.

Project-reported tests include short games, long Deathmatches, a scripted human player, save/load in every direction and tick-by-tick simulation/AI/render-state comparisons. Mixed original/rebuilt TCP hosts and clients reportedly finish without desynchronization. Separate lobby/Direct Connect startup checks do not show in-game peer sync and must not be confused with the stronger automated multiplayer test. WON online servers no longer exist and were not tested; audio output and physical input remain uncovered. Main deliberately preserves original bugs for compatibility. fixes-all changes simulation/AI and should play only with the same branch, so interoperability cannot be generalized to every branch.

The GitHub history query reachable from the pinned revision returned 22 commits, all with Claude Opus 5.5 co-author trailers. This differs from the candidate's count of twenty; both scopes are retained. Twenty-two is neither AI-contributed functions nor a complete development audit. Only commit messages and README were read, not AI sessions, all test logs or implementation. Publicly readable is not a general open-source grant: README says No license is granted, and users need legal game data. This collection built nothing, played no network game and executed no code. Work remains in progress.

Sealed whole post: 3 likes, 275 views, 0 reposts, 1 reply. The candidate says twenty trailers; the pinned history query returned 22 commits. Neither count measures functional correctness.

## Sources

- [yibie on Empire Earth mixed multiplayer and AI commit credits, November 12, 2026 at 16:30:18 Beijing time](https://x.com/i/status/2120796315898777815)
- [Supplementary pinned Empire Earth README committed November 8, 2026 at 15:31:23 Beijing time, containing a November 7 measurement](https://github.com/Protryon/empire_earth/blob/073017a6b1809735d2d586f633ce7b8ddc2b4584/README.md)
- [Supplementary pinned history entry: Claude Opus 5.5 credits in reachable commits, not runtime verification](https://github.com/Protryon/empire_earth/commits/073017a6b1809735d2d586f633ce7b8ddc2b4584)

[中文](../empire-earth-ai-trailers-compatible-engine-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
