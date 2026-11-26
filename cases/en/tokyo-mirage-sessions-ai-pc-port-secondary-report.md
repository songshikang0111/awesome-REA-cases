# Tokyo Mirage Sessions/TMSRecomp: Claude-credited static recompilation, tested through chapter two

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-26
Stage: In progress

At 06:18:32 Beijing time on October 28, 2026, playswave (@playswave_com) reports a fan PC decompilation port of Tokyo Mirage Sessions at 60–120 FPS in an AI-coding narrative. The older account names no project, developer, repository, OS, version, measurement or AI work records. Its linked article was not obtained, and under one million sales is only background it supplies. The historical source is retained without identifying the later named project as the same implementation.

At 14:50:23 on November 26, Furkan YILDIRIM (@furkandev) introduces TMSRecomp, a static Windows recompilation of the Switch game Tokyo Mirage Sessions #FE Encore. Quoting its README, the post credits Claude through Claude Code for all code, tools and reversing, with a human directing, testing and reviewing. It describes ARM-to-C-to-Windows-x64 translation and claims up to 4K/240 FPS and five betas in three days since November 23. The latter are a relayed timeline and advertised ceiling, not measured labor or benchmarks run here. This evidence is appended to the existing ID for the same game target without erasing uncertainty about the earlier report's identity.

Supplementary reading pins godofknife/TMSRecomp's README to 5807e38667c8a5c4d96c4f69c1d81b063fce7179, committed at 04:09:54 Beijing time on November 26, before this window. It confirms v0.1.4 beta and the AI/human attribution, 32-bit ARM statically translated to C, required NVN graphics implemented on Vulkan and no JIT. It describes runtime memory, Horizon services, audio and input, and Ryujinx's translator turning Maxwell shaders into SPIR-V. The document mentions test_a32.py comparisons against Unicorn, but test implementation/results were not read; comprehensive translation validation is not established.

On Windows, the project reports only NVIDIA RTX testing through the chapter two Idolasphere with saving/loading. Later chapters, AMD/Intel and weaker PCs are unknown. Users need their own base Switch version 1.0.0 without updates, title ID 0100A9400C9C2000; fixed-address hooks do not support 1.0.1+ or DLC. 4K and 30–240 or uncapped frame rates are options, not measured performance in every scene. Docs say 60 FPS is most tested, while NPC turns still step at 30 Hz at high frame rates. Experimental Linux work separately reports Ubuntu 26.04/GTX 1650/driver 620 running scenes, saving/loading and other functions at 60 FPS. Battles, AMD/Intel and Steam Deck are untested and FSR3/DLSS is not wired up. This is neither RTX-only testing on every platform nor a fully verified Linux playthrough. Emulator saves and saves from updated game versions are also untested.

Docs state that no game is included and a locally generated game.dll contains game material and must not be shared. This is a distribution statement, not an audit of the entire release package. No game, keys, firmware, release package or dependencies were obtained; no build, execution, implementation review or graphics/frame-rate reproduction was performed. Only public documents and attribution were checked. Results remain project reports, status in-progress, and REA unmentioned.

Older candidate snapshot: 0 likes, 31 views, 0 reposts. Its 60–120 FPS and AI attribution are secondhand and are not retroactively verified by the new project's docs.
November 26 sealed candidate: 2 likes, 246 views, 0 reposts, 1 reply. Five betas in three days is relayed, not checked against release history. README is project-reported evidence only.

## Sources

- [playswave's Tokyo Mirage Sessions port report, October 28, 2026; identity with TMSRecomp unestablished](https://x.com/i/status/2115206541045551503)
- [Furkan YILDIRIM on TMSRecomp and chapter-two testing limits, November 26, 2026 at 14:50:23 Beijing time](https://x.com/i/status/2125844598161346932)
- [Supplementary pinned TMSRecomp README, committed November 26, 2026 at 04:09:54 Beijing time; pre-window documentation](https://github.com/godofknife/TMSRecomp/blob/5807e38667c8a5c4d96c4f69c1d81b063fce7179/README.md)

[中文](../tokyo-mirage-sessions-ai-pc-port-secondary-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
