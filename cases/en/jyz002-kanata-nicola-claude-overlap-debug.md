# NICOLA thumb-shift input: Claude-assisted kanata macro debugging, with 608 reported errors reduced to zero

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-04
Stage: Analysis test

At 02:23:45 Beijing time on November 4, 2026, @jyz002 describes Claude Code-assisted NICOLA adaptation on a MacBook9,1 running Ubuntu 26.04. NICOLA is a Japanese thumb-shift input method. This setup combines kanata 1.12.0 and Mozc: Eisu/Kana taps change kanata layers and send Hangul_Hanja/Hangul to turn Mozc off/on with one-shot actions. Kanata runs under a dedicated hardened systemd user; the author's own account is not in the input group.

Exhaustive two-key-pair testing in kanata_simulated_input reportedly found accidental Eisu layer changes and up to four concurrent macros interleaving ka and ta as k t a. The fixes require a tap under 150 ms with no output in the preceding 200 ms, and insert 6 ms only immediately after other output. The author reports 608 broken two-key pairs reduced to zero. This does not cover every real typing situation; NICOLA's three-key rule still cannot be expressed in kanata configuration. The program sees all keystrokes and the post explicitly warns of risk. No private input was read, configuration run or figures retested. This is independent of the same post's speaker-driver investigation; audio results are not input-test evidence.

November 4 candidate snapshot: 1 like, 25 views, 0 reposts. The 608-to-zero result is the author's simulated two-key-pair test.

## Sources

- [@jyz002's kanata/Mozc debugging and unresolved three-key rule, November 4, 2026](https://x.com/i/status/2117684171720233121)

[中文](../jyz002-kanata-nicola-claude-overlap-debug.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
