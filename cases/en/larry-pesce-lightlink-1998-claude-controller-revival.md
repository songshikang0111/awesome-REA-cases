# A 1998 LightLink lights up again: Claude reads old firmware and schematics, a human replaces the controller and fixes wiring

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-24
Stage: Needs verification

At 02:47:43 Beijing time on November 24, 2026, a media author points to Larry Pesce's revival of a 1998 LED sign. Supplementary reading covers Bill Brenner's CYBR.SEC.Media report and Pesce's own November 23 Secure Ideas article. Both predate this candidate window and provide provenance only. The target is an Inova LightLink CFM16.200S-IP, a 200-by-16 red/green display bought at DEF CON and left unused for at least ten years because its software and Ethernet protocol were proprietary and undocumented. This did not crack that network protocol: Pesce bypassed the old controller and drove the panels directly.

Pesce says Claude used hardware photographs to find Yadid Ramot's 2015 project, read its PIC firmware and Eagle schematic, recovered scanning, clocking and ribbon pinouts, and recognized the voltage mismatch between a 5 V 74HC244 and the ESP8266's 3.3 V output, recommending level translation. Claude then wrote a timer-driven display driver, Wi-Fi setup, web preview, text playlists, REST API, FSEQ lighting-sequence playback and OTA firmware updates. Pesce says the assistant worked around PlatformIO network restrictions by obtaining another toolchain, compiled the firmware and checked FSEQ handling against the specification. These are project reports; no build was executed here.

Initial hardware tests showed missing green on the upper band. After Pesce supplied photographs, Claude suggested checking that data line. He found it grounded incorrectly, moved one jumper and reported normal operation. The human provided parts, wiring, measurements, power-on tests and judgment, and caught at least one model omission; AI did not independently repair the sign. Claude later used KiCad's API to design a through-hole PCB, wrote its own two-layer maze router when a third-party autorouter could not run, and reportedly passed DRC. The article explicitly says the board has not been fabricated or physically tested. An afternoon refers only to PCB design, not total restoration time. The public repository is linked by the original article; code, binaries and complete check records were not audited here, nothing was downloaded for execution and no hardware was connected. Pesce proposes displaying automated IoT-testing job status. REA use is unspecified; status remains unverified here.

Sealed candidate: 1 like, 57 views, 0 reposts, 0 replies. At least ten years means time unused; an afternoon is the reported PCB-design stage, not total project duration.

## Sources

- [Candidate: media author introduces Larry Pesce's project, November 24, 2026 at 02:47 Beijing time](https://x.com/i/status/2124937961007706132)
- [Supplementary first-party account: research, hardware wiring fix and unfabricated PCB, November 23, 2026, before the window](https://www.secureideas.com/teaching-a-1998-led-sign-new-tricks-with-an-ai-riding-shotgun/)
- [Supplementary media report by Bill Brenner, November 23, 2026, before the window](https://www.cybrsecmedia.com/ai-helps-security-researcher-bring-1998-led-sign-back-to-life/)
- [Public firmware and PCB repository linked by the first-party article; not executed or audited file by file](https://github.com/AppliedMalice/lightlink-esp8266)

[中文](../larry-pesce-lightlink-1998-claude-controller-revival.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
