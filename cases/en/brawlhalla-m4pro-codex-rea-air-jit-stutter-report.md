# Brawlhalla stutter: Codex/REA traces AIR's interpreter branch under Rosetta

Category: Games and preservation · REA
Record date: 2026-11-02
Stage: Analysis test

At 15:48:28 Beijing time on November 2, 2026, fexx_off (@fexx_off) reports brief freezes in the fighting game Brawlhalla on a MacBook Pro M4 Pro. Offline Training was affected too, with more noticeable stutter in Free-for-all games with more than two players. The author used Codex, GPT 6.1 sol and REA. FPS targets, fullscreen and clean launches did not eliminate the freezes; fullscreen helped only somewhat.

According to the author, REA helped inspect the installed application and collect evidence. Native stack sampling and binary inspection led to the bundled Adobe AIR runtime: this build deliberately selects ActionScript interpreter-only execution rather than JIT compilation when it detects Rosetta. The investigation found an existing AS3JIT=2 configuration override, tested it temporarily with a shared-configuration backup and automatic restoration after startup, and took a fresh sample that no longer showed the previously recurring interpreter call path. The author then personally played Training and Free-for-all and reports freezes 'basically gone' in both, before asking Sol to persist the setting for normal Steam launches.

This is an author-reported chain from symptoms to a runtime decision, configuration experiment, resampling and human play-testing, not a reproduction by this collection. Game/AIR versions, code addresses, stacks, the full configuration location, frame-time distributions, test duration and a reverted-setting control are not published. It does not guarantee effectiveness across Macs, AIR versions or modes, and the absence of one sampled call path does not quantify performance gains. Original-post lookup confirms attribution and full text. No game was run, configuration changed or independent test obtained here.

Sealed candidate snapshot: 1 like, 21 views, 0 reposts; neither a popularity winner nor independent validation.
AS3JIT=2 and improvements in both modes are author reports without quantitative frame times or raw samples.

## Sources

- [fexx_off's Codex/REA sampling, AIR-branch and play-testing report, November 2, 2026](https://x.com/i/status/2117161909883408416)

[中文](../brawlhalla-m4pro-codex-rea-air-jit-stutter-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/games.md)
