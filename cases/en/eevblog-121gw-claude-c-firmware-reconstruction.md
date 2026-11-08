# 121GW multimeter: Dave Jones reports completed Claude Code C reconstruction and a hardware-test video

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-07
Stage: In progress

At 12:50:30 Beijing time on November 2, 2026, EEVblog's Dave Jones (@eevblog) endorses 121GW firmware reversing by a forum user who did not own the meter, and separately says Claude Code is working on his C reconstruction. At 14:18:49, Cozy asks how C behavior is validated; the retrieved older thread has no answer. The forum user's work and Dave's AI work remain separate attributions; one does not validate the other.

The November 4, 06:35:38 candidate announces EEVblog 1784, titled 'Claude Code Reverse Engineer 121GW Firmware SUCCESS', claiming a working entire firmware C reconstruction with one prompt in under 24 hours. The body once says 12GW, inconsistent with the 121GW title; the title's target is retained, not a newly invented model. The contents list connecting a 121GW through ST-LINK V2 at 02:39; GCC/Ghidra installation at 11:50; completed bootloader at 14:47; firmware completed next morning at 19:39; testing Zombu4's assembler version at 23:14; direct programming discussion at 24:23; human testing at 29:20; real hardware and source at 30:10; conventional binary download at 32:29; and checking Bluetooth at 33:54. The new result is an author's completion and hardware-test report, not merely ongoing progress.

A new window retelling at 14:02:51 on November 4 claims Claude Code rebuilt the bootloader and full application with 691 functions from the binary, running on real hardware including Bluetooth. This is more explicit than the video's Bluetooth question, but remains a third party's interpretation of the same demonstration, not another hardware test. No function inventory or Bluetooth log is supplied; neither equivalence of all 691 functions nor a Bluetooth pass verified by this collection is established.

This collection read the post and retrieved the original, but did not watch the video, expand short links, inspect source/forum material or obtain test outputs. A Bluetooth question in the contents is not a confirmed pass, nor does the announcement establish full equivalence, measurement accuracy, calibration, electrical safety or a replacement suitable for the original firmware. Under 24 hours and one prompt are author figures, not unattended work: human wiring, programming and testing appear in the contents. Zombu4's assembler version is not automatically an AI result. REA is not mentioned. No dependencies were installed, target code run, meter connected or firmware flashed.

A new Japanese retelling at 17:53:02 Beijing time on November 7, 2026 further describes the public repository's scope: a custom SD-card bootloader and v2.05 measurement application on STM32L152xD, with FatFs and the C runtime in addition to 691 functions. ST's ROM bootloader is documented only, not reimplemented. It describes Ghidra scripts, Unicorn differential-test harnesses, function mapping and memory maps, comparing original and rebuilt bootloaders, individual functions and whole application images. The undistributed original flash dump is required. Emulator equivalence and hardware testing are claimed, along with under-24-hour, one-prompt work within the author's basic $25 monthly plan. This is a secondary account of EEVblog and a repository, not source inspection or testing performed here, and $25 is not a measured model bill for this case. Claimed late-stage tests and fixes without author input do not erase earlier human wiring/programming. The separately tested Zombu4 assembly version is not conflated with AI work. Measurement accuracy, electrical safety and full compatibility remain unestablished.

November 7 sealed candidate: 0 likes, 385 views, 0 reposts. New hardware/revision/test scope is secondary reporting, not source or metrology verification.
November 2 main candidate: 49 likes, 2,795 views, 4 reposts; question: 0 likes, 63 views, 0 reposts. Historical snapshots retained.
November 4 candidate: 46 likes, 1,364 views, 4 reposts. One prompt, under 24 hours and working firmware are author reports, not independently checked.
New 14:02 retelling candidate: 0 likes, 49 views, 0 reposts. The 691 functions and working Bluetooth are unverified here.

## Sources

- [Dave Jones endorses forum 121GW reversing and describes Claude Code progress, November 2, 2026](https://x.com/i/status/2117117123134967821)
- [Supporting reader question: how is C behavior checked? November 2, 2026 at 14:18:49 Beijing time](https://x.com/i/status/2117139347879415851)
- [EEVblog 1784: C-reconstruction completion and hardware-test video contents, November 4, 2026](https://x.com/i/status/2117747558344962144)
- [Window third-party retelling claiming 691 functions and working Bluetooth, November 4, 2026 at 14:02:51 Beijing time](https://x.com/i/status/2117860102908887349)
- [Japanese account of 121GW repository scope and Unicorn/dump requirements, November 7, 2026 at 17:53:02 Beijing time](https://x.com/i/status/2119005193673351330)

[中文](../eevblog-121gw-claude-c-firmware-reconstruction.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
