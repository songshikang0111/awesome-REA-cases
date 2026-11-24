# Netflix serves IntelliJ's index to agents: less blind text search after JAR decompilation

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-24
Stage: Analysis test

At 09:50:14 Beijing time on November 24, 2026, @eltc9584 discusses Java agent-navigation research presented by Netflix engineer Paul Bakker. The post says agents faced with dependencies commonly shipped as JARs unzip them, sometimes decompile class files and search text, missing types, dependencies and structure. Netflix ran IntelliJ IDEA's indexing engine without the IDE and built a daemon and CLI for Claude Code and Codex, improving this reverse-reading workflow with semantic code understanding. It is not recovery of every Java library's original source or an external attack on closed Netflix services.

The poster recounts July/August experiments on an internal service and the open-source DGS Framework: typically 20–30% improvement in combined token/time efficiency, with a best case of roughly 65% for the strongest model at high effort on code-navigation tasks; correctness stayed steady or improved. The figures are described as an October case-study snapshot. Netflix built the daemon because JetBrains had not yet supplied one. The post also says the capability ships in Java & Kotlin by IntelliJ IDEA and benchmarks are planned for Python, TypeScript/JavaScript and Go. Combined efficiency is not rewritten as separately saving 65% of both tokens and time; planned languages are not treated as tested support.

Supplementary retrieval of the quoted JetBrains post, dated November 23 at 17:57:04 Beijing time, confirms an official description of bringing Java structure understanding to agents. It predates this window and is supporting context only. The video was not watched, and the original October case study, CLI source and full experimental data were not obtained. Detailed figures and extension-release status remain the candidate writer's account; the short official text does not confirm those numbers. No Java library, agent or benchmark was run here. REA is unmentioned; analysis-test status retains the lack of independent verification.

Sealed candidate: 4 likes, 183 views, 0 reposts, 1 reply. The 20–30% and roughly 65% figures are relayed combined-efficiency results; raw component data was not obtained.

## Sources

- [eltc9584's Netflix/IntelliJ research and benchmark account, November 24, 2026 at 09:50:14 Beijing time](https://x.com/i/status/2125044288727974397)
- [Supplementary official JetBrains post introducing Netflix collaboration, November 23, 2026 at 17:57:04 Beijing time, before the window; video not watched](https://x.com/jetbrains/status/2124804416259653985)

[中文](../netflix-intellij-headless-java-agent-navigation-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
