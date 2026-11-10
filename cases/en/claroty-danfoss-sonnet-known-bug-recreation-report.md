# Danfoss refrigeration controllers: Sonnet bug recreation, a Sekoia firmware investigation and a repair idea

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-10
Stage: Needs verification

At 05:30 Beijing time on November 3, 2026, Hacked (@hackedpodcast) relays Claroty CTO and Team82's Amir Preminger: Sonnet recreated a known Danfoss refrigeration-controller bug from research for about $6. This evaluates cheaper reproduction from prior research, not first discovery. Discussion of cheaper models bypassing safeguards and European refrigeration attacks establishes no AI involvement in real attacks. At 07:11, ChrisR (@le_kryzz) asks about reversing repairs for unsupported devices and suggests AI rewriting. A November 3, 03:06 parent identifies Danfoss before that round's 04:00 window, as background only. Support status, affected stores and scale are unchecked; the suggestion is not an implemented repair.

At 04:14:04 and 04:14:50 on November 7, Frelzu (@Frelzu) relays Claroty's use of public firmware, known bugs and researcher supervision: Sonnet 4.6 reportedly reaches lab-device root in 28 minutes for about $6. Authentication bypass initially failed and needed researcher redirection. A reply says firmware fixes exist without a checked advisory or version, and says the French attack path and AI involvement were unconfirmed, while the Pentagon had not confirmed freezer failures as an attack. These remain the sources' statements at the time, not a causal link between lab runs and incidents.

At 02:22:49 on November 10, Sekoia (@sekoia_io) reports its own investigation: an unnamed LLM given a captured request and public Danfoss firmware confirmed within minutes that an admin account could be renamed without authentication, the first step in a password reset. Supplementary thread retrieval confirms a claim that honeypots caught attempted exploitation of a non-public bug on November 1, and that French authorities attributed attacks to IRGC's Shahid Kaveh/CyberAv3ngers. Roughly 2,700 exposed controllers on October 11, about 1,700 in France, is also Sekoia's historical observation. The original article and French advisory were not checked; the newer attribution is not independently confirmed, nor does it show attackers used AI. This request-driven LLM analysis is attributed separately from Claroty's known-bug experiment. One rename step is not a complete password reset, root access or proof of the same CVE.

Those earlier materials do not establish a controller model, CVE, raw inputs/outputs, billing or reproduction/repair logs; the full podcast was not watched. The newer secondary account's model/CVE distinctions follow below. Sonnet 4.6, 28 minutes, root, minutes and fix availability are respective source claims, not autonomous discovery, universal costs or reliable exploitation of arbitrary devices. No code, device or patch was exercised here. REA is unspecified.

A new long-form candidate at 08:02:24 Beijing time on November 10, 2026 further relays Sekoia using GLM 5.3 and public Danfoss firmware to interpret the captured rename request within minutes. It names four 800A web-interface honeypots and distinguishes CVE-2025-41450's date-code issue from the nonpublic rename issue observed on November 1. The model number describes the honeypot interface, not established hardware for Claroty's earlier experiment. GLM 5.3 is attributed by the new secondary account, not substituted into Sekoia's originally unnamed wording or evidence both teams used it. The full Sekoia report, vendor advisory, HAR and model output were not read. Attack scale and an LLM demonstration are not combined into proof AI executed the real attacks; the older experiment and new investigation remain distinct.

Older candidates: podcast 1 like/73 views; repair idea 0 likes/33 views; both 0 reposts. About $6 is relayed.
November 7 posts: 11 likes/129 views/0 reposts and 0 likes/20 views/0 reposts; not independently reproduced.
November 10 sealed candidate: 1 like, 45 views, 0 reposts. Minutes is Sekoia's report, without billing or model name.
New 08:02:24 candidate: 0 likes, 182 views, 0 reposts. GLM 5.3 is named by this secondary account, not checked against the original report.

## Sources

- [Hacked relays Amir Preminger's Sonnet experiment, November 3, 2026](https://x.com/i/status/2117368895518507120)
- [ChrisR proposes AI repair of unsupported hardware, November 3, 2026](https://x.com/i/status/2117394194646081838)
- [Supplementary parent: Danfoss context, November 3 at 03:06, before that round's window](https://x.com/i/status/2117332531959754878)
- [Frelzu adds lab conditions, $6 and 28 minutes, November 7 at 04:14:04 Beijing time](https://x.com/i/status/2118799095670403137)
- [Same thread: Sonnet 4.6, human correction, firmware fix and attribution limits, 04:14:50](https://x.com/i/status/2118799287606030680)
- [Sekoia reports LLM analysis of a request and public firmware, November 10, 2026](https://x.com/i/status/2119858264485642574)
- [Supplementary thread: Sekoia's attack-attribution account, not evidence of AI involvement](https://x.com/i/status/2119858261042036806)
- [Supplementary thread: honeypot captures and historical exposure counts](https://x.com/i/status/2119858262908514520)
- [New candidate relays GLM 5.3, 800A honeypots and rename-request research, November 10, 2026 at 08:02:24 Beijing time](https://x.com/i/status/2119943720531312936)

[中文](../claroty-danfoss-sonnet-known-bug-recreation-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
