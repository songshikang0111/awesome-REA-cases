# Elecbrakes trailer braking: Claude reads Android bytecode, researchers test an authentication gap and coordinate fixes

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-23
Stage: Needs verification

At 20:36:56 Beijing time on November 23, 2026, a candidate introduces Claude-assisted Elecbrakes trailer-controller research. Supplementary reading of Patrick Forck and Jeremy McCarthy's November 19 Element Digital article establishes the first-party account. Their own remote unexpectedly connected to another trailer, prompting an investigation. Unfamiliar with Android Smali bytecode, they gave decompiled com.ElecBrake.Remote to Claude to analyze BLE characteristics, commands and authentication. They report 47 characteristics across four services, only 42 shown by the app, and absent authentication on brake control. Jeremy also used Claude to build Chrome Web Bluetooth research tooling and an Android tool not used in testing. Subsequent hardware experiments reportedly took about four hours, not the entire research, tool-building or disclosure process.

The authors state that tests used their own equipment on private roads or closed setups, reporting brake changes and state feedback. Firmware work was static only: visible update layers used CRC rather than signatures, but the separate bootloader region was not obtained and malicious firmware was not flashed. Persistent implantation was therefore not demonstrated. The article also corrects an initial assessment of the fixed firmware's update entry point: it requires an authenticated bonded connection, while future signing remains a vendor plan. No braking payloads, UUIDs or operating steps are reproduced here.

The article dates initial reversal to February, hardware testing to May, vendor notification to May 18, and fixes EB2 3.0.4.4.3 and VM1 1.3.4.2.1 to July 6, with coordination continuing until November 19 publication. Roughly sixty percent means the vendor's October 30 firmware-uptake figure among daily active EB2/VM1 users, not all sold controllers or today's proportion. The older ELBC 2000 had no fix as of the article. Supplementary retrieval of CVE-2026-96805 finds a PUBLISHED record dated November 20 at 18:58:14Z, distinct from the article's November 19 CISA-advisory date. It corroborates missing authentication, affected products and fix revisions, crediting both researchers. The article lists two further CVEs for replay and the update channel; their individual registrations were not read.

Both article and CVE record predate the candidate window and are supplementary tracing, not new candidates. AI use, hardware tests and coordination remain first-party reports; the registry is external documentary corroboration of the vulnerability and versions, not reproduction by this collection. The vendor's original notice, original tools and complete experiment logs were not checked. No device was connected, controller program run or firmware flashed. Model revision and REA are unspecified. Status remains unverified here; consult current vendor notices for safety decisions.

Sealed candidate: 3 likes, 97 views, 1 repost, 0 replies. About four hours refers only to the authors' hardware-test stage; roughly sixty percent refers to October 30 firmware uptake among daily active EB2/VM1 users.

## Sources

- [Secondary account of Claude-assisted Elecbrakes app analysis, November 23, 2026 at 20:36 Beijing time](https://x.com/i/status/2124844647403176032)
- [Supplementary first-party account: Forck and McCarthy's research, tests and disclosure, November 19, 2026, before the window](https://elementdigital.com.au/blog/brake-check-trailer-brakes-over-bluetooth/)
- [Supplementary public CVE record published November 20, 2026, before the window: authentication gap, models and fix versions](https://cveawg.mitre.org/api/cve/CVE-2026-96805)

[中文](../elecbrakes-claude-android-brake-audit-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
