# FreeCAD binaries to MCP: a five-task DeepSeek/REA study of native interfaces

Category: Applications and clients · REA
Record date: 2026-11-26
Stage: Analysis test

At 03:01:26 Beijing time on November 26, 2026, Ao Qu (@ao_qu18465) introduces Agent-Native Computer Use: an agent receives software binaries and reversing tools, rewires interaction and builds MCP instead of clicking through screens. Morluto quotes the same work at 03:33:26. This window's 04:24:51 post by research author Paul Liang (@pliang279) explicitly names collaboration with the REA team and repeats the FreeCAD demo's 55× speed and 35× token reduction. These introduce one study, not three independent reproductions.

Supplementary reading locates MIT-MI's public research blog, pinned to c822a0c47cdea82fa28b3955a4216c80f1cc5db9 at 02:47:04 that day, before this window. It is supplementary documentation, not a new candidate. The blog specifies FreeCAD 0.20.2 binaries, REA and an offline sandbox without source, docs, network or evaluation tasks. DeepSeek V4.1 Flash handles both builds and tasks. The agent identifies embedded Python entry points among libpython3.11 exports, injects a script with Frida and calls FreeCAD's own Python API on the Qt main thread, producing an 85-tool server. Calls represent whole modeling operations, not individual clicks. Building precedes exposure to evaluation tasks; the server cannot change during evaluation. The public code-repository listing was located, but implementation was not reviewed file by file.

The project reports five tasks, board-plate, cable-slot, service-standoffs, lid-vent and enclosure, with respectively 9, 10, 10, 13 and 21 output-file checks and deadlines of 20, 20, 20, 40 and 90 minutes. Each setup runs each task three times. MCP passes every check, versus 40% on average for screen-based computer use. Starting files already pass 10%–33%, so these are not from-scratch models. Reported totals for five tasks are 4.5 minutes/3.1M tokens for MCP versus 180.6 minutes/127.1M, roughly 40× less of each; mean tool-call totals are 211 versus 1,466. The lid-vent demo is 44 seconds/0.64M versus 40 minutes/22.2M, which supplies 55×/35×, not the aggregate five-task ratio.

These figures exclude one-time server construction: three builds took 37, 30 and 85 minutes. In the no-REA ablation the agent can operate windows but not inspect files or processes, and its resulting servers pass no checks beyond the starting files. This demonstrates a difference in this experimental setting, not that all software requires reversing or all CAD tasks gain equally. Methods and tables are first-party reports; raw logs, complete grading code, token billing and statistical uncertainty were not reviewed. No checks were rerun, software built, process injected or dependencies installed. Fruit Ninja is a separate existing game entry; its scores do not validate FreeCAD.

Older sealed candidate: 22 likes, 1,227 views, 5 reposts, 6 replies. Paul Liang candidate: 18 likes, 1,160 views, 2 reposts, 3 replies. Performance and check counts are research-team reports, not rerun here.

## Sources

- [Ao Qu's Agent-Native Computer Use and FreeCAD comparison account, November 26, 2026 at 03:01:26 Beijing time](https://x.com/i/status/2125666188630073806)
- [Supplement: morluto quotes the same agent-native interface research, November 26, 2026 at 03:33:26 Beijing time; not an independent test](https://x.com/i/status/2125674241169539568)
- [Paul Liang introduces REA collaboration and the FreeCAD demo, November 26, 2026 at 04:24:51 Beijing time](https://x.com/i/status/2125687177313198563)
- [Supplementary pinned research blog: methods, five tasks, ablation and build costs; November 26, 2026 at 02:47:04 Beijing time commit, pre-window documentation](https://github.com/MIT-MI/Agent-Native-Computer-Use/blob/c822a0c47cdea82fa28b3955a4216c80f1cc5db9/index.html)
- [Supplementary pinned code-repository listing; November 26, 2026 at 02:06:11 Beijing time commit; implementation not reviewed file by file](https://github.com/MIT-MI/Agent-Native-Computer-Use-Code/tree/eda0ba7fd7163deb09ee36f7e0c337af9bae5418)

[中文](../aoqu-agent-native-freecad-binary-mcp-computer-use.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
