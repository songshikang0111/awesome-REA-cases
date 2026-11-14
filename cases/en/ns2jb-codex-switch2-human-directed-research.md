# ns2jb: Codex-assisted Switch 2 research, with the author correcting the one-prompt autonomous-jailbreak story

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-11
Stage: In progress

Candidates posted between 16:10 and 19:38 Beijing time on October 22, 2026 describe pepsipu (Sammy Hajhamid), ns2jb, Codex-assisted Switch 2 firmware 23.0.1 research and a Mario Kart World mod. An earlier review traced them to the author's blog, jailbreaking the switch 2, dated October 18: supplementary first-party evidence, not research newly released on October 22. Its later Edit has no separate timestamp, so the correction is not dated October 18 here.

The goal is homebrew, game investigation and modification, save backups and progress toward custom firmware. The author built a Switch 1/2 interaction harness: JetKVMs provide USB controller input and HDMI video; a Bluetooth mechanical switch presses power after crashes. Codex contributed to SmileBASIC-interpreter and filesystem-service-object research and parallel exploration of several system services. The human selected attack surfaces, investigated privileges, improved unstable memory operations and chose directions. This records collaboration, not attack instructions.

The author explicitly corrects 'set a goal to jailbreak the switch 2. make no mistakes': it was a joke. The automated userland-code-execution goal failed, the jailbreak required substantial effort over roughly two weeks, and a footnote also marks WebKit exploration unsuccessful. The one-day, largely vibecoded activity was the Mario Kart World mod, not the jailbreak. The blog reports ordinary sysmodule privileges and native execution in built-in fs. It is tethered and must be rerun after reboot; modules beyond fs remain uncompromised and full custom firmware is a goal. Switch 1 was tested but not packaged, without all modchip capabilities. First known is the author's qualification, not this collection's exhaustive finding.

An October 24 candidate relays Mike Heskin's comments on FS contributions and privilege limits; Chen's October 30 report relays SmileBASIC 4 removal and claims no new firmware blocked it at that time. Their sources and historical limits remain in metadata. A new candidate at 04:04:35 Beijing time on November 11 reports firmware 23.5.0 patches the OS vulnerability used by ns2jb, attributing the blocked escape from vulnerable apps to OatmealDome. It says principal game-dumping and modding capabilities are blocked, with possible exceptions for some future cartridges. This is a later secondary limitations report, not a new author experiment. Nintendo's announcement, OatmealDome's original and device comparisons were not obtained. It guarantees neither failure of every older entry point nor valid cartridge exceptions, and the October 30 statement is not retained as current status.

This collection read blog text and posts only, downloading or executing no exploit, accessing no console or decrypted assets, and not independently watching verification videos. Project reports are not independent reproduction. REA is unmentioned. chasm's sealed October 22 snapshot of 1,858 likes, 123,985 views and 90 reposts is not technical validation.

Candidates originally posted 2026-10-22T16:30:18+08:00 and 17:06:02; blog originally dated 2026-10-18, with no separate Edit timestamp.
Sealed chasm candidate snapshot (2026-10-22): 1,858 likes, 123,985 views and 90 reposts; not independent verification.
A new candidate at 15:56:48 Beijing time on October 24, 2026 attributes comments to Mike Heskin (HexKyz); the candidate author is unavailable and Heskin's original was not obtained. It says the FS bug and object-exploitation concept were already known; the valuable new AI contribution was making heap grooming work, not discovering the entire chain. FS yields no key material and does not make kernel escalation easier. Other entry points and untethered operation remain theoretical possibilities. A predicted patch to the 23.0.1 chain is this comment's forecast, not testing of later firmware.
At 06:44:09 Beijing time on October 30, 2026, Chen (@chenYijl) relays that SmileBASIC 4 was removed from eShop and claims older firmware remained usable with no new firmware blocking it at that time. Store history and firmware announcements were not obtained; these changeable states are not established facts here. The post repeats two weeks of research, a one-day Mario Kart World mod and loss on reboot. Generalized claims that AI found the whole chain do not supersede the existing human contributions and recorded failures. Candidate snapshot: 1 like, 18 views, 0 reposts.
November 11, 2026 at 04:04:35 Beijing time: sealed candidate 0 likes, 140 views, 0 reposts. Firmware 23.5.0 and cartridge exceptions are secondary claims, not device-tested here.

## Sources

- [Candidate: chasm relays Codex and ns2jb](https://x.com/i/status/2113186167713640787)
- [Candidate: Chinese report naming Sammy, JetKVM and reboot limits](https://x.com/i/status/2113195160893116655)
- [Supplementary first-party blog and correction of the prompt/human-effort story](https://pepsipu.com/blog/2026-10-switch2-jailbreak-ns2jb)
- [New candidate: FS comments attributed to Mike Heskin, October 24, 2026, secondhand](https://x.com/i/status/2113902515779477645)
- [Chen relays SmileBASIC 4 removal and firmware limits at that time, October 30, 2026](https://x.com/i/status/2115937762637443462)
- [New secondary report: firmware 23.5.0 blocking escape, November 11, 2026](https://x.com/i/status/2120246261211451498)

[中文](../ns2jb-codex-switch2-human-directed-research.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
