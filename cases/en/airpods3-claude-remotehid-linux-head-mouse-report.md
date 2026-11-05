# AirPods 3 as a head-controlled mouse: a report of Claude Code studying RemoteHID and Linux MTU

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-05
Stage: Needs verification

At 21:17:00 Beijing time on November 5, 2026, a Chinese retrospective describes a developer wanting AirPods 3 to act as a head-controlled mouse on Linux, after five consulted open-source projects marked it unsupported. It says Claude Code first failed at roughly 300 Bluetooth probes. A human stopped the blind attempts and redirected research toward Wireshark plugins, reverse-engineered clone-earbud material and public iOS framework pseudocode, combining clues from six or seven projects.

The post attributes the breakthrough to AirPods 3 using RemoteHID rather than the Pro sensor path, plus a Linux-default MTU of 672 versus iOS's 2582. It claims 200Hz motion data after the change and subsequent driver, console UI, 37 automated tests and public protocol documentation. These numbers and causal explanations are a retelling, not packet captures, hardware comparisons or test results from this collection. They do not establish that changing MTU works on every headset and system. 'First public' and all previous projects' capabilities were not verified.

A pinnable repository, developer identity, commit, full protocol document and readable original retrospective were not obtained. Supplementary search found a similar earlier same-day retelling, used only as a lead, not a replacement candidate. Retained as an unverified concrete interoperability experiment, not encryption cracking or a production driver. No Bluetooth device, cursor control, driver or test was exercised here. REA is not mentioned.

Sealed snapshot: 11 likes, 1,297 views, 0 reposts. Roughly 300 attempts, 200Hz and 37 tests are secondary claims, not independent reruns.

## Sources

- [Chinese AirPods 3/Claude Code/RemoteHID retrospective, November 5, 2026 at 21:17:00](https://x.com/i/status/2118331749214175491)

[中文](../airpods3-claude-remotehid-linux-head-mouse-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
