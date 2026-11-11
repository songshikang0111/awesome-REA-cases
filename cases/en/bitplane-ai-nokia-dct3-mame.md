# Nokia DCT3: bitplane adds a terminal-game Easter egg motive and pending hardware dumps to the MAME project

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-11
Stage: In progress

At 17:05:27 Beijing time on October 24, 2026, davidsong (@bitplane) reports AI-assisted reverse engineering of old Nokia DCT3 phones for a MAME driver, expecting several more months. The purpose is platform emulation/preservation, not unlocking or an Android port. AI attribution comes from the overall list without a named model or REA invocation.

The previously reviewed nokia-dct3-re README is pinned to a revision changed at 02:24:23 Beijing time on October 23, 2026. It identifies Nokia 3210 NSE-8/9 and MAD2 as reference; other DCT families are research directions. Reported progress includes an interactive desktop, Phone book entry through a physical-key input path, peripheral regressions and second-ROM checks. Keys refer to emulator input, not this collection's hardware tests. It separates DSP, radio, GSM and external-service protocol HLE from full silicon emulation. A 32-frame native-DSP codec reference check does not establish native whole-handset speech or a call lifecycle. RF, frequency hopping and broader peripherals remain limited. Firmware is not bundled and must be legally supplied.

A new post at 23:56:51 on November 11 explains the motive: a Nokia 3210 Easter-egg level in the author's terminal game, with a MAME emulator for correct timings and progression. The surrounding project is described as a 130,000-line 2.5D terminal scene API with ANSI animation, GUI, TeleText and font tools. That is the author's context and count, not the DCT3 driver's size. Although he broadly says he reversed all DCT3 phones, he immediately says weeks of work and chip-firmware extraction from eBay-purchased hardware remain, perhaps another month or two overall. Family-wide compatibility is not established. The comparison to a decade of human work is rhetoric, not measured elapsed or saved labor.

The post also mentions an open-source TeleText converter/font engine, handcrafted terminal fonts and ongoing VFX and 1990s-style mod-tracker work. These provide game context, not separate completed AI-reversing outcomes. No new firmware dumps, device matrix, tests or upstream-merge evidence were obtained. This collection read text and earlier documentation only, acquired no firmware and ran no emulator. Status remains in progress. The newer one-to-two-month and older several-month estimates are expectations at their respective dates, not release commitments.

3210 reference work, not completed family-wide support. Interactive desktop and 32-frame DSP reference checks are project reports; HLE is not complete silicon or native calling. Nothing was run.
November 11 candidate: 0 likes, 8 views, 0 reposts. The 130,000-line figure concerns the surrounding terminal project; a decade is not measured work, and one or two months is an author estimate.

## Sources

- [bitplane's ongoing Nokia DCT3/MAME report, October 24, 2026](https://x.com/i/status/2113919789886218477)
- [Supplementary nokia-dct3-re README, last changed October 23, 2026 Beijing time](https://github.com/bitplane/nokia-dct3-re/blob/f729fab82ae8d5ba4dd3ab8f60ffa80c5cb202b1/README.md)
- [Author adds the Nokia 3210 game Easter egg motive and pending hardware dumps, November 11, 2026 at 23:56:51 Beijing time](https://x.com/i/status/2120546305671873018)

[中文](../bitplane-ai-nokia-dct3-mame.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
