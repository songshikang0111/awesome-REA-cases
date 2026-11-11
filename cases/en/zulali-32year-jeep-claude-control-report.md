# A 32-year-old Jeep: SCI diagnostics, fuel-trim formulas and why passing emissions is not proof of compliance

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-11
Stage: Needs verification

At 01:19:29 Beijing time on November 11, 2026, Muhammad (@zulali) says Claude reverse-engineered his 32-year-old Jeep and started controlling it. The post says the video was edited with Fable 5.2; the editing label does not identify the exact vehicle-research model. Earlier supplementary replies at 03:31:50, 03:32:09 and 03:37:37 call it a weekend experiment, point to a detailed video and repository in its description, and propose uploading some sessions. These are earlier supplementary materials, not new candidates in this 12:00–16:00 window. An intention to upload is not an available complete trace.

At 10:18:15, Mia Sardinella (@MiaSardinella) challenges the framing, citing existing documentation and open source and locating the value in diagnosis and repair. Diagnostic commands activating engine components are not steering, braking or autonomous driving. Earlier retrieval confirmed attribution and wording, not inspection of the cited repository or an independent vehicle audit.

At 12:52:01, fly (@dailingfei3) says they reviewed a ten-minute video and repository, identifying a 1994 Cherokee 4.0L with OBD1 and SCI serial communication. Their account credits a $3 Arduino with Claude Code/Codex for wiring, diagnosis, driving logs and reading the computer's program. A resistor reportedly suppressed the first signal; removing it yielded a first reading at 01:38. Roughly a week of work, a board made four months too early and missing programming components, loading a small program over three wires and writing EEPROM are fly's account, not read/write capabilities checked by this collection.

A concrete new evidence lead concerns fuel-trim direction: fly says a ChryslerScanner formula interpreted raw value 110 as +21.6% (initially about +22%), whereas disassembly of this firmware supported -4.7%, citing the calculation routine and a reset writing 128. The lesson offered is to check conversion before replacing parts; this collection did not inspect the disassembly or calculate those formulas, so they remain attributed. fly also describes a fuel pump activated for about ten seconds, project AGENTS.md rules requiring case-by-case human confirmation for clearing faults, resetting trims and actuator tests, and a warning not to identify pins by wire color alone. Written rules are not enforced isolation, nor is every read assumed absolutely safe.

fly reports initial NOx of 702 against a 539 limit at 25 mph, about $100 per inspection, and a retest result of 13 at both 15 and 25 mph. They also say the final modification is unclear, distinguish passing inspection from compliance and relay the owner's claim that legally questionable hidden controls were not used for inspection. The post cites California Vehicle Code 27156 and BAR software/Cal ID/CVN rules, but this collection did not read the law, inspection documents or modified code. It neither alleges illegality nor treats an old car being outside a particular check as proof of legality. Engine-state changes, emissions results and autonomous driving are distinct claims.

Supplementary retrieval here confirms fly's identity and full text only. The video, images, project repository, sessions, firmware and inspection reports were not read. Earlier uncertainty about model and functions is now supplemented with explicit secondary attribution, not independent confirmation. REA remains unmentioned. No target was downloaded, car connected, firmware modified or commands executed here; status remains unverified.

Older sealed candidate: 341 likes, 15,417 views, 25 reposts. Age and weekend duration are author descriptions, not measurements here.
Criticism candidate: 0 likes, 21 views, 0 reposts. No reviewable vehicle tests were supplied to this collection.
fly's sealed candidate: 1 like, 136 views, 0 reposts. The quoted original-post snapshot at 12:20 of 647,000 views and 5,387 bookmarks is secondary and does not replace older sealed metrics.

## Sources

- [Muhammad's old-Jeep/Claude reversing and control report, November 11, 2026 at 01:19:29 Beijing time](https://x.com/i/status/2120204711790023128)
- [Earlier supplementary author thread: weekend experiment and repository in video description, 03:31:50 that day](https://x.com/i/status/2120238017524928838)
- [Earlier supplementary author: repository link and intended session uploads, 03:37:37 that day](https://x.com/i/status/2120239476366864803)
- [Mia Sardinella distinguishes diagnostic commands from autonomous driving, November 11, 2026 at 10:18:15 Beijing time](https://x.com/i/status/2120340296147873894)
- [fly's detailed SCI, firmware fuel-trim and inspection/compliance account, November 11, 2026 at 12:52:01 Beijing time](https://x.com/i/status/2120378991718650300)

[中文](../zulali-32year-jeep-claude-control-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
