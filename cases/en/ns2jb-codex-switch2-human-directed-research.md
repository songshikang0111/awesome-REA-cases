# ns2jb: Codex-assisted Switch 2 research, with the author correcting the one-prompt autonomous-jailbreak story

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-10-30
Stage: In progress

Candidates posted between 16:10 and 19:38 Beijing time on October 22, 2026 describe pepsipu (Sammy Hajhamid), ns2jb, Codex-assisted Switch 2 firmware 23.0.1 research and a Mario Kart World mod. This review traced them to the author's public blog, jailbreaking the switch 2, dated October 18: supplementary first-party evidence from before this window, not research newly released on October 22. Its later Edit has no separate timestamp, so the correction itself is not dated October 18 here.

The goal is homebrew, game investigation and modification, save backups and progress toward custom firmware. The author built an interaction harness around Switch 1 and 2: JetKVMs provide USB controller input and HDMI video, and a Bluetooth mechanical switch presses power after crashes. Codex contributed to investigation of the SmileBASIC interpreter, filesystem-service objects and parallel exploration of several system services. The human also selected attack surfaces, investigated privileges, improved unstable memory operations and chose subsequent directions. This records collaborative research, not instructions for reproducing the attack.

The author explicitly corrects the viral caption, set a goal to jailbreak the switch 2. make no mistakes: it was a joke. His automated userland-code-execution goal failed, and the jailbreak required substantial effort over roughly two weeks. A footnote also marks the WebKit attempt unsuccessful. The one-day, largely vibecoded activity was the Mario Kart World mod for fun, not the entire jailbreak. Neither one day nor one prompt is its reported development effort.

The blog reports software-only native execution with ordinary sysmodule privileges and in the built-in fs module, supporting homebrew, game research, mods and save backups. It is tethered and must be rerun after reboot; built-in modules other than fs remain outside its demonstrated compromise, and full custom firmware is a future goal. The author reports Switch 1 testing without packaging and says it does not provide all modchip capabilities. First known is the author's qualification, not an independently exhaustive finding by this collection.

This review read the blog and candidates only. It downloaded or executed no exploit, accessed no console or decrypted assets, and did not independently watch and verify the videos. Project-reported operation is not independent reproduction. REA is not mentioned. The sealed October 22 snapshot of chasm's candidate has 1,858 likes, 123,985 views and 90 reposts; engagement does not validate the technology.

Candidates originally posted 2026-10-22T16:30:18+08:00 and 17:06:02; blog originally dated 2026-10-18, with no separate Edit timestamp.
Sealed chasm candidate snapshot (2026-10-22): 1,858 likes, 123,985 views and 90 reposts; not independent verification.
A new candidate at 15:56:48 Beijing time on October 24, 2026 attributes comments to Mike Heskin (HexKyz); the candidate author is unavailable and Heskin's original was not obtained. It says the FS bug and object-exploitation concept were already known; the valuable new AI contribution was making heap grooming work, not discovering the entire chain. FS yields no key material and does not make kernel escalation easier. Other entry points and untethered operation remain theoretical possibilities. A predicted patch to the 23.0.1 chain is this comment's forecast, not testing of later firmware.
At 06:44:09 Beijing time on October 30, 2026, Chen (@chenYijl) relays that SmileBASIC 4 was removed from eShop and claims older firmware remained usable with no new firmware blocking it at that time. Store history and firmware announcements were not obtained; these changeable states are not established facts here. The post repeats two weeks of research, a one-day Mario Kart World mod and loss on reboot. Generalized claims that AI found the whole chain do not supersede the existing human contributions and recorded failures. Candidate snapshot: 1 like, 18 views, 0 reposts.

## Sources

- [Candidate: chasm relays Codex and ns2jb](https://x.com/i/status/2113186167713640787)
- [Candidate: Chinese report naming Sammy, JetKVM and reboot limits](https://x.com/i/status/2113195160893116655)
- [Supplementary first-party blog and correction of the prompt/human-effort story](https://pepsipu.com/blog/2026-10-switch2-jailbreak-ns2jb)
- [New candidate: FS comments attributed to Mike Heskin, October 24, 2026, secondhand](https://x.com/i/status/2113902515779477645)
- [Current candidate: Chen relays SmileBASIC 4 removal and firmware limits, October 30, 2026](https://x.com/i/status/2115937762637443462)

[中文](../ns2jb-codex-switch2-human-directed-research.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
