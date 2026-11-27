# VIctory compatibility research: AvatarManz's fork, Claude attribution, single-machine performance and graphics defects

Category: Games and preservation · Other AI-assisted work
Record date: 2026-11-27
Stage: Needs verification

At 20:19:02 Beijing time on November 26, 2026, Tiancai (@BitTheOnly) describes Victory's Xbox-to-PC compatibility work, relaying AI-assisted API/graphics research, visible opening cinematics and prologue characters, vehicles and buildings, but serious shader/texture problems, plus a participant's forecast of minimal playability in 48 hours. Earlier retrieval confirmed attribution, wording and a video attachment, not viewing or execution. Forty-eight hours is a forecast, not verified playability or total labor. The post's claim that Leonida stopped does not settle conflicting evidence about that project.

At 07:17:00 Beijing time on November 27, Ai Neural Ape (@Shenjingape) says Claude and Gemini helped an experimental Xbox emulator rise from 3–5 to 25–30 FPS in a day, with Claude credited on 171 of AvatarManz's 176 commits, one build running 41 minutes without crashing, and Take-Two issuing DMCA notices against related repositories. No counting query, precise revision, hardware, run log or notice is attached. These figures, legal status and official-PC-release rumors are not established facts here.

Supplementary reading identifies the public avatarmanz/VIctory-7900XTX repository, pinned to 014d52dedf837d1ac660a0bd256c4704be9eeb40, committed at 06:33:21 Beijing time on November 27, as supporting material rather than another candidate. Its README, dated November 26, describes a Marvisak/VIctory compatibility-layer fork starting from fxceless's fork and credits DexNom, Belobug and others. It explicitly credits Claude Code for this fork's changes; the latest commit message co-credits Claude Opus 5.5. This confirms public attribution, not the 171/176 statistic, Gemini's use in this fork or wholly autonomous model work. The existing Victory ID is retained rather than adding the named fork as another target. Documented contributions from Belobug do not identify every earlier demo and author as one revision.

The project aims first for correct Series X visuals on RX 7900 XTX, then 30+ FPS with ray tracing, then smaller memory requirements. It calls the approach porting rather than emulating: patching renderer behavior and translating shaders ahead of time to reduce copying shared memory. On one Windows 11/i9-12900K/64 GB RAM/RX 7900 XTX machine, reported 270-second city standing/walking runs give roughly 10/9 FPS at 4K output rendered at 1440p with ray tracing and 45 GB RAM; the same output without ray tracing gives about 20/16 FPS. At 1080p output without ray tracing it reports about 25/23 FPS and 42 GB RAM; Series S without ray tracing gives about 23/16 FPS and 37 GB RAM. This is not 25–30 FPS for all settings or achievement of the 30 FPS goal. An older table lists 57–75 ms in the same scene before patches, roughly 22 FPS without ray tracing and 25,790/25,985 translated shaders, with the remainder described as unused geometry shaders. All are project reports, not proof of whole-game correctness.

The docs report fixes for briefly disappearing trees and some indoor lighting, but retain distant flicker, slow texture/model detail streaming, corrupt ray-traced structures for moving objects (about 450 stray pointers per frame), pipeline stutter on new builds, and frame recording triggering the game's watchdog. The latest commit reports latency changes in other scenes, not a single combined performance result. Only the pinned README and commit message were read, not full patches, logs or reruns; the earlier missing-repository limitation is lifted only to this extent. The repository says it contains no game files and requires the user's own copy. Asset policy, lawful provenance and game/key acquisition were not verified; no target was executed. REA is unmentioned and status remains unverified.

Old sealed candidate: 6 likes, 1,711 views, 0 reposts, 0 replies. The 48-hour forecast and boot visuals lack independent verification.
New sealed candidate: 1 like, 257 views, 0 reposts, 0 replies. 171/176, 41 minutes, 25–30 FPS and DMCA are unverified secondhand claims.
Pinned README reports only one RX 7900 XTX machine. Settings, scenes and dates must not be mixed; public credits are not an independent audit of all code or tests.

## Sources

- [Tiancai relays Victory's AI compatibility work, prologue visuals and defects, November 26, 2026 at 20:19:02 Beijing time](https://x.com/i/status/2125927306569130432)
- [Ai Neural Ape relays AvatarManz, frame rates and Claude credits, November 27, 2026 at 07:17:00 Beijing time](https://x.com/i/status/2126092889000132767)
- [Supplementary pinned VIctory-7900XTX README: November 26 docs, single-machine data and Claude Code credit; revision committed November 27 at 06:33:21 Beijing time](https://github.com/avatarmanz/VIctory-7900XTX/blob/014d52dedf837d1ac660a0bd256c4704be9eeb40/README.md)
- [Same pinned commit message: scene latencies and Claude Opus 5.5 co-credit; full patch not examined](https://github.com/avatarmanz/VIctory-7900XTX/commit/014d52dedf837d1ac660a0bd256c4704be9eeb40)

[中文](../victory-gta6-ai-pc-compatibility-secondary-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
