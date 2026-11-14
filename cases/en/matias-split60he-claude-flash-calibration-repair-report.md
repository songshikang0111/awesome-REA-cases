# Split60HE nonstop keypresses: Matías reports Claude decoding flash calibration settings to repair a used keyboard

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-15
Stage: Needs verification

At 03:52:44 Beijing time on November 15, 2026, Matías (@matias_1g) reports repairing a used Split60HE bought on Mercari: a split Hall-effect keyboard with a trackball whose right half continuously typed every key. Same-author replies from 03:53:07 through 03:54:26 were read as supplementary sources for the candidate, not additional candidates.

The author says Claude read the open-source firmware and KiCad PCB files to understand communication between the halves, then wrote a tool to read live sensor data over USB. The sensors reportedly worked, yet all 39 right-side keys showed 100% pressed. The keymap's bootloader key also triggered, repeatedly putting the right half into bootloader mode. A chip-flash dump and decoded settings log reportedly revealed that the last two writes changed the resting calibration value from 2400 to 2350 and then 1200. The author attributes the fault to that value, not recovery of original closed-source firmware.

The final reply reports backing up both halves, erasing them, flashing v1.11 with byte-by-byte checks and setting a resting value of 2700 for these sensors. All 69 keys then reportedly read 0% at rest, without soldering or new parts. One session is not timed working hours, and these values are not universal calibration advice for every Split60HE. No firmware repository URL, dump, settings log, patch, USB trace or long-term key test was obtained. No image was interpreted, firmware flashed or keyboard connected here. This records the author's AI-assisted investigation of an existing device fault; REA is unmentioned and neither the repair nor sensor diagnosis was independently verified.

Original sealed candidate: 0 likes, 3 views, 0 reposts, 1 reply. The 39 keys refer to the faulty right half; 69 to all keys after repair, not two independent reproductions.

## Sources

- [Matías's Split60HE fault and Claude repair report, November 15, 2026 at 03:52:44 Beijing time](https://x.com/i/status/2121692829080793468)
- [Same-thread supplement: open firmware, KiCad and 39-key USB readings, 03:53:07](https://x.com/i/status/2121692925117563011)
- [Same-thread supplement: bootloader key triggering reboots, 03:53:39](https://x.com/i/status/2121693062003105867)
- [Same-thread supplement: flash settings log and 2400/2350/1200, 03:53:50](https://x.com/i/status/2121693105128894521)
- [Same-thread result: v1.11, 2700 calibration and 69 keys at 0% at rest, 03:54:26](https://x.com/i/status/2121693258610835862)

[中文](../matias-split60he-claude-flash-calibration-repair-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
