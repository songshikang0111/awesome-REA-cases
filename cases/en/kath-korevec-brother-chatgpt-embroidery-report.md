# ZigZag and Brother Skitch: public implementation supplements the ChatGPT account, with protocol reuse from Respira

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-13
Stage: Needs verification

Earlier sources are Hanqing's (@hanqing1120) $12 hardware-subscription reply at 20:36:06 Beijing time on October 26, 2026, and Valar's (@ValarMind) parent at 18:26:52. The latter says Kath Korevec bought an approximately $300 Brother embroidery machine, used ChatGPT for direct-control software and made generated-art patches. The $12/month, sellout and employment claims belong to that retelling, not independent verification. The old record called her an OpenAI product lead; supplementary public GitHub profile retrieval now shows simpsoka self-identifying as Kathy Korevec, Product @google. This corrects an overconfident secondary job attribution without inferring historical employment from a current profile.

At 09:15:25 Beijing time on November 13, Andrew111 (@AndrewSignalZ) explicitly names open-source Zigzag and simpsoka/zigzag as a subscription-software alternative for a $300 embroidery machine. It relays 314 Show HN points, 130 comments and roughly $100 secondhand machines. These remain the post's claims; the HN thread and prices were not checked. They do not establish reproduction here or recovery of every machine function. Shared author clues and the Brother direct-control target support supplementing the existing ID rather than creating a duplicate. Earlier material is not re-reviewed as a new current-window candidate.

Supplementary README and NOTICE were read at commit 7fdb49f34517f569128bf02f215b45fa280c818c, dated November 13 at 08:50:47 Beijing time: project evidence, not a second candidate. README identifies the Brother Skitch PP1. The Rust editor converts SVG to stitches, exports PES/DST/EXP/JEF/VP3 or uploads over Bluetooth. MCP allows Claude Code, Codex and others to operate on the visible design, send designs and query machine status. Mac/Windows release paths are documented, but packages and implementation were not downloaded or audited. Pausing still requires the machine's physical button, not Bluetooth. Settings writes await a known layout and unchanged-value write/readback agreement; complete device control is not established.

Important attribution correction: NOTICE explicitly credits ports from Jan-Henrik Bruhn's Respira (Apache-2.0) for the PP1 Bluetooth protocol, sewing flow, errors, rollback and PEN encoding. PES/PEC/DST layouts come from pyembroidery; Image Trace and other components come from VectorCraft. The entire protocol discovery cannot be credited to ChatGPT or independent ZigZag research. MCP support establishes an AI-facing design workflow, not how ChatGPT contributed to the earlier protocol work; original AI work logs are still missing.

README reports 136 library tests, 153 editor/MCP tests and 222 tests in the used Image Trace component, stitch-position round trips through pyembroidery, and testing on a real Skitch PP1. These are project statements; itemized logs, demonstrations and reruns were not reviewed or performed. Simulated-machine tests do not validate every real device. Status remains unverified. No code or device was run, and subscription terms or technical-protection bypasses were not established. REA is unmentioned. This is not merged with the Brother scan-button/NAS project.

Earlier candidate: 1 like, 16 views, 0 reposts. The $300, $12/month and sellout claims are secondary.
November 13 current snapshot: 1 like, 118 views, 0 reposts, 2 replies. HN 314 points/130 comments and about $100 are relayed, without checking the thread or prices.
136/153/222 are test-group counts reported in the pinned README, not execution results here. Protocol/PEN ports and upstream attribution are in NOTICE.

## Sources

- [Earlier source: Hanqing's $12-subscription reply, October 26, 2026](https://x.com/i/status/2114697580362055944)
- [Earlier parent: Valar's Kath Korevec/Brother/ChatGPT account, October 26, 2026](https://x.com/i/status/2114665054780133816)
- [Current Andrew111 account explicitly naming Zigzag's repository, November 13, 2026 at 09:15:25 Beijing time](https://x.com/i/status/2121049262045937692)
- [Supplementary pinned README: Skitch PP1, MCP and project tests, November 13, 2026 at 08:50:47 commit](https://github.com/simpsoka/zigzag/blob/7fdb49f34517f569128bf02f215b45fa280c818c/README.md)
- [NOTICE at the same commit: Respira protocol ports and other upstream credits](https://github.com/simpsoka/zigzag/blob/7fdb49f34517f569128bf02f215b45fa280c818c/NOTICE)
- [Supplementary public GitHub profile: Kathy Korevec's self-description, not historical employment evidence](https://github.com/simpsoka)

[中文](../kath-korevec-brother-chatgpt-embroidery-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
