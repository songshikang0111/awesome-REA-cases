# Darmoshark TOP75 on Mac: AI-assisted Windows-utility research, then IOKit Bluetooth checks

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-18
Stage: Needs verification

At 01:24:07 Beijing time on November 18, 2026, Bedirhan Skywalker (@bedirhansamsa) explains the source of the Darmoshark TOP75 keyboard's Bluetooth protocol: he reverse-engineered its Windows utility with AI help and tested commands on the paired keyboard through IOKit. He says Bluetooth reuses the 64-byte USB command with a 06 55 prefix. His supplementary main post at 00:10:33 describes a macOS 14-or-later app for RGB, key remapping, macros and scheduled lights-off. Although also inside the window, that main post is supplementary evidence, not another candidate. The model and REA use are unspecified.

Supplementary reading covers kreativecenter/top75-macos documentation pinned at 93650a4, committed November 17, 2026 at 18:42:08 UTC, or November 18 at 02:42:08 Beijing time. This is a post-candidate documentation snapshot, not proof that every feature existed at 01:24. The README credits Bedirhan Samsa and links the same X account, identifying an MIT-licensed community project. protocol.md records static inspection of the Windows installer and identification of yc500_top75_soc, ID 957, cross-checked against existing sharkfin protocol documentation. This does not establish independent AI discovery of every field. Bluetooth documentation describes a 66-byte output report carrying the prefix and 64-byte command, accepting responses and confirming device identity.

The project reports readback and rollback of lighting, profiles, short macros and selective restore on firmware 274, with Bluetooth schedules restoring prior settings. It also records a five-page macro write causing USB re-enumeration, followed by a populated-page writer and size limits. Short per-key color intervals dropped writes, so additional waiting was introduced. Display artwork uses USB; transport acknowledgement is not image readback. The device owner confirmed still-image display, but on-device GIF playback remains unvalidated. Apple Silicon hardware was tested; a universal Intel build is not proof of Intel hardware testing. Results on one firmware are not generalized across the family.

Only the author thread, pinned README and protocol/verification notes were read here. Full source and tests were not reviewed or executed, no Mac app was installed and no keyboard connected. Documented tests remain project reports, not independent reproduction. Status stays unverified.

November 18, 2026 sealed candidate: 0 likes, 11 views, 0 reposts, 1 reply. Low engagement does not invalidate concrete engineering evidence. Tests are project reports, not tests run here.

## Sources

- [Bedirhan on AI-assisted Windows-utility research and IOKit testing, November 18, 2026 at 01:24:07 Beijing time](https://x.com/i/status/2122742591888175234)
- [Supplementary in-window main post: TOP75 Mac app uses, November 18 at 00:10:33 Beijing time](https://x.com/i/status/2122724078431748229)
- [Post-candidate pinned README: attribution, features and compatibility limits, commit November 17, 2026 at 18:42:08 UTC](https://github.com/kreativecenter/top75-macos/blob/93650a4f3e094cc5472a7eff18c1311dbbf5501c/README.md)
- [Protocol and project hardware-verification notes at the same pinned commit](https://github.com/kreativecenter/top75-macos/blob/93650a4f3e094cc5472a7eff18c1311dbbf5501c/docs/protocol.md)

[中文](../darmoshark-top75-macos-ai-protocol-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
