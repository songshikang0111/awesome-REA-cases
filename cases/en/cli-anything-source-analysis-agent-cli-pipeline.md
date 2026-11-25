# CLI-Anything: source-derived agent command lines, with runtime and telemetry limits

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-25
Stage: Related project

A Chinese post at 00:14:26 Beijing time on November 22, 2026 introduces HKUDS CLI-Anything: command-line layers for Blender, GIMP, FreeCAD, Obsidian and LibreOffice, replacing screenshot-driven clicking for agents. Its seven-step pipeline scans source, defines command groups, creates a Click CLI with REPL/JSON and undo/redo, then tests, documents, publishes and emits SKILL.md. The research targets readable source and software controls, not established universal closed-binary handling.

The post claims real backend calls and reports 2,461 tests, 208 Blender tests, 258 FreeCAD commands, a rover model and a four-minute HTTPS diagram demonstration. Repository test output, command inventories and demo records were not obtained. Its 61,868 stars and third-place trend ranking are contemporaneous post claims, not independently checked. The author also warns about strong-model dependence, poorer results without source and multiple refine passes.

At 14:25:49 Beijing time on November 25, 2026, Felix (@Stevezh1f) adds two routes: existing cli-anything-hub harnesses or generating a new harness, explicitly without hands-on testing. He relays prerequisites of target source and installed real applications. Strong-model examples are Claude Opus 4.6, Sonnet 4.6 and GPT-5.4; weaker models may generate incomplete or wrong CLIs, and multiple refine passes are usually needed. Python 3.10 or later is required; on Windows, Claude Code needs Git for Windows including bash or WSL, and generation consumes model quota. The post also says cli-hub sends anonymous events to PostHog by default, with CLI_HUB_NO_ANALYTICS=1 as an opt-out, and warns that agents connected to real software can execute commands and need scoped authorization. These are relayed deployment/privacy constraints, not telemetry switches or complete support verified here.

Felix cites an observation at 20:06 Beijing time on November 24 of 1,075 stars added that day and approximately 64,200 total, clarifying that the day was UTC-based and not over, and describes an Apache-2.0 license. These were not independently rechecked. Included as a related project for AI analysis and agent interoperability. No installation or generation commands were run; complete software coverage, passing tests and binary recovery are unverified. Model names are workflow context in the posts, not models tested here. REA use is unconfirmed.

November 22 sealed candidate: 2 likes, 300 views, 0 reposts, 8 replies. Repository stars and test counts were not rechecked.
November 25 sealed candidate: 1 like, 33 views, 0 reposts, 0 replies. The quoted star snapshot is from November 24 at 20:06, not a November 25 measurement.

## Sources

- [Chinese account of HKUDS CLI-Anything's seven-step pipeline and limits, November 22, 2026 at 00:14:26 Beijing time](https://x.com/i/status/2124174608618168350)
- [Felix adds source/runtime, model and PostHog telemetry limitations, November 25, 2026 at 14:25:49 Beijing time; explicitly not hands-on tested](https://x.com/i/status/2125476030005526899)

[中文](../cli-anything-source-analysis-agent-cli-pipeline.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
