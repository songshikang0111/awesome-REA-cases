# A 32-year-old Jeep: SCI diagnostics, fuel-trim formulas and why passing emissions is not proof of compliance

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-14
Stage: Needs verification

At 01:19:29 Beijing time on November 11, 2026, Muhammad (@zulali) says Claude reverse-engineered his 32-year-old Jeep and started controlling it. The video was edited with Fable 5.2; that label does not identify the exact vehicle-research model. Earlier supplementary replies at 03:31:50, 03:32:09 and 03:37:37 call it a weekend experiment, point to the video and its repository link, and propose uploading sessions. These are November 11 background, not new candidates in this November 14 window; intended uploads are not a complete public trace.

At 10:18:15 on November 11, Mia Sardinella (@MiaSardinella) questions the framing, crediting existing documentation/open source and emphasizing diagnosis and repair. Diagnostic engine-component commands are not steering, braking or autonomous driving. Earlier retrieval confirmed wording and attribution, not an independent vehicle audit. At 12:52:01 that day, fly (@dailingfei3) says they reviewed a ten-minute video and repository, identifying a 1994 Cherokee 4.0L, OBD1 and SCI serial communication. They credit a $3 Arduino plus Claude Code/Codex with wiring diagnosis, drive logs and program reading. A resistor reportedly suppressed the initial signal; removing it yielded readings at 01:38. Roughly a week of work, a programming board made four months earlier and missing parts, loading a small program over three wires and writing EEPROM are fly's account, not read/write capabilities verified here.

fly also says a ChryslerScanner formula interpreted raw 110 as +21.6% (initially about +22%), whereas this firmware's disassembly supported -4.7%, citing the calculation routine and a reset writing 128. This collection did not inspect disassembly or calculate the formulas. Checking conversion before replacing parts is the author's recommendation. A fuel pump reportedly activated for about ten seconds and AGENTS.md rules requiring individual confirmation for clearing codes, resetting trims and actuator tests are also attributed. Written rules are not enforced isolation, and reads are not universally safe.

fly reports initial NOx of 702 versus a 539 limit at 25 mph, inspections at about $100, and retests of 13 at both 15 and 25 mph. They say the final modification is unclear, passing inspection is not compliance, and relay the owner's claim that legally questionable hidden controls were not changed for inspection. Their California Vehicle Code 27156 and BAR software/Cal ID/CVN references were not checked against law, inspection documents or modified code here. Neither illegality nor legality from an old car falling outside a particular check is inferred.

The new November 14 candidate at 19:39:47 names xj-scanner and reports SCI at about 7,800 baud with inverted signaling, about $15 in materials and Codex-written EEPROM-related code. Supplementary reading covers MZULALI/xj-scanner's README pinned at 9239683, dated November 10, 2026 at 17:03:04 UTC, before the candidate and used only as primary-project background. It explicitly says it was built and tested on one 1994 Jeep Cherokee XJ 4.0L with computer 56030117; other 1991–95 SBEC-family units are only expected to be similar. It lists about $15 of materials, a $3 Nano, fault codes, live data, drive logging and built-in tests. It warns of 12 V in the diagnostic connector and against identifying wires by color; wiring procedures are not reproduced here.

The README credits László Dániel's ChryslerScanner for parameter IDs, scaling, OBD1 messages and fault-code text, and existing SBEC disassembly in AR1972/jeep_2.5L for the fuel-trim scale. This strengthens the human/open-source foundation, not a claim that AI independently discovered every field. The project is GPLv3. The read README does not independently establish EEPROM rewriting, 7,800 baud, final emissions results or compliance; those remain attributed reports. The old unread-repository limitation is updated only to having read a pinned README: video, full source, firmware, sessions and inspection documents remain unreviewed. No car was connected, target downloaded, firmware modified or commands executed here. REA is unmentioned; status remains unverified.

Older sealed candidate: 341 likes, 15,417 views, 25 reposts. Age and weekend duration are author descriptions, not measurements here.
Criticism candidate: 0 likes, 21 views, 0 reposts. No reviewable vehicle tests were supplied to this collection.
fly's sealed candidate: 1 like, 136 views, 0 reposts. The quoted original-post snapshot at 12:20 of 647,000 views and 5,387 bookmarks is secondary and does not replace older sealed metrics.
New November 14 candidate: 0 likes, 31 views, 0 reposts, 1 reply. The primary README reports only one tested car, not cross-model certification.

## Sources

- [Muhammad's old-Jeep/Claude reversing and control report, November 11, 2026 at 01:19:29 Beijing time](https://x.com/i/status/2120204711790023128)
- [Earlier supplementary author thread: weekend experiment and repository in video description, 03:31:50 that day](https://x.com/i/status/2120238017524928838)
- [Earlier supplementary author: repository link and intended session uploads, 03:37:37 that day](https://x.com/i/status/2120239476366864803)
- [Mia Sardinella distinguishes diagnostic commands from autonomous driving, November 11, 2026 at 10:18:15 Beijing time](https://x.com/i/status/2120340296147873894)
- [fly's detailed SCI, firmware fuel-trim and inspection/compliance account, November 11, 2026 at 12:52:01 Beijing time](https://x.com/i/status/2120378991718650300)
- [New candidate: Jeep/xj-scanner SCI and EEPROM report, November 14, 2026 at 19:39:47 Beijing time](https://x.com/i/status/2121568773425520720)
- [Pre-window pinned xj-scanner README: single-car testing and prior-research credits, commit November 10, 2026 at 17:03:04 UTC](https://github.com/MZULALI/xj-scanner/blob/9239683e5743b9294f26358366a9c5a744a329d5/README.md)

[中文](../zulali-32year-jeep-claude-control-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
