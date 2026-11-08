# 2009 Kindle 2: Codex-assisted 4bpp driver, partial-refresh and cover-Home changes

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-09
Stage: In progress

At 03:28:37 Beijing time on November 9, 2026, Radacted (@onehit42) reports letting Codex maintain a 2009 Kindle 2: jailbreak, access restriction, partition backups, firmware updating and clock repair after an aging battery, followed by work on the existing display driver and Home program to keep the reader useful. Retrieval of the full original confirms the details below; an incomplete candidate ending does not make the entire report unusable.

The author says a paired 4bpp conversion loop was developed and installed for this exact driver, preserving pixel conversion results, controller commands, hardware waits, factory waveform data and temperature handling. Checks reportedly included ARM-code comparisons, controller image-RAM readbacks, diagnostic patterns and restarts. Reported median software page response fell from about 430 ms to 330–340 ms (about 24%), and image-loading work from about 130 ms to 23 ms (82%). These are not measurements by this collection or necessarily whole e-ink display refresh times.

A narrow request interceptor handles ordinary portrait stock-reader page turns, checking page-key input, reading rectangle, timing and request buffer before substituting partial updates. After trying six- and ten-page cleanup intervals, manual cleanup was selected; Shift then F requests a full refresh. Menus, opening books and unmatched operations keep native behavior. Home uses guarded hooks in two native classes plus a Java helper compatible with the old JVM, indexing 35 books with four large covers per screen, Recent/All views and ten series folders in reading order. Titles were cleaned and title cards made for unsuitable covers.

According to the author, original book paths were preserved, all 35 files matched their pre-change copies byte for byte, and MOBI, PDF and protected Kindle books opened in the native reader at saved positions. Original Menu/Settings and stock Home remain available. The author reports a very weak battery and has not supplied a video comparison because it would show copyrighted material. No patch, source, raw timing logs or battery/long-term ghosting tests were obtained. This does not generalize to other Kindles or all pages, or establish DRM removal. No device was flashed or retested here; REA is unmentioned.

Sealed snapshot: 3 likes, 108 views, 0 reposts. Percentages, timings and the 35-file check are author-reported.

## Sources

- [Radacted's full Kindle 2 modification and self-test report, November 9, 2026](https://x.com/i/status/2119512432859341049)

[中文](../kindle2-codex-4bpp-refresh-home-hooks.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
