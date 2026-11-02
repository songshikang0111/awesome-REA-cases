# benilla: a Rust/Bevy WoW 1.12.1 client, with Claude attribution from a secondary report

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-02
Stage: In progress

At 20:32 Beijing time on November 2, 2026, grokked (@grokkedd) introduces benilla, crediting Claude, Rust and Bevy with rewriting the 2006 World of Warcraft 1.12.1 client. It uses owned data and a compatible server for quests, professions, raids, battlegrounds, social features, trade, mail and auctions. AI roles are attributed by the secondary report, not independently confirmed from developer records.

This review read samwhosung/benilla's README and deviations excerpts at 6a5f0f1064ef52788a92b8b81dffb39958ced71b, committed November 2 at 18:41:22 Beijing time. The project describes from-scratch formats, original protocol and a FrameXML/Lua engine, without original-client code, third-party WoW crates or game assets, while crediting early wowemulation-dev and warcraft-rs guidance. Full playability is a project claim. Settings and ESC menus intentionally follow Classic Era and other differences are itemized; this is not complete byte-for-byte equivalence.

The README requires legally obtained 1.12.1 build 5875 data. Development uses English clients and vmangos. Servers must not enforce Warden or require client changes beyond MPQ archives. Warden and other expansions are not planned. Addon compatibility, remaining options, performance and small differences are ongoing. No prebuilt downloads are offered; macOS, Linux and Windows builds are claimed. MIT/Apache-2.0 covers project code, not Blizzard content.

The benilla-re README was also read at fc85dad3cb85dec9330fb259a87f9d01eea5c68e, committed October 31 at 23:10:11 Beijing time, before the window. It records functions, structures and confidence by WoW.exe address and describes bitwise differential tests running original functions in an emulator against Rust. Generated tables and tests require the user's matching client. Other-build matches are leads, not semantic proofs. These are supplementary project methods, not new experiments in this window or tests rerun here. The candidate's 500 stars, 99 forks and 558 commits were not checked as current statistics. No assets were downloaded, build compiled or server connected.

Candidate snapshot: 19 likes, 376 views, 1 repost. Claude attribution is secondary; functionality and differential validation are project reports, not independently reproduced.
No game data is distributed. Warden is unsupported; official-service access or Blizzard endorsement is not established.

## Sources

- [Grokked's secondary benilla/Claude rewrite report, November 2, 2026](https://x.com/i/status/2117233457667403885)
- [Supplementary pinned benilla README: features and runtime limits, November 2, 2026](https://github.com/samwhosung/benilla/blob/6a5f0f1064ef52788a92b8b81dffb39958ced71b/README.md)
- [Supplementary pinned deviations excerpts, November 2, 2026](https://github.com/samwhosung/benilla/blob/6a5f0f1064ef52788a92b8b81dffb39958ced71b/docs/DEVIATIONS.md)
- [Supplementary pinned benilla-re README: addresses and differential methods, October 31, 2026, before the window](https://github.com/samwhosung/benilla-re/blob/fc85dad3cb85dec9330fb259a87f9d01eea5c68e/README.md)

[中文](../benilla-wow1121-claude-rust-bevy-client.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
