# Eleven: agent-assisted analysis of apps and binaries

Category: Applications and clients · REA use unconfirmed
Record date: 2026-11-10
Stage: Needs verification

The poster introduces Eleven as a self-made agent-assisted reverse-engineering tool. It reportedly opens Mac apps, Android APKs and Windows/Linux binaries, with function views for pseudocode, assembly, graphs and hex. Users can ask Claude, Codex, Gemini, Cursor or ACP agents questions, inspect analysis steps, and accept or undo proposed function renames and comments. The post also claims safe byte editing on copies, build comparisons and lldb debugging. This scope and free/open-source status are the author's introduction only. No repository link, code verification or independent runtime tests were available in this review. The post does not explicitly establish REA use.

On 2026-10-15, the poster says Eleven received a major update and describes an agent-first reverse-engineering app that opens applications or binaries for agent-assisted dissection. This is the product author's update announcement; it supplies no concrete target-analysis case or validation record and does not confirm REA use.

At 19:18:56 Beijing time on November 10, 2026, Chizi (@chiziaruhoma) says Eleven now runs inside his terminal. It is not rewritten as a TUI: the same app is GPU-rendered in a hidden window, streamed frame by frame into Ghostty, with mouse and keyboard input sent back. He asks Claude what a binary does at startup and says Claude works through Ghidra inside the terminal. This adds a terminal embedding and research interaction, not a target-app rewrite or automated cracking.

Supplementary retrieval confirms attribution, text and a video attachment, not a viewing of it. Bridge implementation, target binary, analysis output, latency and input compatibility tests were not obtained. The author calls it rough; all old functionality, cross-platform testing and total GUI replacement are not established. The new post does not identify REA, so unknown is retained. Eleven was not installed and Ghidra was not run here. Earlier third-party architecture claims remain attributed in metadata.

Author describes software as free and open source; no verifiable project link or independent tests supplied.
REA use unconfirmed.
2026-10-15: author announces a major Eleven update; specific analysis results and REA use are not confirmed by that post.
Two third-party introductions added this review claim Ghidra, LLDB and REA underneath, GPUIX in front, ACP/MCP agent control of control-flow and decompiler views, and Metal shader and on-device model analysis. These are not code verification by this collection. The REA field remains unknown; retelling alone cannot confirm the author's implementation.
First circulating post's snapshot this review (2026-10-15): 98 likes | 7,668 views | 16 reposts; separate from older author-post metrics.
A new October 15, 16:00–20:00 introduction says Ghidra is called through REA, Rizin is also supported and Android uses jadx. It emphasizes undoable edits and patches written to copies without overwriting originals. This adds product claims about editing safeguards, not code-inspected confirmation or a guarantee of no side effects. The REA field remains unknown.
November 10 sealed candidate: 11 likes, 439 views, 1 repost. Terminal demonstration is author-reported, not runtime verification by this collection.

## Sources

- [Author's original Eleven release post](https://x.com/i/status/2110035757691703722)
- [Author's original Eleven update post](https://x.com/i/status/2110476050815983632)
- [Third-party tool introduction this review (REA attribution is secondhand)](https://x.com/i/status/2110603171920023720)
- [Third-party architecture and feature claims this review](https://x.com/i/status/2110634488938275080)
- [This October 15 window: copies, undo and toolchain introduction](https://x.com/i/status/2110655118282781161)
- [Chizi on Ghostty embedding and Claude/Ghidra, November 10, 2026 at 19:18:56 Beijing time](https://x.com/i/status/2120113977589907635)

[中文](../eleven-agent-reverse-engineering.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
