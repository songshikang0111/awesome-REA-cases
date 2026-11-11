# Nichicon battery ECHONET Lite: Gemini, HEX and remote-control comparisons show an acknowledgment is not execution

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-11
Stage: In progress

At 17:00:28 Beijing time on November 11, 2026, @Masato1864646's TechFeed roundup lists a second ECHONET Lite/Gemini article. Supplementary title search through Qiita's public API locates matsukawa's original, published that day at 05:24:46 and updated 05:27:21 Beijing time, before this window. It recalls work from late August to early September; publication is not the experiment date. The goal is self-built home-energy management: read a Nichicon battery and household power, then schedule charging/discharging without buying a roughly ¥10,000 Wi-SUN module and applying for a smart-meter B-route. The author chooses existing LAN and standard ECHONET Lite UDP interfaces, initially generating Python in browser Gemini, manually copying/running it and feeding errors back. Antigravity comes later in the current workflow.

The author first requests Panasonic AiSEG3 branch-circuit readings. Naively decoding two bytes as an unsigned integer yields abnormal 8–9 kW readings. Bytewise HEX analysis with Gemini reportedly reveals circuit attributes in the high bits, so the entire word is not current. Large packets and slow polling prompt a battery Get-property-map investigation. A suspected vendor extension, 0xF5, has 12 bytes compared against live remote-display values: signed grid import/export power in the first four bytes, reserved middle bytes and solar power in the last four. Combined with standard charge/discharge readings, it reportedly yields household load. Field interpretation and calculation effectiveness remain author tests without original captures recomputed here.

For scheduling, standard power-limit fields initially return success while the displayed times remain unchanged. Comparing full-property HEX dumps under two manually configured schedules then locates a 21-byte 0xF4 extension; the author reports schedule changes taking effect. An ongoing discharge does not stop immediately after a schedule change, prompting separate operating-mode control. The article describes inverter-transition anomalies overflowing SQLite, followed by length/range validation, skipping bad readings and retaining the previous value. Its enormous power figures are inconsistent with the 32-bit explanation and are not copied as reliable measurements.

At 9% charge, application logic entering standby below 10% reportedly makes recovery immediately return to standby, missing night charging. The author describes a charging-period state-machine exception as a fix. This records the failure and claimed treatment, not a recommendation to copy safeguard exceptions or proof of battery safety, manufacturer-protection behavior or electrical compliance. The article also identifies competing UDP ports across scripts and local copy-paste fixes that erase existing safeguards, motivating a planned specification-driven agent refactor. Exact device model, firmware, model version, full project, long-term savings and independent safety tests are absent. REA is unmentioned. This collection only read the article, sending no control packets, connecting no equipment and running no code.

Whole roundup sealed snapshot: 2 likes, 514 views, 0 reposts, not engagement with the original article or a battery result. Device control was not reproduced by this collection.

## Sources

- [TechFeed's second ECHONET Lite/Gemini analysis article listing, November 11, 2026 at 17:00:28 Beijing time](https://x.com/i/status/2120441519195013509)
- [Supplementary original: matsukawa recalls August–September research; published November 11, 2026 at 05:24:46 and updated 05:27:21 Beijing time, before the window](https://qiita.com/matsukawa/items/35a232fef2e345c9a489)

[中文](../gemini-echonet-lite-code-copy-analysis-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
