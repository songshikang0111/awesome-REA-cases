# macOS accessibility trees: DailyAIDev proposes AXUIElement and Swift instead of guessing click coordinates from screenshots

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-09
Stage: Related project

At 12:21:43 Beijing time on November 9, 2026, 木言 (@DailyAIDev) describes studying macOS's AXUIElement accessibility tree and using a native Swift scheduling engine instead of repeatedly taking screenshots and visually inferring click locations in Computer Use. The intended problems are latency, API expense and multi-monitor offsets. A supplementary author reply at 14:59:02 argues for obtaining controls' hierarchy and geometry from the system to avoid pixel errors from window movement, scaling and high DPI. That reply is contextual evidence, not another candidate.

This is a related-project claim about exposing target applications' visible control structures to AI desktop automation, not demonstrated reversing of WindowServer or private APIs. The author's explanation involving kernel handles lacks source or call traces. Advertised zero-millisecond memory queries, 100% absolute coordinates and $0 offline operation have no hardware, benchmark, coordinate-system description or invoices. They do not establish complete trees for every app, accuracy across every monitor layout, or zero model cost for an entire AI task.

The linked long-form article was not read, and no named repository, Swift implementation, permission requirements or test records were obtained. The public thread contains discussion and intentions to try it. No engine or macOS automation was run here. Retained only as a concrete UI-research and automation approach, without promoting advertising to usability or performance verification. REA use is not confirmed.

Sealed candidate: 7 likes, 683 views, 0 reposts. Performance and cost are promotional claims, not independent measurements.

## Sources

- [DailyAIDev introduces AXUIElement and a Swift engine, November 9, 2026 at 12:21:43 Beijing time](https://x.com/i/status/2119646592831799433)
- [Supplementary author reply on control hierarchy, geometry and scaling, November 9, 2026 at 14:59:02 Beijing time](https://x.com/i/status/2119686182020010356)

[中文](../daily-aidev-macos-accessibility-swift-computer-use.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
